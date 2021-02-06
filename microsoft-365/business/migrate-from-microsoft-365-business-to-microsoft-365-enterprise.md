---
title: Siirtyminen Microsoft 365 Businessista Microsoft 365 E3:lle
f1.keywords:
- NOCSH
ms.author: josephd
author: JoeDavies-MSFT
manager: laurawi
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Opi siirtämään yrityksesi Microsoft 365 Business Premiumista Microsoft 365 E3:lle.
ms.openlocfilehash: 019a422bb879389f42a32cf30f9a8094f776078a
ms.sourcegitcommit: eac5d9f759f290d3c51cafaf335a1a1c43ded927
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/06/2021
ms.locfileid: "50126197"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="82ac5-103">Siirtyminen Microsoft 365 Business Premiumista Microsoft 365 E3:lle</span><span class="sxs-lookup"><span data-stu-id="82ac5-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="82ac5-104">Microsoft 365 Business Premium sisältää kaiken, mitä tarvitset pienyritystä varten yhdistämällä luokkansa parhaat pilvipohjaiset tuottavuussovellukset yksinkertaiseen laitehallintaan ja tietoturvaan, joiden avulla työntekijät voivat tehdä parasta työtään.</span><span class="sxs-lookup"><span data-stu-id="82ac5-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="82ac5-105">Joissakin tapauksissa sinun on kuitenkin ehkä siirrettävä Microsoft 365 Business Premium -tilauksesi Microsoft 365 E3:lle.</span><span class="sxs-lookup"><span data-stu-id="82ac5-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span> 

<span data-ttu-id="82ac5-106">Yrityksesi on esimerkiksi kasvanut ja tarvitsee yli 300 käyttöoikeutta (onneksi olkoon).</span><span class="sxs-lookup"><span data-stu-id="82ac5-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="82ac5-107">Yrityksesi tarvitsee myös yritysominaisuuksia, kuten Microsoft 365 -sovellukset yrityksille, Windows 10 Enterprise E3 tai Enterprise Client Access Licenses (CALs).</span><span class="sxs-lookup"><span data-stu-id="82ac5-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="82ac5-108">Päivitys on helppoa: voit käynnistää päivityksen [hallintakeskuksesta.](../commerce/subscriptions/upgrade-to-different-plan.md)</span><span class="sxs-lookup"><span data-stu-id="82ac5-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="82ac5-109">Kaikki nykyisen tilauksesi tiedot ja määritykset säilytetään.</span><span class="sxs-lookup"><span data-stu-id="82ac5-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="82ac5-110">Sinun ei tarvitse valmistautua siirtoon eikä tehdä mitään sen jälkeen, paitsi hyödyntää uusia ominaisuuksia.</span><span class="sxs-lookup"><span data-stu-id="82ac5-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

