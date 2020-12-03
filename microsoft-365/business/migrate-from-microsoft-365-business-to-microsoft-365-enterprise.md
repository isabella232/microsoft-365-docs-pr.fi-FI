---
title: Siirtyminen Microsoft 365 Business-Microsoft 365 E3-tieto koneesta
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
description: Opi siirtämään yrityksesi Microsoft 365 Business Premiumista Microsoft 365 E3-tieto koneeseen.
ms.openlocfilehash: 3f1bb9591e1bd2bac49326325ce6c8c2d6778497
ms.sourcegitcommit: c1dd5be42fe0c5dcc7c05817c941edd9076febf8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/02/2020
ms.locfileid: "49558234"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="faf31-103">Siirtäminen Microsoft 365 Business Premiumista Microsoft 365 E3-tieto koneesta</span><span class="sxs-lookup"><span data-stu-id="faf31-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="faf31-104">Microsoft 365 Business Premiumissa on kaikki, mitä tarvitset pien yrityksellesi, yhdistämällä huippuhuippuiset pilvipohjaiset tuottavuus sovellukset yksinkertaiseen laite hallintaan ja tieto turvaan, jotka mahdollistavat työn tekijöiden parhaan työn.</span><span class="sxs-lookup"><span data-stu-id="faf31-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="faf31-105">Joissain tapa uksissa Microsoft 365 Business Premium-tilaus on ehkä siirrettävä Microsoft 365 E3-tila ukseen.</span><span class="sxs-lookup"><span data-stu-id="faf31-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span> 

<span data-ttu-id="faf31-106">Esimerkiksi yrityksesi on kasvanut ja tarvitsee enemmän kuin 300-käyttö oikeuksia (onneksi olkoon).</span><span class="sxs-lookup"><span data-stu-id="faf31-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="faf31-107">Tai yrityksesi tarvitsee yritys ominaisuuksia, kuten Microsoft 365-sovelluksia yritys käyttöön, Windows 10 Enterprise E3 tai Enterprise Client-käyttö oikeuksia (CALs).</span><span class="sxs-lookup"><span data-stu-id="faf31-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="faf31-108">Päivitys on helppoa: voit aloittaa päivityksen [hallinta keskuksesta](../commerce/subscriptions/upgrade-to-different-plan.md).</span><span class="sxs-lookup"><span data-stu-id="faf31-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="faf31-109">Kaikki nykyisen tilauksesi tiedot ja määritykset säilytetään.</span><span class="sxs-lookup"><span data-stu-id="faf31-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="faf31-110">Sinun ei tarvitse tehdä mitään, jos haluat valmistautua siirtoon eikä mitään jälkeenpäin, paitsi hyödyntää uusia ominaisuuksia.</span><span class="sxs-lookup"><span data-stu-id="faf31-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

