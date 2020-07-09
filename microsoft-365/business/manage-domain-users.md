---
title: Toimialueen käyttäjien synkronoiminen Microsoft 365:ksi
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
description: Synkronoi toimialueen hallitut käyttäjät Microsoft 365 for Businessin kanssa.
ms.openlocfilehash: af9cb7c9b2b639edc2375679a73ab41c4cf6de71
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081848"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="26c8d-103">Toimialueen käyttäjien synkronoiminen Microsoft 365:ksi</span><span class="sxs-lookup"><span data-stu-id="26c8d-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="26c8d-104">1. Hakemistosynkronoinnin valmisteleminen</span><span class="sxs-lookup"><span data-stu-id="26c8d-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="26c8d-105">Ennen kuin synkronoit käyttäjät ja tietokoneet paikallisesta Active Directory -toimialueesta, tutustu [ohjeaiheeseen Hakemistosynkronoinnin valmisteleminen Microsoft 365:ksi](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="26c8d-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="26c8d-106">Erityisesti:</span><span class="sxs-lookup"><span data-stu-id="26c8d-106">In particular:</span></span>

   - <span data-ttu-id="26c8d-107">Varmista, että hakemistossasi ei ole kaksoiskappaleita seuraaville määritteille: **sähköposti,** **proxyAddresses**ja **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="26c8d-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="26c8d-108">Näiden arvojen on oltava yksilöllisiä ja kaksoiskappaleet on poistettava.</span><span class="sxs-lookup"><span data-stu-id="26c8d-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="26c8d-109">Microsoft suosittelee, että määrität **userPrincipalName** (UPN) -määritteen kullekin paikalliselle käyttäjätilille vastaamaan lisensoitua Microsoft 365 -käyttäjää vastaavaa ensisijaista sähköpostiosoitetta.</span><span class="sxs-lookup"><span data-stu-id="26c8d-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="26c8d-110">Esimerkki: *mary.shelley@contoso.com* *mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="26c8d-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="26c8d-111">Jos Active Directory -toimialue päätyy ei-reititettävään liitteeseen , kuten *.local* tai *.lan*, internet-reititettävän liitteen , kuten *.com* tai *.org*, sijaan , säädä paikallisten käyttäjätilien UPN-liite ensin kohdassa [Ei-reititettävän toimialueen valmisteleminen hakemistosynkronointia varten](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)kuvatulla tavalla .</span><span class="sxs-lookup"><span data-stu-id="26c8d-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="26c8d-112">**Suorita IdFix** vaiheessa neljä (4) alla, myös varmistaa paikallinen Active Directory on valmis dir sync.</span><span class="sxs-lookup"><span data-stu-id="26c8d-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for dir sync.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="26c8d-113">2. Asenna ja määritä Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="26c8d-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="26c8d-114">Jos haluat synkronoida paikallisen Active Directoryn käyttäjät, ryhmät ja yhteystiedot Azure Active Directoryyn, asenna Azure Active Directory Connect ja määritä hakemistosynkronointi.</span><span class="sxs-lookup"><span data-stu-id="26c8d-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="26c8d-115">Valitse hallintakeskuksessa <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Asetukset** vasemmassa siirtymisruudussa.</span><span class="sxs-lookup"><span data-stu-id="26c8d-115">In the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="26c8d-116">Valitse **Kirjautumis- ja suojaus -kohdassa** **Synkronoi käyttäjiä organisaatiosi hakemistosta**-kohdassa **Näytä** .</span><span class="sxs-lookup"><span data-stu-id="26c8d-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="26c8d-117">Valitse **Synkronoi käyttäjät organisaatiosi hakemistosivulta** **Aloita**.</span><span class="sxs-lookup"><span data-stu-id="26c8d-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="26c8d-118">Ensimmäisessä vaiheessa suorita IdFix työkalu valmistautua Hakemistosynkronointia.</span><span class="sxs-lookup"><span data-stu-id="26c8d-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="26c8d-119">Lataa Azure AD Connect ohjatun toiminnon ohjeiden avulla ja synkronoi sen avulla toimialueohjatut käyttäjät Microsoft 365:ksi.</span><span class="sxs-lookup"><span data-stu-id="26c8d-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="26c8d-120">Lisätietoja on [ohjeaiheessa Microsoft 365:n hakemistosynkronoinnin määrittäminen.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)</span><span class="sxs-lookup"><span data-stu-id="26c8d-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="26c8d-121">Kun määrität Azure AD Connectin asetukset, suosittelemme, että otat käyttöön **salasanan synkronoinnin,** **saumattoman kertakirjautuksen**ja **salasanan takaisinkirjoitusominaisuuden,** jota myös Microsoft 365 for Business tukee.</span><span class="sxs-lookup"><span data-stu-id="26c8d-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="26c8d-122">Azure AD Connectin valintaruudun lisäksi salasanan takaisinkirjoituksessa on joitakin lisävaiheita.</span><span class="sxs-lookup"><span data-stu-id="26c8d-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="26c8d-123">Lisätietoja on [ohjeaiheessa Toimintaohjeet: salasanan takaisinkirjoituksen määrittäminen](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="26c8d-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="26c8d-124">Jos haluat hallita myös toimialueeseen liitettyjä Windows 10 -laitteita, katso lisätietoja ohjeaiheesta [Toimialueen käyttöönottamien windows 10 -laitteiden ottaminen käyttöön Microsoft 365 Business Premiumin hallinnassa](manage-windows-devices.md) azure AD -yhdistelmäliitoksen määrittämiseksi.</span><span class="sxs-lookup"><span data-stu-id="26c8d-124">If you want to manage domain-joined Windows 10 devices also, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 