>[!Note]
><span data-ttu-id="82ac5-111">Voit myös käyttää Microsoft 365 Business Premium -tilausta enintään 300 käyttöpaikkaa varten ja saada Microsoft 365 E3 -tilauksen, jossa on yli 300 käyttöpaikkaa.</span><span class="sxs-lookup"><span data-stu-id="82ac5-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="82ac5-112">Microsoft Defender for Office 365 ei kuitenkaan sisälly Microsoft 365 E3:lle.</span><span class="sxs-lookup"><span data-stu-id="82ac5-112">However, Microsoft Defender for Office 365 is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="82ac5-113">Jatkuvan uhkien suojauksen vuoksi sinun on lisättävä Office 365 -käyttöoikeuksiin ylimääräinen Defender, jotta kaikilla Defender for Office 365 -käyttäjillä on käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="82ac5-113">For continued threat protection, you should add additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span>
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="82ac5-114">Microsoft 365 Business Premiumin ja Microsoft 365 Enterprisen erot</span><span class="sxs-lookup"><span data-stu-id="82ac5-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="82ac5-115">Tässä taulukossa on esitetty Microsoft 365 Business Premiumin ja Microsoft 365 E3:n väliset erot.</span><span class="sxs-lookup"><span data-stu-id="82ac5-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="82ac5-116">Ominaisuus</span><span class="sxs-lookup"><span data-stu-id="82ac5-116">Feature</span></span>    | <span data-ttu-id="82ac5-117">Microsoft 365 Business Premiumin tuki</span><span class="sxs-lookup"><span data-stu-id="82ac5-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="82ac5-118">Microsoft 365 E3:n tuki</span><span class="sxs-lookup"><span data-stu-id="82ac5-118">Support in Microsoft 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="82ac5-119">**Paikallinen**</span><span class="sxs-lookup"><span data-stu-id="82ac5-119">**On-premises**</span></span>        | | | 
| <span data-ttu-id="82ac5-120">Windows 10</span><span class="sxs-lookup"><span data-stu-id="82ac5-120">Windows 10</span></span>    | <span data-ttu-id="82ac5-121">Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="82ac5-121">Windows 10 Business</span></span>  |     <span data-ttu-id="82ac5-122">Windows 10 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="82ac5-122">Windows 10 Enterprise E3</span></span>| 
| <span data-ttu-id="82ac5-123">Office-sovellukset\*</span><span class="sxs-lookup"><span data-stu-id="82ac5-123">Office apps\*</span></span>    | [<span data-ttu-id="82ac5-124">Microsoft 365 -sovellukset yrityksille</span><span class="sxs-lookup"><span data-stu-id="82ac5-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="82ac5-125">Microsoft 365 -yrityssovellukset</span><span class="sxs-lookup"><span data-stu-id="82ac5-125">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="82ac5-126">**Pilvipalvelun tuottavuussovellukset**</span><span class="sxs-lookup"><span data-stu-id="82ac5-126">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="82ac5-127">Exchange Online ja Outlook</span><span class="sxs-lookup"><span data-stu-id="82ac5-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="82ac5-128">50 Gigatavun tallennustilaraja postilaatikkoa kohden ja rajoittamaton Exchange Online -arkistointi</span><span class="sxs-lookup"><span data-stu-id="82ac5-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="82ac5-129">100 Gigatavun tallennustilaraja postilaatikkoa kohden ja rajoittamaton Exchange Online -arkistointi</span><span class="sxs-lookup"><span data-stu-id="82ac5-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> | 
| <span data-ttu-id="82ac5-130">Teams</span><span class="sxs-lookup"><span data-stu-id="82ac5-130">Teams</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="82ac5-133">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="82ac5-133">OneDrive for Business</span></span>    | <span data-ttu-id="82ac5-134">1 Tt tallennustilaraja käyttäjää kohden</span><span class="sxs-lookup"><span data-stu-id="82ac5-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="82ac5-135">Rajoittamaton</span><span class="sxs-lookup"><span data-stu-id="82ac5-135">Unlimited</span></span> | 
| <span data-ttu-id="82ac5-136">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="82ac5-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="82ac5-139">MileIQ</span><span class="sxs-lookup"><span data-stu-id="82ac5-139">MileIQ</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | | 
| <span data-ttu-id="82ac5-141">**Threat Protection**</span><span class="sxs-lookup"><span data-stu-id="82ac5-141">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="82ac5-142">Hyökkäyspinta-alaan pienentämisominaisuudet</span><span class="sxs-lookup"><span data-stu-id="82ac5-142">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="82ac5-143">Katso tämä luettelo</span><span class="sxs-lookup"><span data-stu-id="82ac5-143">See this list</span></span>](#threat-protection) | <span data-ttu-id="82ac5-144">Microsoft Edgen laitteistopohjaisen eristysympäristön yrityksen hallinta</span><span class="sxs-lookup"><span data-stu-id="82ac5-144">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> | 
| <span data-ttu-id="82ac5-145">Defender for Office 365 Plan 1</span><span class="sxs-lookup"><span data-stu-id="82ac5-145">Defender for Office 365 Plan 1</span></span> | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | <span data-ttu-id="82ac5-147">Ei sisälly, mutta se voidaan lisätä</span><span class="sxs-lookup"><span data-stu-id="82ac5-147">Not included, but can be added on</span></span> | 
| <span data-ttu-id="82ac5-148">**Käyttäjätietojen hallinta**</span><span class="sxs-lookup"><span data-stu-id="82ac5-148">**Identity management**</span></span>        | | | 
| <span data-ttu-id="82ac5-149">Azure Active Directory (Azure AD) -yhdistelmätilien omatoiminen salasanan palautus, Azure AD:n monimenetelmäinen todentaminen (MFA), ehdollinen käyttöoikeus, paikallisen käyttäjäryhmän salasanan palautus</span><span class="sxs-lookup"><span data-stu-id="82ac5-149">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="82ac5-152">Cloud App Discovery, Azure AD Connect Health</span><span class="sxs-lookup"><span data-stu-id="82ac5-152">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="82ac5-154">Azure AD Office 365 -sovellukset Sign-On (SSO): 10 sovellusta käyttäjää kohden (Valikoima SaaS -sovellukset, kuten Salesforce)\*</span><span class="sxs-lookup"><span data-stu-id="82ac5-154">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="82ac5-157">Azure AD Premium 1 SSO: ei rajoitusta (paikallinen sovellus Azure AD -sovelluksen välityspalvelimen ja muiden kuin valikoimasovellusten kautta käyttämällä Self-Service-integrointimalleja)</span><span class="sxs-lookup"><span data-stu-id="82ac5-157">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="82ac5-159">**Laitteiden ja sovellusten hallinta**</span><span class="sxs-lookup"><span data-stu-id="82ac5-159">**Device and app management**</span></span>        | | | 
| <span data-ttu-id="82ac5-160">Microsoft Intune, Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="82ac5-160">Microsoft Intune, Windows Autopilot</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="82ac5-163">Virtual Desktop Access (VDA)</span><span class="sxs-lookup"><span data-stu-id="82ac5-163">Virtual Desktop Access (VDA)</span></span>    |  |     ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="82ac5-165">Windowsin virtuaalityöpöytä (WVD)</span><span class="sxs-lookup"><span data-stu-id="82ac5-165">Windows Virtual Desktop (WVD)</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png) |     ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="82ac5-168">Jaetun tietokoneen aktivointi (SCA)</span><span class="sxs-lookup"><span data-stu-id="82ac5-168">Shared Computer Activation (SCA)</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png) |     ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="82ac5-171">Microsoftin työpöytäoptimoinnin paketti</span><span class="sxs-lookup"><span data-stu-id="82ac5-171">Microsoft Desktop Optimization Package</span></span>    | |     ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="82ac5-173">**Tietojen suojaus**</span><span class="sxs-lookup"><span data-stu-id="82ac5-173">**Information protection**</span></span>        | | | 
| <span data-ttu-id="82ac5-174">Office 365:n tietojen menetyksen estäminen, Azure Information Protection Plan 1</span><span class="sxs-lookup"><span data-stu-id="82ac5-174">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="82ac5-177">Window Information Protection for endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="82ac5-177">Window Information Protection for endpoint DLP</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="82ac5-180">**Client Access License (CAL-oikeudet)**</span><span class="sxs-lookup"><span data-stu-id="82ac5-180">**Client Access License (CAL rights)**</span></span>    | | |     
| <span data-ttu-id="82ac5-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windowsin oikeuksien hallinta)</span><span class="sxs-lookup"><span data-stu-id="82ac5-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="82ac5-183">**Yhteensopivuus**</span><span class="sxs-lookup"><span data-stu-id="82ac5-183">**Compliance**</span></span>        | | | 
| <span data-ttu-id="82ac5-184">Rajoittamattoman sähköpostin arkistointi</span><span class="sxs-lookup"><span data-stu-id="82ac5-184">Unlimited email archiving</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="82ac5-187">Yhteensopivuuden hallinta</span><span class="sxs-lookup"><span data-stu-id="82ac5-187">Compliance Manager</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="82ac5-190">eDiscovery</span><span class="sxs-lookup"><span data-stu-id="82ac5-190">eDiscovery</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="82ac5-193">Pito- ja oikeusistuntoon pito</span><span class="sxs-lookup"><span data-stu-id="82ac5-193">In-place hold and litigation hold</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="82ac5-196">Messaging Records Management (MRM) -säilytystunnisteet ja säilytyskäytännöt</span><span class="sxs-lookup"><span data-stu-id="82ac5-196">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
||||