>[!Note]
><span data-ttu-id="faf31-111">Voit käyttää myös Microsoft 365 Business Premium-pakettia, jossa on enintään 300 paikkaa ja saat Microsoft 365 E3-tila uksen, jossa on yli 300 paikkaa.</span><span class="sxs-lookup"><span data-stu-id="faf31-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="faf31-112">Microsoft Defender for Office 365 ei kuitenkaan sisälly Microsoft 365 E3-sovellukseen.</span><span class="sxs-lookup"><span data-stu-id="faf31-112">However, Microsoft Defender for Office 365 is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="faf31-113">Jos haluat jatkaa uhkien suojaamista, lisää Office 365-käyttö oikeuksien Defender, jotta kaikki Office 365-käytäntöjä koskevat käyttäjät saavat käyttö oikeuden.</span><span class="sxs-lookup"><span data-stu-id="faf31-113">For continued threat protection, you should add additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span>
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="faf31-114">Erot Microsoft 365 Business Premiumin ja Microsoft 365 Enterprisen välillä</span><span class="sxs-lookup"><span data-stu-id="faf31-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="faf31-115">Tässä taulukossa esitellään Microsoft 365 Business Premiumin ja Microsoft 365 E3-messujen erot.</span><span class="sxs-lookup"><span data-stu-id="faf31-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="faf31-116">Ominaisuus</span><span class="sxs-lookup"><span data-stu-id="faf31-116">Feature</span></span>    | <span data-ttu-id="faf31-117">Microsoft 365 Business Premiumin tuki</span><span class="sxs-lookup"><span data-stu-id="faf31-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="faf31-118">Tuki Microsoft 365 E3-sovelluksessa</span><span class="sxs-lookup"><span data-stu-id="faf31-118">Support in Microsoft 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="faf31-119">**Paikallinen**</span><span class="sxs-lookup"><span data-stu-id="faf31-119">**On-premises**</span></span>        | | | 
| <span data-ttu-id="faf31-120">Windows 10</span><span class="sxs-lookup"><span data-stu-id="faf31-120">Windows 10</span></span>    | <span data-ttu-id="faf31-121">Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="faf31-121">Windows 10 Business</span></span>  |     <span data-ttu-id="faf31-122">Windows 10 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="faf31-122">Windows 10 Enterprise E3</span></span>| 
| <span data-ttu-id="faf31-123">Office-sovellukset \*</span><span class="sxs-lookup"><span data-stu-id="faf31-123">Office apps\*</span></span>    | [<span data-ttu-id="faf31-124">Microsoft 365-sovellukset yrityksille</span><span class="sxs-lookup"><span data-stu-id="faf31-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="faf31-125">Microsoft 365 -yrityssovellukset</span><span class="sxs-lookup"><span data-stu-id="faf31-125">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="faf31-126">**Pilvi palveluiden tuottavuus sovellukset**</span><span class="sxs-lookup"><span data-stu-id="faf31-126">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="faf31-127">Exchange Online ja Outlook</span><span class="sxs-lookup"><span data-stu-id="faf31-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="faf31-128">50 gt tallennus tilan rajoitus posti laatikkoa kohden ja rajoittamaton Exchange Online-arkistointi</span><span class="sxs-lookup"><span data-stu-id="faf31-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="faf31-129">100 gt tallennus tilan rajoitus posti laatikkoa kohden ja rajoittamaton Exchange Online-arkistointi</span><span class="sxs-lookup"><span data-stu-id="faf31-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> | 
| <span data-ttu-id="faf31-130">Teams</span><span class="sxs-lookup"><span data-stu-id="faf31-130">Teams</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="faf31-133">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="faf31-133">OneDrive for Business</span></span>    | <span data-ttu-id="faf31-134">1 TERATAVUN tallennus tila raja käyttäjää kohden</span><span class="sxs-lookup"><span data-stu-id="faf31-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="faf31-135">Rajoittamattomat</span><span class="sxs-lookup"><span data-stu-id="faf31-135">Unlimited</span></span> | 
| <span data-ttu-id="faf31-136">Yammer, SharePoint Online, Planner, Streamin</span><span class="sxs-lookup"><span data-stu-id="faf31-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="faf31-139">MileIQ</span><span class="sxs-lookup"><span data-stu-id="faf31-139">MileIQ</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | | 
| <span data-ttu-id="faf31-141">**Uhkien suojaus**</span><span class="sxs-lookup"><span data-stu-id="faf31-141">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="faf31-142">Hyökkäys pinnan vähennys ominaisuudet</span><span class="sxs-lookup"><span data-stu-id="faf31-142">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="faf31-143">Katso tämä lista</span><span class="sxs-lookup"><span data-stu-id="faf31-143">See this list</span></span>](#threat-protection) | <span data-ttu-id="faf31-144">Microsoft Edgen laitteistopohjaisen eristämisen yritys hallinta</span><span class="sxs-lookup"><span data-stu-id="faf31-144">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> | 
| <span data-ttu-id="faf31-145">Office 365-paketin 1 Defender</span><span class="sxs-lookup"><span data-stu-id="faf31-145">Defender for Office 365 Plan 1</span></span> | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | <span data-ttu-id="faf31-147">Ei sisälly, mutta se voidaan lisätä</span><span class="sxs-lookup"><span data-stu-id="faf31-147">Not included, but can be added on</span></span> | 
| <span data-ttu-id="faf31-148">**Tunniste tietojen hallinta**</span><span class="sxs-lookup"><span data-stu-id="faf31-148">**Identity management**</span></span>        | | | 
| <span data-ttu-id="faf31-149">Omatoiminen Sala sanan palautus yhdistelmä Azure Active Directory (Azure AD)-tileillä, Azure AD Multi-Factor-todennus (MFA), ehdollinen käyttö oikeus, Sala sanan palauttaminen paikallisille identiteeteille</span><span class="sxs-lookup"><span data-stu-id="faf31-149">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="faf31-152">Pilvi sovellusten etsiminen, Azure AD Connect Health</span><span class="sxs-lookup"><span data-stu-id="faf31-152">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="faf31-154">Azure AD Office 365-sovellukset yksi Sign-On (SSO): 10 sovellusta käyttäjää kohden (Galleria SaaS-sovellukset, kuten Salesforce) \*</span><span class="sxs-lookup"><span data-stu-id="faf31-154">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="faf31-157">Azure AD Premium 1 SSO: ei rajoitusta (paikalliset sovellukset Azure AD Application Proxy-ja Non-Gallery-sovellusten kautta Self-Service sovellusten integrointi mallien avulla)</span><span class="sxs-lookup"><span data-stu-id="faf31-157">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="faf31-159">**Laitteen ja sovellusten hallinta**</span><span class="sxs-lookup"><span data-stu-id="faf31-159">**Device and app management**</span></span>        | | | 
| <span data-ttu-id="faf31-160">Microsoft Intune, Windowsin Autopilot</span><span class="sxs-lookup"><span data-stu-id="faf31-160">Microsoft Intune, Windows Autopilot</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
|<span data-ttu-id="faf31-163">Virtual Desktop Accessia (VDA)</span><span class="sxs-lookup"><span data-stu-id="faf31-163">Virtual Desktop Access (VDA)</span></span>    |  |     ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
|<span data-ttu-id="faf31-165">Windowsin Näennäistyöpöytä (WVD)</span><span class="sxs-lookup"><span data-stu-id="faf31-165">Windows Virtual Desktop (WVD)</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png) |     ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
|<span data-ttu-id="faf31-168">Jaettujen tieto koneiden Akti vointi (SCA)</span><span class="sxs-lookup"><span data-stu-id="faf31-168">Shared Computer Activation (SCA)</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png) |     ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="faf31-171">Microsoftin työpöydän optimointi paketti</span><span class="sxs-lookup"><span data-stu-id="faf31-171">Microsoft Desktop Optimization Package</span></span>    | |     ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="faf31-173">**Tieto turva**</span><span class="sxs-lookup"><span data-stu-id="faf31-173">**Information protection**</span></span>        | | | 
| <span data-ttu-id="faf31-174">Office 365 tietojen menetyksen estäminen, Azuren tieto turva sopimus 1</span><span class="sxs-lookup"><span data-stu-id="faf31-174">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="faf31-177">Ikkuna tieto turva pääte pisteen DLP</span><span class="sxs-lookup"><span data-stu-id="faf31-177">Window Information Protection for endpoint DLP</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="faf31-180">**Client Access License (CAL-käyttö oikeus)**</span><span class="sxs-lookup"><span data-stu-id="faf31-180">**Client Access License (CAL rights)**</span></span>    | | |     
| <span data-ttu-id="faf31-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoftin pääte pisteen määritysten hallinta, Windows Rights Management)</span><span class="sxs-lookup"><span data-stu-id="faf31-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="faf31-183">**Noudattamisen**</span><span class="sxs-lookup"><span data-stu-id="faf31-183">**Compliance**</span></span>        | | | 
| <span data-ttu-id="faf31-184">Rajoittamaton sähkö postin arkistointi</span><span class="sxs-lookup"><span data-stu-id="faf31-184">Unlimited email archiving</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="faf31-187">Yhteensopivuuden valvoja</span><span class="sxs-lookup"><span data-stu-id="faf31-187">Compliance Manager</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="faf31-190">eDiscovery</span><span class="sxs-lookup"><span data-stu-id="faf31-190">eDiscovery</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="faf31-193">Pidossa oleva pito ja oikeus toimiin liittyvään pitoon</span><span class="sxs-lookup"><span data-stu-id="faf31-193">In-place hold and litigation hold</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="faf31-196">Viestintä tietueiden hallinta (MRM) säilytys Tunnisteet ja säilytys käytännöt</span><span class="sxs-lookup"><span data-stu-id="faf31-196">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
||||

