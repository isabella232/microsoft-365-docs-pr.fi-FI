---
title: Toimialuekäyttäjien synkronoiminen Microsoft 365:lle
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Synkronoi toimialueohjatut käyttäjät Microsoft 365 for Businessin kanssa.
ms.openlocfilehash: 1c939dec7229f02991b15f08c48f184efecaddb0
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913250"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="bde96-103">Toimialuekäyttäjien synkronoiminen Microsoft 365:lle</span><span class="sxs-lookup"><span data-stu-id="bde96-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="bde96-104">1. Hakemistosynkronoinnin valmisteleminen</span><span class="sxs-lookup"><span data-stu-id="bde96-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="bde96-105">Ennen kuin synkronoit käyttäjät ja tietokoneet paikallisesta Active Directory -toimialueesta, tarkista Hakemistosynkronoinnin [valmisteleminen Microsoft 365:lle.](../enterprise/prepare-for-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="bde96-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](../enterprise/prepare-for-directory-synchronization.md).</span></span> <span data-ttu-id="bde96-106">Erityisesti:</span><span class="sxs-lookup"><span data-stu-id="bde96-106">In particular:</span></span>

   - <span data-ttu-id="bde96-107">Varmista, että hakemistossa ei ole kaksoiskappaleita seuraaville määritteille: **mail,** **proxyAddresses** ja **userPrincipalName.**</span><span class="sxs-lookup"><span data-stu-id="bde96-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="bde96-108">Näiden arvojen on oltava yksilöllisiä ja kaksoiskappaleet on poistettava.</span><span class="sxs-lookup"><span data-stu-id="bde96-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="bde96-109">Suosittelemme, että määrität kunkin paikallisen **käyttäjätilin userPrincipalName** (UPN) -määritteen vastaamaan ensisijaista sähköpostiosoitetta, joka vastaa lisensoituta Microsoft 365 -käyttäjää.</span><span class="sxs-lookup"><span data-stu-id="bde96-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="bde96-110">Esimerkki: *mary.shelley@contoso.com.mary@contoso* *sijaan*</span><span class="sxs-lookup"><span data-stu-id="bde96-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="bde96-111">Jos Active Directory -toimialue päättyy ei-reititettävään jälkiliitteeseen, kuten *.local* tai *.lan,* internet-reititettävän jälkiliitteen, kuten *.com* tai *.org,* sijaan, muokkaa ensin paikallisten käyttäjätilien UPN-jälkiliitettä kohdassa Valmistele ei-reititettävä toimialue hakemistosynkronointia varten kuvatulla [tavalla.](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="bde96-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md).</span></span> 

<span data-ttu-id="bde96-112">Suorita **IdFix vaiheessa** 4 (4) alla varmistaa myös, että paikallinen Active Directory on valmis hakemistosynkronointia varten.</span><span class="sxs-lookup"><span data-stu-id="bde96-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for directory synchronization.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="bde96-113">2. Azure AD Connectin asentaminen ja määrittäminen</span><span class="sxs-lookup"><span data-stu-id="bde96-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="bde96-114">Jos haluat synkronoida käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directoryyn, asenna Azure Active Directory Connect ja määritä hakemistosynkronointi.</span><span class="sxs-lookup"><span data-stu-id="bde96-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="bde96-115">Valitse [hallintakeskuksessa](https://go.microsoft.com/fwlink/p/?linkid=2024339)Asetukset **vasemmassa** siirtymisruudussa.</span><span class="sxs-lookup"><span data-stu-id="bde96-115">In the [admin center](https://go.microsoft.com/fwlink/p/?linkid=2024339), select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="bde96-116">Valitse **Sisäänkirjautuminen ja suojaus -kohdassa** **Näytä** kohdassa Synkronoi **käyttäjät organisaatiosi hakemistosta.**</span><span class="sxs-lookup"><span data-stu-id="bde96-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="bde96-117">Valitse **Organisaation hakemistosivun Synkronoi** käyttäjät -sivulla **Aloittaminen.**</span><span class="sxs-lookup"><span data-stu-id="bde96-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="bde96-118">Suorita ensimmäisessä vaiheessa IdFix-työkalu hakemistosynkronointia varten.</span><span class="sxs-lookup"><span data-stu-id="bde96-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="bde96-119">Lataa Azure AD Connect ohjatun toiminnon ohjeiden mukaisesti ja synkronoi sen avulla toimialueohjatut käyttäjät Microsoft 365:lle.</span><span class="sxs-lookup"><span data-stu-id="bde96-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="bde96-120">Lisätietoja [on kohdassa Hakemistosynkronoinnin](../enterprise/set-up-directory-synchronization.md) määrittäminen Microsoft 365:lle.</span><span class="sxs-lookup"><span data-stu-id="bde96-120">See [Set up directory synchronization for Microsoft 365](../enterprise/set-up-directory-synchronization.md) to learn more.</span></span>

<span data-ttu-id="bde96-121">Kun määrität Azure AD Connectin asetukset, suosittelemme, että otat käyttöön salasanojen  synkronoinnin,  **saumattoman** kertakirjautunnin ja salasanan takaisinkirjaamista varten, jota tuetaan myös Microsoft 365 for Businessissa.</span><span class="sxs-lookup"><span data-stu-id="bde96-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="bde96-122">On joitakin lisävaiheita salasanan palautusta varten Azure AD Connectin valintaruudun ulkopuolella.</span><span class="sxs-lookup"><span data-stu-id="bde96-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="bde96-123">Lisätietoja on ohjeaiheessa Ohjeet: salasanan [palautusten määrittäminen.](/azure/active-directory/authentication/howto-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="bde96-123">For more information, see [How-to: configure password writeback](/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="bde96-124">Jos haluat myös hallita toimialueeseen liitettyjä Windows 10 -laitteita, katso kohta Ota toimialueeseen yhdistetyt Windows 10 -laitteet käyttöön, joita [Microsoft 365 Business Premium hallitsee](manage-windows-devices.md) Azure AD -yhdistelmäympäristön liittämistä varten.</span><span class="sxs-lookup"><span data-stu-id="bde96-124">If you also want to manage domain-joined Windows 10 devices, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span>