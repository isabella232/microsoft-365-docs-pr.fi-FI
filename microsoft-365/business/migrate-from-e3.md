---
title: Siirtyminen Microsoft 365-yritykseen Office 365 E3-tieto koneesta
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
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
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Opi siirtämään yrityksesi Microsoft 365 Business Premiumiin Office 365 E3-tieto koneesta.
ms.openlocfilehash: b8aa58f1f050ec6247479ed02e142507a2df45fc
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842156"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="09a4a-103">Siirtyminen Office 365 E3-tieto koneesta Microsoft 365 Business Premiumiin</span><span class="sxs-lookup"><span data-stu-id="09a4a-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span> 

<span data-ttu-id="09a4a-104">Microsoft 365 Business Premiumissa on kaikki, mitä tarvitset pien yrityksellesi, yhdistämällä luokkansa parhaat pilvipohjaiset tuottavuus sovellukset yksinkertaiseen laitteiden hallintaan ja tieto turvaan.</span><span class="sxs-lookup"><span data-stu-id="09a4a-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="09a4a-105">Jos sinulla on tällä hetkellä Office 365 E3-tilaus, mutta sinulla ei ole enempää kuin 300 työn tekijää, harkitse siirtymistä käyttämään Microsoft 365 Business Premiumia tieto turva ominaisuuksien lisäämiseen.</span><span class="sxs-lookup"><span data-stu-id="09a4a-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="09a4a-106">Siirtäminen on helppoa: ensin vaihdat käyttö oikeuksia ja kaikki tiedot ja käyttäjä tiedot nykyisessä paketilassasi säilytetään.</span><span class="sxs-lookup"><span data-stu-id="09a4a-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="09a4a-107">Siirron jälkeen sinun on määritettävä Microsoft 365 Business Premiumiin lisätyt ominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="09a4a-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="09a4a-108">Office 365 E3-ja Microsoft 365 Business Premium-erot</span><span class="sxs-lookup"><span data-stu-id="09a4a-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="09a4a-109">Tässä taulukossa esitellään Microsoft 365 Business Premiumin ja Office 365 E3-ohjelmien erot.</span><span class="sxs-lookup"><span data-stu-id="09a4a-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="09a4a-110">Ominaisuus</span><span class="sxs-lookup"><span data-stu-id="09a4a-110">Feature</span></span>    | <span data-ttu-id="09a4a-111">Microsoft 365 Business Premiumin tuki</span><span class="sxs-lookup"><span data-stu-id="09a4a-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="09a4a-112">Office 365 E3-tuki</span><span class="sxs-lookup"><span data-stu-id="09a4a-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="09a4a-113">**Paikallinen**</span><span class="sxs-lookup"><span data-stu-id="09a4a-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="09a4a-114">Office-sovellukset<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="09a4a-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="09a4a-115">Microsoft 365-sovellukset yrityksille</span><span class="sxs-lookup"><span data-stu-id="09a4a-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="09a4a-116">Microsoft 365 -sovellukset yrityksille</span><span class="sxs-lookup"><span data-stu-id="09a4a-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="09a4a-117">**Pilvi palveluiden tuottavuus sovellukset**</span><span class="sxs-lookup"><span data-stu-id="09a4a-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="09a4a-118">Exchange Online ja Outlook</span><span class="sxs-lookup"><span data-stu-id="09a4a-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="09a4a-119">50 gt tallennus tilan rajoitus posti laatikkoa kohden ja rajoittamaton Exchange Online-arkistointi</span><span class="sxs-lookup"><span data-stu-id="09a4a-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="09a4a-120">100 gt tallennus tilan rajoitus posti laatikkoa kohden ja rajoittamaton Exchange Online-arkistointi</span><span class="sxs-lookup"><span data-stu-id="09a4a-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="09a4a-121">Teams</span><span class="sxs-lookup"><span data-stu-id="09a4a-121">Teams</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="09a4a-124">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="09a4a-124">OneDrive for Business</span></span>    | <span data-ttu-id="09a4a-125">1 TERATAVUN tallennus tila raja käyttäjää kohden</span><span class="sxs-lookup"><span data-stu-id="09a4a-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="09a4a-126">Rajoittamattomat</span><span class="sxs-lookup"><span data-stu-id="09a4a-126">Unlimited</span></span> | 
| <span data-ttu-id="09a4a-127">Yammer, SharePoint Online, Planner, Streamin</span><span class="sxs-lookup"><span data-stu-id="09a4a-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="09a4a-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="09a4a-130">StaffHub</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3-pakettiin](../media/check-mark.png) | 
| <span data-ttu-id="09a4a-133">Outlook Customer Managerilla, Mireiq</span><span class="sxs-lookup"><span data-stu-id="09a4a-133">Outlook Customer Manager, MileIQ</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | | 
| <span data-ttu-id="09a4a-135">**Uhkien suojaus**</span><span class="sxs-lookup"><span data-stu-id="09a4a-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="09a4a-136">Office 365-paketin 1 Defender</span><span class="sxs-lookup"><span data-stu-id="09a4a-136">Defender for Office 365 Plan 1</span></span> | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | <span data-ttu-id="09a4a-138">Ei sisälly, mutta se voidaan lisätä</span><span class="sxs-lookup"><span data-stu-id="09a4a-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="09a4a-139">**Tunniste tietojen hallinta**</span><span class="sxs-lookup"><span data-stu-id="09a4a-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="09a4a-140">Omatoiminen Sala sanan palautus (yhdistelmä Azure Active Directory (Azure AD)-tilit, Azure Multi-Factor-todennus (MFA), ehdollinen käyttö oikeus, Sala sanan palauttaminen paikallisille identiteeteille</span><span class="sxs-lookup"><span data-stu-id="09a4a-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    |  | 
| <span data-ttu-id="09a4a-142">**Laitteen ja sovellusten hallinta**</span><span class="sxs-lookup"><span data-stu-id="09a4a-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="09a4a-143">Microsoft Intune, Windowsin AutoPilot</span><span class="sxs-lookup"><span data-stu-id="09a4a-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    |  |
| <span data-ttu-id="09a4a-145">Jaettujen tieto koneiden Akti vointi</span><span class="sxs-lookup"><span data-stu-id="09a4a-145">Shared computer activation</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3-pakettiin](../media/check-mark.png)| 
| <span data-ttu-id="09a4a-148">Windows 10 Pron päivitys oikeudet Win 7/8.1 Pro-käyttö oikeuksista</span><span class="sxs-lookup"><span data-stu-id="09a4a-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    || 
| <span data-ttu-id="09a4a-150">**Tieto turva**</span><span class="sxs-lookup"><span data-stu-id="09a4a-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="09a4a-151">Office 365-tietojen menetyksen estäminen</span><span class="sxs-lookup"><span data-stu-id="09a4a-151">Office 365 Data Loss Prevention</span></span>|    ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)|![Sisältyy Office 365 E3-pakettiin](../media/check-mark.png)|
|<span data-ttu-id="09a4a-154">Azure Information Protectionin tieto turva sopimus 1, BitLocker-valvonta</span><span class="sxs-lookup"><span data-stu-id="09a4a-154">Azure Information Protection Plan 1, Bitlocker enforcement</span></span>|![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)||
|<span data-ttu-id="09a4a-156">Azuren tieto turva sopimus 1, herkkyys Tunnisteet</span><span class="sxs-lookup"><span data-stu-id="09a4a-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)||
|<span data-ttu-id="09a4a-158">**Client Access License (CAL-käyttö oikeus)**</span><span class="sxs-lookup"><span data-stu-id="09a4a-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="09a4a-159">Enterprise CAL-ohjelmisto paketti (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="09a4a-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Sisältyy Office 365 E3-pakettiin](../media/check-mark.png)|

