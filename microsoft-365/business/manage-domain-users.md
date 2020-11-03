---
title: Toimi alueen käyttäjien synkronoiminen Microsoft 365
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
description: Synkronoi toimi alueen hallitsemat käyttäjät Microsoft 365 for Businessin kanssa.
ms.openlocfilehash: b40a995a1723808d2fd171c534e9131a891840ba
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841355"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="621a6-103">Toimi alueen käyttäjien synkronoiminen Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="621a6-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="621a6-104">1. hakemisto synkronoinnin valmisteleminen</span><span class="sxs-lookup"><span data-stu-id="621a6-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="621a6-105">Ennen kuin synkronoit käyttäjät ja tieto koneet paikallisesta Active Directory-toimi alueesta, tarkista [Hakemisto synkronoinnin valmisteleminen Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="621a6-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="621a6-106">Erityisesti:</span><span class="sxs-lookup"><span data-stu-id="621a6-106">In particular:</span></span>

   - <span data-ttu-id="621a6-107">Varmista, ettei hakemistossasi ole kaksoiskappaleita seuraavista määritteistä: **Sähkö posti** , **proxyAddresses** ja **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="621a6-107">Make sure that no duplicates exist in your directory for the following attributes: **mail** , **proxyAddresses** , and **userPrincipalName**.</span></span> <span data-ttu-id="621a6-108">Näiden arvojen on oltava yksilöllisiä, ja kaikki kaksoiskappaleet on poistettava.</span><span class="sxs-lookup"><span data-stu-id="621a6-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="621a6-109">Suosittelemme määrittämään kunkin paikallisen käyttäjä tilin **userPrincipalName** (UPN)-määritteen vastaamaan Microsoft 365-käyttö oikeutta vastaavaa pääsähkö posti osoitetta.</span><span class="sxs-lookup"><span data-stu-id="621a6-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="621a6-110">Esimerkki: *Mary.Shelley@contoso.com* sen sijaan, että *Mary@contoso. Local*</span><span class="sxs-lookup"><span data-stu-id="621a6-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="621a6-111">Jos Active Directory-toimi alueen pääte on muu kuin reititettävissä oleva jälki liite (esimerkiksi. *Local* tai *. LAN* ) sen sijaan, että käytössä olisi Internet-reititettävissä oleva jälki liite, kuten *. com* tai *. org* , voit muuttaa paikallisten käyttäjä tunnusten UPN-jälki liitettä ensin, kun [olet kuvannut ei-reititettävän toimi alueen määrittäminen hakemisto synkronointia](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)</span><span class="sxs-lookup"><span data-stu-id="621a6-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan* , instead of an internet routable suffix such as *.com* or *.org* , adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="621a6-112">Vaiheen neljä (4) **Suorita IdFix-korjaus** varmistaa myös, että paikallinen Active Directory-hakemisto on valmis hakemisto synkronointiin.</span><span class="sxs-lookup"><span data-stu-id="621a6-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for directory synchronization.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="621a6-113">2. Azure AD Connectin asentaminen ja määrittäminen</span><span class="sxs-lookup"><span data-stu-id="621a6-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="621a6-114">Jos haluat synkronoida paikallisen Active Directoryn käyttäjät, ryhmät ja yhteys tiedot Azure Active Directoryyn, asenna Azure Active Directory Connect ja Määritä hakemisto synkronointi.</span><span class="sxs-lookup"><span data-stu-id="621a6-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="621a6-115">Valitse [hallinta keskuksessa](https://go.microsoft.com/fwlink/p/?linkid=2024339) **Asetukset** vasemmanpuoleisesta siirtymis ruudusta.</span><span class="sxs-lookup"><span data-stu-id="621a6-115">In the [admin center](https://go.microsoft.com/fwlink/p/?linkid=2024339), select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="621a6-116">Valitse **Kirjautuminen ja tieto turva** -kohdassa **oman organisaatiosi hakemiston Synkronoi käyttäjät** -kohdassa **Näytä** .</span><span class="sxs-lookup"><span data-stu-id="621a6-116">Under **Sign-in and security** , choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="621a6-117">Valitse organisaatiosi **hakemisto-sivun Synkronoi käyttäjät** -kohdassa **aloittaminen**.</span><span class="sxs-lookup"><span data-stu-id="621a6-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="621a6-118">Voit valmistella hakemisto synkronoinnin ensimmäisessä vaiheessa suorittamalla IdFix-työkalun.</span><span class="sxs-lookup"><span data-stu-id="621a6-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="621a6-119">Lataa Azure AD Connect noudattamalla ohjatun toiminnon ohjeita ja synkronoi toimi alueen hallitsemat käyttäjät Microsoft 365-palvelussa sen avulla.</span><span class="sxs-lookup"><span data-stu-id="621a6-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="621a6-120">Lisä tietoja on artikkelissa [Hakemisto synkronoinnin määrittäminen Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) -käyttöön.</span><span class="sxs-lookup"><span data-stu-id="621a6-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="621a6-121">Kun määrität asetukset Azure AD Connect-sovelluksessa, suosittelemme, että otat käyttöön **Sala sanojen synkronoinnin** , **saumattoman kertakirjautumisen** ja **Sala sanan takaisinkirjoitusominaisuuden** , jota tuetaan myös Microsoft 365 for Businessissa.</span><span class="sxs-lookup"><span data-stu-id="621a6-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization** , **Seamless Single Sign-On** , and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="621a6-122">Sala sanan takaisinkirjoitus on käytettävissä myös muilla tavoilla Azure AD Connectin valinta ruudun ulkopuolella.</span><span class="sxs-lookup"><span data-stu-id="621a6-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="621a6-123">Lisä tietoja on Ohje aiheessa [toiminta ohjeet: Sala sanan takaisinkirjoitus-kohdan määrittäminen](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="621a6-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="621a6-124">Jos haluat myös hallita toimi alueeseen liittyneitä Windows 10-laitteita, Katso lisä tietoja artikkelista [Microsoft 365 Business Premiumin hallinnoitava toimi alue-yhdistetyt Windows 10-laitteet](manage-windows-devices.md) , jotta voit määrittää hybridi-Azure-mainos liitoksen.</span><span class="sxs-lookup"><span data-stu-id="621a6-124">If you also want to manage domain-joined Windows 10 devices, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 