<span data-ttu-id="faf31-199">\* Käyttäjät, joille on määritetty SaaS-sovellusten käyttö oikeus, voivat hankkia KERTAKIRJAUTUMISEN jopa 10 sovellukseen.</span><span class="sxs-lookup"><span data-stu-id="faf31-199">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="faf31-200">Järjestelmänvalvojat voivat määrittää KERTAKIRJAUTUMISEN ja vaihtaa käyttö oikeuksia eri SaaS-sovelluksille, mutta kertakäyttöinen käyttö oikeus on sallittu vain 10: lle sovelluksen käyttäjää kohden kerrallaan.</span><span class="sxs-lookup"><span data-stu-id="faf31-200">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="faf31-201">Kaikki Office 365-sovellukset lasketaan yhdeksi sovellukseksi.</span><span class="sxs-lookup"><span data-stu-id="faf31-201">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="faf31-202">Siirto</span><span class="sxs-lookup"><span data-stu-id="faf31-202">Migration</span></span>

<span data-ttu-id="faf31-203">Jos haluat siirtää Microsoft 365 Business Premium-tila uksen ja käyttö oikeudet sopivan Microsoft 365 E3-tila ukseen, sinun on työskenneltävä yhdessä kumppanien kanssa.</span><span class="sxs-lookup"><span data-stu-id="faf31-203">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="faf31-204">Seuraavissa osissa kerrotaan, mitä muutoksia sinun on tehtävä ja mitä voit tehdä siirron jälkeen.</span><span class="sxs-lookup"><span data-stu-id="faf31-204">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="faf31-205">Microsoft 365-tila uksen määritykset ja tiedot</span><span class="sxs-lookup"><span data-stu-id="faf31-205">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="faf31-206">Sinun ei tarvitse tehdä muutoksia nykyiseen tilaukseesi tai tiedoihisi ennen siirtoa, joka sisältää seuraavat tiedot:</span><span class="sxs-lookup"><span data-stu-id="faf31-206">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="faf31-207">Tila uksen määritykset, kuten DNS-toimi alue nimet.</span><span class="sxs-lookup"><span data-stu-id="faf31-207">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="faf31-208">Käyttäjä-ja ryhmä tunnukset sekä todennus asetukset, kuten usean tekijän todentaminen tai ehdolliset käyttö oikeus käytännöt.</span><span class="sxs-lookup"><span data-stu-id="faf31-208">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="faf31-209">Tuottavuus palvelu määritykset ja niiden tiedot, kuten tiimit, Exchange Online-posti laatikot, SharePoint Online-sivustot, OneDrive for Business-kansiot ja OneNote-muisti kirjat.</span><span class="sxs-lookup"><span data-stu-id="faf31-209">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="faf31-210">Käyttäjät voivat nyt nauttia rajoittamattomasta tallennus tilasta Exchange Online-posti laatikoissa ja OneDrive for Business-kansioissa.</span><span class="sxs-lookup"><span data-stu-id="faf31-210">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="faf31-211">Voit aloittaa pilvi sovellusten etsimisen, Azure AD Connect Healthin ja SKERTA:N käytön yli 10 sovellukselle.</span><span class="sxs-lookup"><span data-stu-id="faf31-211">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