<span data-ttu-id="09a4a-161"><sup>1</sup> Office-sovellusten Microsoft 365 Business Premium-versioon ei kuulu määrä Akti vointia ryhmä käytännöllä, sovellustelemetrialla, päivitys komponenteilla, laskenta taulukon vertailujen ja kysely-tai yritys tietojen avulla.</span><span class="sxs-lookup"><span data-stu-id="09a4a-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="09a4a-162">Siirto</span><span class="sxs-lookup"><span data-stu-id="09a4a-162">Migration</span></span>

<span data-ttu-id="09a4a-163">Jos haluat siirtää tila uksen, Katso ohjeet artikkelista palvelu [pakettien muuttaminen manuaalisesti](../commerce/subscriptions/change-plans-manually.md) , jotta voit siirtyä vain muutamasta henkilöstä Microsoft 365 Business Premiumiin.</span><span class="sxs-lookup"><span data-stu-id="09a4a-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="09a4a-164">Voit myös [päivittää kaikki automaattisesti](../commerce/subscriptions/upgrade-to-different-plan.md)tai käyttää kumppania, jos haluat siirtää E3-tilauksesi ja käyttö oikeutesi Microsoft 365 Business Premium-tila ukseen.</span><span class="sxs-lookup"><span data-stu-id="09a4a-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="09a4a-165">Seuraavissa osissa kuvataan muutokset, jotka sinun on tehtävä ja mitä voit tehdä siirron jälkeen.</span><span class="sxs-lookup"><span data-stu-id="09a4a-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="09a4a-166">Office 365 E3-tila uksen määritykset ja tiedot</span><span class="sxs-lookup"><span data-stu-id="09a4a-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="09a4a-167">Sinun ei tarvitse tehdä muutoksia nykyiseen tilaukseesi tai tiedoihisi ennen siirtoa, joka sisältää seuraavat tiedot:</span><span class="sxs-lookup"><span data-stu-id="09a4a-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="09a4a-168">Tila uksen määritykset, kuten DNS-tietueet ja toimi alue nimet.</span><span class="sxs-lookup"><span data-stu-id="09a4a-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="09a4a-169">Käyttäjä-ja ryhmä tunnukset sekä todennus asetukset, kuten usean tekijän todentaminen tai ehdolliset käyttö oikeus käytännöt.</span><span class="sxs-lookup"><span data-stu-id="09a4a-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="09a4a-170">Tuottavuus palvelu määritykset ja niiden tiedot, kuten tiimit, Exchange Online-posti laatikot, SharePoint Online-sivustot, OneDrive for Business-kansiot ja OneNote-muisti kirjat.</span><span class="sxs-lookup"><span data-stu-id="09a4a-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="09a4a-171">Office-sovellukset skaalautuvat automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="09a4a-171">Office applications will scale automatically.</span></span> <span data-ttu-id="09a4a-172">Office 365 Modern Licensing tarkistaa käyttäjän käyttö oikeus Varauksen 72 tunnin välein ja muuntaa Office-sovellukset käyttäjän tilausta vastaavaksi versioksi.</span><span class="sxs-lookup"><span data-stu-id="09a4a-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="09a4a-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="09a4a-173">Windows 10</span></span>