<span data-ttu-id="82ac5-199">\* Käyttäjät, joilla on SaaS-sovellusten käyttöoikeus, voivat käyttää SSO-käyttöomme jopa 10 sovellusta.</span><span class="sxs-lookup"><span data-stu-id="82ac5-199">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="82ac5-200">Järjestelmänvalvojat voivat määrittää kertakirjautumisen ja muuttaa eri SaaS-sovellusten käyttöoheuksia, mutta kertakirjautumisen käyttö sallitaan vain 10 käyttäjälle kerrallaan.</span><span class="sxs-lookup"><span data-stu-id="82ac5-200">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="82ac5-201">Kaikki Office 365 -sovellukset lasketaan yhteen sovellukseen.</span><span class="sxs-lookup"><span data-stu-id="82ac5-201">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="82ac5-202">Siirto</span><span class="sxs-lookup"><span data-stu-id="82ac5-202">Migration</span></span>

<span data-ttu-id="82ac5-203">Siirrä Microsoft 365 Business Premium -tilauksesi ja -käyttöoikeutesi sopivaan Microsoft 365 E3 -tilaukseen, jonka käyttöoikeudet sinulla on, työskentele yhdessä kumppanisi kanssa.</span><span class="sxs-lookup"><span data-stu-id="82ac5-203">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="82ac5-204">Seuraavissa osissa kerrotaan, mitä muutoksia on tehtävä ja mitä voit tehdä siirron jälkeen.</span><span class="sxs-lookup"><span data-stu-id="82ac5-204">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="82ac5-205">Microsoft 365 -tilauksen määritykset ja tiedot</span><span class="sxs-lookup"><span data-stu-id="82ac5-205">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="82ac5-206">Sinun ei tarvitse tehdä muutoksia nykyiseen tilaukseesi tai tietoihin ennen sen muutosta, joka sisältää seuraavat:</span><span class="sxs-lookup"><span data-stu-id="82ac5-206">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="82ac5-207">Tilausmääritykset, kuten DNS-toimialuenimet.</span><span class="sxs-lookup"><span data-stu-id="82ac5-207">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="82ac5-208">Käyttäjä- ja ryhmätilit ja todennusasetukset, kuten monimenetelmäinen todentaminen tai ehdollisten käyttöoikeuksien käytännöt.</span><span class="sxs-lookup"><span data-stu-id="82ac5-208">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="82ac5-209">Tuottavuuspalvelun määritykset ja niiden tiedot, kuten Teams, Exchange Online -postilaatikot, SharePoint Online -sivustot, OneDrive for Business -kansiot ja OneNote-muistikirjat.</span><span class="sxs-lookup"><span data-stu-id="82ac5-209">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="82ac5-210">Käyttäjät voivat nyt nauttia rajoittamattomasta tallennustilasta Exchange Online -postilaatikoissa ja OneDrive for Business -kansioissa.</span><span class="sxs-lookup"><span data-stu-id="82ac5-210">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="82ac5-211">Voit aloittaa Cloud App Discoveryn, Azure AD Connect Healthin ja SSO:n käytön yli 10 sovellukselle.</span><span class="sxs-lookup"><span data-stu-id="82ac5-211">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