>[!Note]
><span data-ttu-id="faf31-212">Käyttäjät, jotka on siirretty Microsoft 365 E3-käyttö kohteeseen, eivät voi enää käyttää MileIQ-valmistetta</span><span class="sxs-lookup"><span data-stu-id="faf31-212">Users migrated to Microsoft 365 E3 can no longer use MileIQ.</span></span>
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="faf31-213">Uhkien suojaus</span><span class="sxs-lookup"><span data-stu-id="faf31-213">Threat protection</span></span>

<span data-ttu-id="faf31-214">Windows 10 Business sisältää seuraavat suoja ukset:</span><span class="sxs-lookup"><span data-stu-id="faf31-214">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="faf31-215">Käyttö järjestelmän käynnistys prosessin eheys valvonta</span><span class="sxs-lookup"><span data-stu-id="faf31-215">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="faf31-216">Arkaluonteisten käyttö komponenttien eheys valvonta</span><span class="sxs-lookup"><span data-stu-id="faf31-216">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="faf31-217">Kehittynyt haavoittuvuus ja nolla päivän heikkoutta hyödyntävät lieventävät tekijät</span><span class="sxs-lookup"><span data-stu-id="faf31-217">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="faf31-218">Maine-pohjainen verkon suojaus Microsoft Edgessä, Internet Explorerissa ja Chromessa</span><span class="sxs-lookup"><span data-stu-id="faf31-218">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="faf31-219">Isäntäpohjainen palo muuri</span><span class="sxs-lookup"><span data-stu-id="faf31-219">Host-based firewall</span></span>
- <span data-ttu-id="faf31-220">Kiristys ohjelmien lieventämis prosessit</span><span class="sxs-lookup"><span data-stu-id="faf31-220">Ransomware mitigations</span></span>
- <span data-ttu-id="faf31-221">Laitteistopohjainen eristys Microsoft Edgessä</span><span class="sxs-lookup"><span data-stu-id="faf31-221">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="faf31-222">Älykkään tieto turva graafin tarjoama sovellus ohjaus objekti</span><span class="sxs-lookup"><span data-stu-id="faf31-222">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="faf31-223">Device Control (USB)</span><span class="sxs-lookup"><span data-stu-id="faf31-223">Device control (USB)</span></span>
- <span data-ttu-id="faf31-224">Verkko suojaus verkkopohjaisia uhkia varten</span><span class="sxs-lookup"><span data-stu-id="faf31-224">Network protection for web-based threats</span></span>
- <span data-ttu-id="faf31-225">Isännän luvattoman käytön estämistä koskevat säännöt</span><span class="sxs-lookup"><span data-stu-id="faf31-225">Host intrusion prevention rules</span></span>