<span data-ttu-id="09a4a-174">Jos Windows ei ole vielä Windows Pro Creator-päivityksessä, [Päivitä ne Windows Pro Creators](upgrade-to-windows-pro-creators-update.md)-päivitykseen.</span><span class="sxs-lookup"><span data-stu-id="09a4a-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="09a4a-175">Käytäntöjen määrittäminen käyttäjien laitteiden ja tiedostojen suojaamiseksi</span><span class="sxs-lookup"><span data-stu-id="09a4a-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="09a4a-176">Jos määrität Office 365 MDM-käytännöt ja-laitteet, kyseiset laitteet näkyvät Microsoft 365-hallinta keskuksen **laitteet** -sivulla.</span><span class="sxs-lookup"><span data-stu-id="09a4a-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="09a4a-177">Määrittämäsi käytännöt näkyvät perinteisten käytäntöjen luettelossa [Intune-portaalissa](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span><span class="sxs-lookup"><span data-stu-id="09a4a-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="09a4a-178">Kun olet määrittänyt käyttö oikeudet Microsoft 365 Business Premiumiin, voit aloittaa käyttäjien laitteiden ja tiedostojen suojaamisen.</span><span class="sxs-lookup"><span data-stu-id="09a4a-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="09a4a-179">Jos olet päivittänyt kaikki organisaatiosi käyttäjät Microsoft 365 Business Premiumiin, näet ohjatun määritys toiminnon aloitus sivulla ja voit suojata tiedostot ja mobiililaitteet noudattamalla [ohjattua määritys toimintoa microsoft 365 Business Premiumin määrittäminen](set-up.md) .</span><span class="sxs-lookup"><span data-stu-id="09a4a-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="09a4a-180">Voit suorittaa nämä vaiheet myös laitteet-sivulla:</span><span class="sxs-lookup"><span data-stu-id="09a4a-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="09a4a-181">Valitse hallinta keskuksen vasemmanpuoleisesta siirtymis ruudusta **laitteet** - \> **käytännöt**.</span><span class="sxs-lookup"><span data-stu-id="09a4a-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="09a4a-182">Valitse **laite käytännöt** -sivulla **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="09a4a-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="09a4a-183">Anna käytännölle nimi **Lisää käytäntöä** -ruudussa ja valitse sitten avattavasta luettelosta haluamasi **käytäntöjen tyyppi** .</span><span class="sxs-lookup"><span data-stu-id="09a4a-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="09a4a-184">Voit määrittää sovellus käytäntöjä, jotka suojaavat tiedostoja Android-ja iPhone-laitteissa sekä Windows 10: ssä, ja voit määrittää laitteiden määritys käytäntöjä yrityksen omistamille Windows 10-laitteille.</span><span class="sxs-lookup"><span data-stu-id="09a4a-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="09a4a-185">Lisä tietoja on seuraavissa linkeissä:</span><span class="sxs-lookup"><span data-stu-id="09a4a-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="09a4a-186">Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten</span><span class="sxs-lookup"><span data-stu-id="09a4a-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="09a4a-187">Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille</span><span class="sxs-lookup"><span data-stu-id="09a4a-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="09a4a-188">Laitteen suojaus asetusten määrittäminen Windows 10-tieto koneisiin</span><span class="sxs-lookup"><span data-stu-id="09a4a-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="09a4a-189">Kun olet määrittänyt käytännöt, sinä ja työn tekijäsi voitte määrittää laitteita:</span><span class="sxs-lookup"><span data-stu-id="09a4a-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="09a4a-190">Lisä tietoja on artikkelissa [Windows-laitteiden määrittäminen Microsoft 365 Business Premium-käyttäjille](set-up-windows-devices.md) Windows-laitteille.</span><span class="sxs-lookup"><span data-stu-id="09a4a-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="09a4a-191">Lisä tietoja on artikkelissa [mobiililaitteiden määrittäminen Microsoft 365 Business Premium-käyttäjille](set-up-mobile-devices.md) Android-puhelimiin ja iPhoneja koskevia ohjeita varten.</span><span class="sxs-lookup"><span data-stu-id="09a4a-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="09a4a-192">Posti laatikon koko</span><span class="sxs-lookup"><span data-stu-id="09a4a-192">Mailbox Size</span></span>