>[!Note]
><span data-ttu-id="82ac5-212">Microsoft 365 E3:lle siirretyt käyttäjät eivät voi enää käyttää MileIQ:a.</span><span class="sxs-lookup"><span data-stu-id="82ac5-212">Users migrated to Microsoft 365 E3 can no longer use MileIQ.</span></span>
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="82ac5-213">Uhkien torjunta</span><span class="sxs-lookup"><span data-stu-id="82ac5-213">Threat protection</span></span>

<span data-ttu-id="82ac5-214">Windows 10 Business sisältää seuraavat suojaukset:</span><span class="sxs-lookup"><span data-stu-id="82ac5-214">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="82ac5-215">Käyttöjärjestelmän käynnistysprosessin eheyden pakotus</span><span class="sxs-lookup"><span data-stu-id="82ac5-215">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="82ac5-216">Arkaluonteisten käyttökomponenttien eheyden pakotus</span><span class="sxs-lookup"><span data-stu-id="82ac5-216">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="82ac5-217">Kehittynyt haavoittuvuus ja nollapäiväinen haun riskien lieventäminen</span><span class="sxs-lookup"><span data-stu-id="82ac5-217">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="82ac5-218">Microsoft Edgen, Internet Explorerin ja Chromen mainepohjainen verkon suojaus</span><span class="sxs-lookup"><span data-stu-id="82ac5-218">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="82ac5-219">Isäntäpohjainen palomuuri</span><span class="sxs-lookup"><span data-stu-id="82ac5-219">Host-based firewall</span></span>
- <span data-ttu-id="82ac5-220">Kiristysohjelmien riskien lieventäminen</span><span class="sxs-lookup"><span data-stu-id="82ac5-220">Ransomware mitigations</span></span>
- <span data-ttu-id="82ac5-221">Microsoft Edgen laitteistopohjainen eristys</span><span class="sxs-lookup"><span data-stu-id="82ac5-221">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="82ac5-222">Älykkään suojauskaavion sovellusohjausobjekti</span><span class="sxs-lookup"><span data-stu-id="82ac5-222">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="82ac5-223">Laiteohjaus (USB)</span><span class="sxs-lookup"><span data-stu-id="82ac5-223">Device control (USB)</span></span>
- <span data-ttu-id="82ac5-224">Verkkosuojaus verkkopohjaisia uhkia varten</span><span class="sxs-lookup"><span data-stu-id="82ac5-224">Network protection for web-based threats</span></span>
- <span data-ttu-id="82ac5-225">Isännän tunkeilun estämissäännöt</span><span class="sxs-lookup"><span data-stu-id="82ac5-225">Host intrusion prevention rules</span></span>

