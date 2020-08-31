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
description: Synkronoi toimi alueen valvottavat käyttäjät Microsoft 365 for Businessin kanssa.
ms.openlocfilehash: 9495d893eb6870ef7c417a78f921296bfc0e6705
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306445"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="5aed9-103">Toimi alueen käyttäjien synkronoiminen Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5aed9-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="5aed9-104">1. hakemisto synkronoinnin valmisteleminen</span><span class="sxs-lookup"><span data-stu-id="5aed9-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="5aed9-105">Ennen kuin synkronoit käyttäjät ja tieto koneet paikallisesta Active Directory-toimi alueesta, tarkista [Hakemisto synkronoinnin valmisteleminen Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="5aed9-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="5aed9-106">Erityisesti:</span><span class="sxs-lookup"><span data-stu-id="5aed9-106">In particular:</span></span>

   - <span data-ttu-id="5aed9-107">Varmista, ettei hakemistossasi ole kaksoiskappaleita seuraavista määritteistä: **Sähkö posti**, **proxyAddresses**ja **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="5aed9-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="5aed9-108">Näiden arvojen on oltava yksilöllisiä, ja kaikki kaksoiskappaleet on poistettava.</span><span class="sxs-lookup"><span data-stu-id="5aed9-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="5aed9-109">Suosittelemme määrittämään kunkin paikallisen käyttäjä tilin **userPrincipalName** (UPN)-määritteen vastaamaan Microsoft 365-käyttö oikeutta vastaavaa pääsähkö posti osoitetta.</span><span class="sxs-lookup"><span data-stu-id="5aed9-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="5aed9-110">Esimerkki: *Mary.Shelley@contoso.com* sen sijaan, että *Mary@contoso. Local*</span><span class="sxs-lookup"><span data-stu-id="5aed9-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="5aed9-111">Jos Active Directory-toimi alueen pääte on muu kuin reititettävissä oleva jälki liite (esimerkiksi. *Local* tai *. LAN*) sen sijaan, että käytössä olisi Internet-reititettävissä oleva jälki liite, kuten *. com* tai *. org*, voit muuttaa paikallisten käyttäjä tunnusten UPN-jälki liitettä ensin, kun [olet kuvannut ei-reititettävän toimi alueen määrittäminen hakemisto synkronointia](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)</span><span class="sxs-lookup"><span data-stu-id="5aed9-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="5aed9-112">Vaiheen neljä (4) **Suorita IdFix-korjaus** varmistaa myös, että paikallinen Active Directory on valmiina dir-synkronointia varten.</span><span class="sxs-lookup"><span data-stu-id="5aed9-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for dir sync.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="5aed9-113">2. Azure AD Connectin asentaminen ja määrittäminen</span><span class="sxs-lookup"><span data-stu-id="5aed9-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="5aed9-114">Jos haluat synkronoida paikallisen Active Directoryn käyttäjät, ryhmät ja yhteys tiedot Azure Active Directoryyn, asenna Azure Active Directory Connect ja Määritä hakemisto synkronointi.</span><span class="sxs-lookup"><span data-stu-id="5aed9-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="5aed9-115">Valitse hallinta keskuksessa <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> vasemmanpuoleisen siirtymis palkin **Asetukset** -kohdassa.</span><span class="sxs-lookup"><span data-stu-id="5aed9-115">In the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="5aed9-116">Valitse **Kirjautuminen ja tieto turva**-kohdassa **oman organisaatiosi hakemiston Synkronoi käyttäjät**-kohdassa **Näytä** .</span><span class="sxs-lookup"><span data-stu-id="5aed9-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="5aed9-117">Valitse organisaatiosi **hakemisto-sivun Synkronoi käyttäjät** -kohdassa **aloittaminen**.</span><span class="sxs-lookup"><span data-stu-id="5aed9-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="5aed9-118">Voit valmistella hakemisto synkronoinnin ensimmäisessä vaiheessa suorittamalla IdFix-työkalun.</span><span class="sxs-lookup"><span data-stu-id="5aed9-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="5aed9-119">Lataa Azure AD Connect noudattamalla ohjatun toiminnon ohjeita ja synkronoi toimi alueen hallitsemat käyttäjät Microsoft 365-palvelussa sen avulla.</span><span class="sxs-lookup"><span data-stu-id="5aed9-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="5aed9-120">Lisä tietoja on artikkelissa [Hakemisto synkronoinnin määrittäminen Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) -käyttöön.</span><span class="sxs-lookup"><span data-stu-id="5aed9-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="5aed9-121">Kun määrität asetukset Azure AD Connect-sovelluksessa, suosittelemme, että otat käyttöön **Sala sanojen synkronoinnin**, **saumattoman kertakirjautumisen**ja **Sala sanan takaisinkirjoitusominaisuuden** , jota tuetaan myös Microsoft 365 for Businessissa.</span><span class="sxs-lookup"><span data-stu-id="5aed9-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="5aed9-122">Sala sanan takaisinkirjoitus on käytettävissä myös muilla tavoilla Azure AD Connectin valinta ruudun ulkopuolella.</span><span class="sxs-lookup"><span data-stu-id="5aed9-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="5aed9-123">Lisä tietoja on Ohje aiheessa [toiminta ohjeet: Sala sanan takaisinkirjoitus-kohdan määrittäminen](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="5aed9-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="5aed9-124">Jos haluat hallita toimi alueen mukaan liitetyissä Windows 10-laitteissa, Katso lisä tietoja artikkelista [Microsoft 365 Business Premiumin hallinnoitava toimi alue-yhdistetyt Windows 10-laitteet](manage-windows-devices.md) , jotta voit määrittää yhdistelmä ympäristön Azure AD Join.</span><span class="sxs-lookup"><span data-stu-id="5aed9-124">If you want to manage domain-joined Windows 10 devices also, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 