<span data-ttu-id="09a4a-193">Microsoft 365 Business Premiumin tallennus tila rajoitus on 50 gt, kun se käyttää Exchange Online-palvelu paketin 1.</span><span class="sxs-lookup"><span data-stu-id="09a4a-193">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="09a4a-194">Vaikka Microsoft 365 Business Premiumiin siirryttäessä käyttäjät ylittäisivät 50 Giga tavua posti laatikon tallennus tilaa, on suositeltavaa, että määrität tämän käyttäjän Exchange Online-palvelu paketin 2 ja poistat Exchange Online-palvelu paketin 1, koska molempien määrittäminen ei ole mahdollista.</span><span class="sxs-lookup"><span data-stu-id="09a4a-194">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>


### <a name="threat-protection"></a><span data-ttu-id="09a4a-195">Uhkien suojaus</span><span class="sxs-lookup"><span data-stu-id="09a4a-195">Threat protection</span></span>

<span data-ttu-id="09a4a-196">Kun olet muuttanut Microsoft 365 Business Premiumiin, sinulla on Office 365 Defender.</span><span class="sxs-lookup"><span data-stu-id="09a4a-196">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="09a4a-197">Katso yleiskuvaus artikkelista [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) .</span><span class="sxs-lookup"><span data-stu-id="09a4a-197">See [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for an overview.</span></span> <span data-ttu-id="09a4a-198">Lisä tietoja on kohdassa [turvallisten linkkien](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)määrittäminen, [turvallisten liitteiden](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)määrittäminen ja [Tietojenkalastelutietojen määrittäminen Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)-sovelluksessa.</span><span class="sxs-lookup"><span data-stu-id="09a4a-198">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="09a4a-199">Luottamuksellisuusmerkinnät</span><span class="sxs-lookup"><span data-stu-id="09a4a-199">Sensitivity labels</span></span>

<span data-ttu-id="09a4a-200">Jos haluat käyttää herkkyys otsikoita, katso [Yleiskatsaus herkkyys merkinnöistä](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) ja [Luo ja hallitse herkkyys otsikoita](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) -video.</span><span class="sxs-lookup"><span data-stu-id="09a4a-200">To start using sensitivity labels, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>