<span data-ttu-id="faf31-226">Windows 10 Enterprise E3 sisältää myös Microsoft Edgeen laitepohjaisen eristämisen yritys hallinnan.</span><span class="sxs-lookup"><span data-stu-id="faf31-226">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

>[!Note]
><span data-ttu-id="faf31-227">Käyttäjät, jotka on siirretty Microsoft 365 E3-käyttö oikeuteen, vaativat Microsoft Defender for Office 365-lisenssin jatkuvan uhkien suojaamiseksi.</span><span class="sxs-lookup"><span data-stu-id="faf31-227">Users migrated to Microsoft 365 E3 will each require a Microsoft Defender for Office 365 license for continued threat protection.</span></span> <span data-ttu-id="faf31-228">Varmista, että ostat lisää Office 365-käyttö oikeuksien Defender-ohjelman, jotta kaikki Office 365-käytäntöjä koskevat käyttäjät saavat käyttö oikeuden.</span><span class="sxs-lookup"><span data-stu-id="faf31-228">Be sure to purchase additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span> 
>

### <a name="device-management-with-intune"></a><span data-ttu-id="faf31-229">Laite hallinta Intune-palvelulla</span><span class="sxs-lookup"><span data-stu-id="faf31-229">Device management with Intune</span></span>

<span data-ttu-id="faf31-230">Sinun ei tarvitse tehdä muutoksia nykyiseen Intune-määritykseen ennen siirtoa, joka sisältää myös rekisteröityneet laitteet sekä laitteiden ja sovellusten asetukset.</span><span class="sxs-lookup"><span data-stu-id="faf31-230">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="faf31-231">Windows 10</span><span class="sxs-lookup"><span data-stu-id="faf31-231">Windows 10</span></span>

<span data-ttu-id="faf31-232">Microsoft 365 Business Premium sisältää Windows 10 Business-palvelu paketit, jotka voit asentaa Windows AutoPilot-asennuksen avulla.</span><span class="sxs-lookup"><span data-stu-id="faf31-232">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="faf31-233">Kun siirryt Microsoft 365 E3-käyttö järjestelmään, jokaiseen käyttäjän käyttö oikeuteen sisältyy Windows 10 Enterprise E3, jonka voit asentaa myös Windows Autopilot-ohjelmiston avulla.</span><span class="sxs-lookup"><span data-stu-id="faf31-233">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="faf31-234">Microsoft 365-sovellukset yrityksille</span><span class="sxs-lookup"><span data-stu-id="faf31-234">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="faf31-235">Laitteisiisi asennettu Microsoft 365-sovellusten yritys sovellus alkaa automaattisesti käyttää Microsoft 365-sovellusten ominaisuuksia yrityksessä.</span><span class="sxs-lookup"><span data-stu-id="faf31-235">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="faf31-236">Siirron jälkeen voit nyt käyttää:</span><span class="sxs-lookup"><span data-stu-id="faf31-236">After migration, you can now use:</span></span>

 - <span data-ttu-id="faf31-237">Määrä Akti vointi ryhmä käytännöllä</span><span class="sxs-lookup"><span data-stu-id="faf31-237">Volume activation through Group Policy</span></span>
 - <span data-ttu-id="faf31-238">Sovellustelemetria</span><span class="sxs-lookup"><span data-stu-id="faf31-238">App telemetry</span></span>
 - <span data-ttu-id="faf31-239">Päivitä komponentit</span><span class="sxs-lookup"><span data-stu-id="faf31-239">Update controls</span></span>
 - <span data-ttu-id="faf31-240">Laskenta taulukon vertailu ja kysely</span><span class="sxs-lookup"><span data-stu-id="faf31-240">Spreadsheet compare and inquire</span></span>
 - <span data-ttu-id="faf31-241">Liiketoiminta tiedot</span><span class="sxs-lookup"><span data-stu-id="faf31-241">Business intelligence</span></span>