<span data-ttu-id="82ac5-226">Windows 10 Enterprise E3 sisältää myös laitteistopohjaisen eristysympäristön hallinnan Microsoft Edgessä.</span><span class="sxs-lookup"><span data-stu-id="82ac5-226">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

>[!Note]
><span data-ttu-id="82ac5-227">Microsoft 365 E3:lle siirretyt käyttäjät edellyttävät microsoft Defender for Office 365 -käyttöoikeutta, jotta he voivat jatkaa uhkientorjuntaa.</span><span class="sxs-lookup"><span data-stu-id="82ac5-227">Users migrated to Microsoft 365 E3 will each require a Microsoft Defender for Office 365 license for continued threat protection.</span></span> <span data-ttu-id="82ac5-228">Muista ostaa lisää Defender for Office 365 -käyttöoikeuksia, jotta kaikilla Defender for Office 365 -käyttäjillä on käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="82ac5-228">Be sure to purchase additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span> 
>

### <a name="device-management-with-intune"></a><span data-ttu-id="82ac5-229">Laitehallinta Intunen avulla</span><span class="sxs-lookup"><span data-stu-id="82ac5-229">Device management with Intune</span></span>

<span data-ttu-id="82ac5-230">Sinun ei tarvitse tehdä muutoksia nykyiseen Intune-määritykseesi ennen sen muutosta, joka sisältää rekisteröidyt laitteet sekä laite- ja sovellusasetukset.</span><span class="sxs-lookup"><span data-stu-id="82ac5-230">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="82ac5-231">Windows 10</span><span class="sxs-lookup"><span data-stu-id="82ac5-231">Windows 10</span></span>

<span data-ttu-id="82ac5-232">Microsoft 365 Business Premium sisältää Windows 10 Businessin, jonka voit asentaa Windows AutoPilotilla.</span><span class="sxs-lookup"><span data-stu-id="82ac5-232">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="82ac5-233">Kun siirryt Microsoft 365 E3:lle, jokainen käyttöoikeus sisältää Windows 10 Enterprise E3:n, jonka voit asentaa myös Windows Autopilotilla.</span><span class="sxs-lookup"><span data-stu-id="82ac5-233">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="82ac5-234">Microsoft 365 -sovellukset yrityksille</span><span class="sxs-lookup"><span data-stu-id="82ac5-234">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="82ac5-235">Laitteisiisi asennetut Microsoft 365 Apps for Business -sovellukset alkavat automaattisesti käyttää Microsoft 365 Apps for Enterprisen ominaisuuksia.</span><span class="sxs-lookup"><span data-stu-id="82ac5-235">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="82ac5-236">Siirron jälkeen voit nyt käyttää:</span><span class="sxs-lookup"><span data-stu-id="82ac5-236">After migration, you can now use:</span></span>

 - <span data-ttu-id="82ac5-237">Ryhmäkäytäntöjen tuki</span><span class="sxs-lookup"><span data-stu-id="82ac5-237">Group Policy support</span></span>
 - <span data-ttu-id="82ac5-238">Spreadsheet Compare ja inquire</span><span class="sxs-lookup"><span data-stu-id="82ac5-238">Spreadsheet compare and inquire</span></span>
 - <span data-ttu-id="82ac5-239">Liiketoimintatiedot</span><span class="sxs-lookup"><span data-stu-id="82ac5-239">Business intelligence</span></span>

