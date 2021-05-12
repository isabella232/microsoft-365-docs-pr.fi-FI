---
title: Siirtyminen Microsoft 365 Business E3 Office 365 stä
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
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
description: Opi siirtämään yrityksesi Microsoft 365 Business Premium E3 Office 365 stä.
ms.openlocfilehash: 990ca8bdae979f1efb8a60a3460add2953a51892
ms.sourcegitcommit: 68383240ef7a673d5f28e2ecfab9f105bf1d8c8f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/11/2021
ms.locfileid: "52327166"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="383d2-103">Siirtyminen Office 365 E3:sta Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="383d2-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span>

<span data-ttu-id="383d2-104">Microsoft 365 Business Premium sisältää kaiken pienyritystäsi varten yhdistämällä luokkansa parhaat pilvipohjaiset tuottavuussovellukset yksinkertaiseen laitehallintaan ja tietoturvaan.</span><span class="sxs-lookup"><span data-stu-id="383d2-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="383d2-105">Jos sinulla on Office 365 E3 -tilaus, mutta yrityksessä on enintään 300 työntekijää, harkitse siirtymistä Microsoft 365 Business Premium suojausominaisuuksia varten.</span><span class="sxs-lookup"><span data-stu-id="383d2-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="383d2-106">Siirtyminen on helppoa: Ensin vaihdat käyttöoikeuksia, ja kaikki nykyisen tilauksesi tiedot ja käyttäjätiedot säilytetään.</span><span class="sxs-lookup"><span data-stu-id="383d2-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="383d2-107">Siirron jälkeen sinun on määritettävä toiminnot, jotka lisätään Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="383d2-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="383d2-108">E3-Office 365 ja Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="383d2-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="383d2-109">Tässä taulukossa esitetään E3 Microsoft 365 Business Premium ja Office 365 väliset erot.</span><span class="sxs-lookup"><span data-stu-id="383d2-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="383d2-110">Ominaisuus</span><span class="sxs-lookup"><span data-stu-id="383d2-110">Feature</span></span>    | <span data-ttu-id="383d2-111">Tuki Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="383d2-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="383d2-112">Tuki Office 365 E3:ssa</span><span class="sxs-lookup"><span data-stu-id="383d2-112">Support in Office 365 E3</span></span> |
|:-------|:-----|:-----|
| <span data-ttu-id="383d2-113">**Paikallinen**</span><span class="sxs-lookup"><span data-stu-id="383d2-113">**On-premises**</span></span>        | | |
| <span data-ttu-id="383d2-114">Office sovellukset<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="383d2-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="383d2-115">Microsoft 365 -sovellukset yrityksille</span><span class="sxs-lookup"><span data-stu-id="383d2-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="383d2-116">Microsoft 365 -sovellukset yrityksille</span><span class="sxs-lookup"><span data-stu-id="383d2-116">Microsoft 365 Apps for enterprise</span></span> |
| <span data-ttu-id="383d2-117">**Pilvitallennussovellukset**</span><span class="sxs-lookup"><span data-stu-id="383d2-117">**Cloud productivity apps**</span></span>        | | |
| <span data-ttu-id="383d2-118">Exchange Online ja Outlook</span><span class="sxs-lookup"><span data-stu-id="383d2-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="383d2-119">Postilaatikkokohtainen 50 gigatavun tallennustilaraja ja rajoittamaton Exchange Online Archiving</span><span class="sxs-lookup"><span data-stu-id="383d2-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="383d2-120">100 Gigatavun tallennustilaraja postilaatikkoa kohden ja rajoittamaton Exchange Online Archiving</span><span class="sxs-lookup"><span data-stu-id="383d2-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> |
| <span data-ttu-id="383d2-121">Teams</span><span class="sxs-lookup"><span data-stu-id="383d2-121">Teams</span></span>    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Office 365 E3:lle](../media/check-mark.png) | 
| <span data-ttu-id="383d2-124">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="383d2-124">OneDrive for Business</span></span>    | <span data-ttu-id="383d2-125">1 Tt tallennustilaraja käyttäjää kohden</span><span class="sxs-lookup"><span data-stu-id="383d2-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="383d2-126">Rajoittamaton</span><span class="sxs-lookup"><span data-stu-id="383d2-126">Unlimited</span></span> | 
| <span data-ttu-id="383d2-127">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="383d2-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Office 365 E3:lle](../media/check-mark.png) | 
| <span data-ttu-id="383d2-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="383d2-130">StaffHub</span></span>    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Office 365 E3:lle](../media/check-mark.png) |
| <span data-ttu-id="383d2-133">**Threat Protection**</span><span class="sxs-lookup"><span data-stu-id="383d2-133">**Threat Protection**</span></span>        | | |
| <span data-ttu-id="383d2-134">Defender for Office 365 Plan 1</span><span class="sxs-lookup"><span data-stu-id="383d2-134">Defender for Office 365 Plan 1</span></span> | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="383d2-136">Ei sisälly, mutta voidaan lisätä</span><span class="sxs-lookup"><span data-stu-id="383d2-136">Not included, but can be added on</span></span> |
| <span data-ttu-id="383d2-137">**Käyttäjätietojen hallinta**</span><span class="sxs-lookup"><span data-stu-id="383d2-137">**Identity management**</span></span>        | | |
| <span data-ttu-id="383d2-138">Omatoiminen salasanan vaihtaminen yhdistelmäympäristön Azure Active Directory (Azure AD) -tileissä, Azure AD:n monimenetelmäinen todentaminen (MFA), ehdollinen käyttöoikeus, paikallisen käyttäjätiedot salasanalla kirjoittamisen palautus</span><span class="sxs-lookup"><span data-stu-id="383d2-138">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="383d2-140">**Laite- ja sovellushallinta**</span><span class="sxs-lookup"><span data-stu-id="383d2-140">**Device and app management**</span></span>        | | |
| <span data-ttu-id="383d2-141">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="383d2-141">Microsoft Intune, Windows AutoPilot</span></span>|     ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="383d2-143">Jaetun tietokoneen aktivointi</span><span class="sxs-lookup"><span data-stu-id="383d2-143">Shared computer activation</span></span>|     ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Office 365 E3:lle](../media/check-mark.png)| 
| <span data-ttu-id="383d2-146">Päivitä käyttöoikeudet Windows 10 Pro Win 7/8.1 -Pro käyttöoikeuksista</span><span class="sxs-lookup"><span data-stu-id="383d2-146">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    ||
| <span data-ttu-id="383d2-148">**Tietojen suojaus**</span><span class="sxs-lookup"><span data-stu-id="383d2-148">**Information protection**</span></span>        | | |
|<span data-ttu-id="383d2-149">Office 365 Tietojen menetyksen estäminen</span><span class="sxs-lookup"><span data-stu-id="383d2-149">Office 365 Data Loss Prevention</span></span>|    ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)|![Sisältyy Office 365 E3:lle](../media/check-mark.png)|
|<span data-ttu-id="383d2-152">Azure Information Protection Plan 1, BitLocker pakotus</span><span class="sxs-lookup"><span data-stu-id="383d2-152">Azure Information Protection Plan 1, BitLocker enforcement</span></span>|![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="383d2-154">Azure Information Protection Plan 1, luottamuksellisuusmerkinnät</span><span class="sxs-lookup"><span data-stu-id="383d2-154">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="383d2-156">**Client Access License (CAL-oikeudet)**</span><span class="sxs-lookup"><span data-stu-id="383d2-156">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="383d2-157">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="383d2-157">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Sisältyy Office 365 E3:lle](../media/check-mark.png)|

<span data-ttu-id="383d2-159"><sup>1</sup> Microsoft 365 Business Premium-sovellusten Office ei sisällä volyymiaktivoinnin ryhmäkäytännön, sovelluksen telemetriatietojen, päivitysohjausobjektien, laskentataulukon vertailun ja kyselyn tai liiketoimintatietojen kautta.</span><span class="sxs-lookup"><span data-stu-id="383d2-159"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="383d2-160">Siirto</span><span class="sxs-lookup"><span data-stu-id="383d2-160">Migration</span></span>

<span data-ttu-id="383d2-161">Jos haluat siirtää tilauksen, katso ohjeet [tilauksen](../commerce/subscriptions/change-plans-manually.md) manuaaliseen Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="383d2-161">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="383d2-162">Voit myös päivittää [kaikki automaattisesti tai](../commerce/subscriptions/upgrade-to-different-plan.md)siirtää E3-tilauksesi ja -käyttöoikeutesi kumppanin kanssa Microsoft 365 Business Premium tilaukseen.</span><span class="sxs-lookup"><span data-stu-id="383d2-162">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="383d2-163">Seuraavissa osissa kuvataan, mitä muutoksia on tehtävä (jos niitä on) ja mitä voit tehdä siirron jälkeen.</span><span class="sxs-lookup"><span data-stu-id="383d2-163">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="383d2-164">Office 365 E3-tilauksen määritykset ja tiedot</span><span class="sxs-lookup"><span data-stu-id="383d2-164">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="383d2-165">Sinun ei tarvitse tehdä muutoksia nykyiseen tilaukseesi tai tietoihin ennen sen muutosta, joka sisältää seuraavat:</span><span class="sxs-lookup"><span data-stu-id="383d2-165">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="383d2-166">Tilausmääritykset, kuten DNS-tietueet ja toimialuenimet.</span><span class="sxs-lookup"><span data-stu-id="383d2-166">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="383d2-167">Käyttäjä- ja ryhmätilit ja todentamisasetukset, kuten monimenetelmäinen todentaminen tai ehdolliset käyttöoikeuskäytännöt.</span><span class="sxs-lookup"><span data-stu-id="383d2-167">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="383d2-168">Tuottavuuspalvelun määritykset ja niiden tiedot, kuten Teams, Exchange Online postilaatikot, SharePoint online-sivustot, OneDrive for Business kansiot OneNote muistikirjat.</span><span class="sxs-lookup"><span data-stu-id="383d2-168">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="383d2-169">Office skaalataan automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="383d2-169">Office applications will scale automatically.</span></span> <span data-ttu-id="383d2-170">Office 365 modernit käyttöoikeudet tarkistavat käyttäjän käyttöoikeusmäärityksen 72 tunnin välein ja muuntaa Office-sovellukset käyttäjän tilausta vastaavaksi versioksi.</span><span class="sxs-lookup"><span data-stu-id="383d2-170">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="383d2-171">Windows 10</span><span class="sxs-lookup"><span data-stu-id="383d2-171">Windows 10</span></span>

<span data-ttu-id="383d2-172">Jos Windows ei ole vielä Windows Pro Creator -päivityksessä, päivitä ne Windows Pro [Creators -päivitykseen.](upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="383d2-172">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="383d2-173">Käyttäjien laitteiden ja tiedostojen suojaamista varten määritettyjen käytäntöjä</span><span class="sxs-lookup"><span data-stu-id="383d2-173">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="383d2-174">Jos määrität Office 365 mobiililaitteiden hallintakäytännöt ja -laitteet, kyseiset  laitteet näkyvät Microsoft 365 hallintakeskuksen Laitteet-sivulla.</span><span class="sxs-lookup"><span data-stu-id="383d2-174">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="383d2-175">Kaikki määrittämäsi käytännöt näkyvät Intune-portaalin perinteiset [käytännöt -luettelossa.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)</span><span class="sxs-lookup"><span data-stu-id="383d2-175">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="383d2-176">Kun olet määrittänyt käyttöoikeudet Microsoft 365 Business Premium, voit alkaa suojata käyttäjien laitteita ja tiedostoja.</span><span class="sxs-lookup"><span data-stu-id="383d2-176">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="383d2-177">Jos olet päivittänyt kaikki organisaation käyttäjät Microsoft 365 Business Premium, näet ohjatun määritystoiminnon aloitussivulla ja voit suojata tiedostoja ja mobiililaitteita ohjatun [Microsoft 365 Business Premium](set-up.md) määritystoiminnon määritysvaiheiden mukaisesti.</span><span class="sxs-lookup"><span data-stu-id="383d2-177">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="383d2-178">Voit myös suorittaa nämä vaiheet Laitteet-sivulla:</span><span class="sxs-lookup"><span data-stu-id="383d2-178">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="383d2-179">Valitse hallintakeskuksen vasemmassa siirtymispalkin **laitekäytännöt** \> .</span><span class="sxs-lookup"><span data-stu-id="383d2-179">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>

2. <span data-ttu-id="383d2-180">Valitse **Laitekäytännöt-sivulla** **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="383d2-180">On the **Device policies** page, choose **Add**.</span></span>

3. <span data-ttu-id="383d2-181">Anna **käytännön nimi** Lisää käytäntö -ruudussa ja valitse sitten **käytäntötyyppi** avattavasta luettelosta.</span><span class="sxs-lookup"><span data-stu-id="383d2-181">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span>

     <span data-ttu-id="383d2-182">Voit määrittää sovelluskäytäntöjä Android- ja iPhone-laitteissa sekä Windows 10-laitteissa olevien tiedostojen suojaamista varten sekä määrittää laitemäärityskäytännöt yrityksen omistamia Windows 10 laitteita varten.</span><span class="sxs-lookup"><span data-stu-id="383d2-182">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="383d2-183">Lisätietoja on seuraavissa linkeissä:</span><span class="sxs-lookup"><span data-stu-id="383d2-183">See the following links for details:</span></span>

  - [<span data-ttu-id="383d2-184">Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten</span><span class="sxs-lookup"><span data-stu-id="383d2-184">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)

  - [<span data-ttu-id="383d2-185">Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille</span><span class="sxs-lookup"><span data-stu-id="383d2-185">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)

  - [<span data-ttu-id="383d2-186">Laitteiden suojausasetusten määrittäminen Windows 10 tietokoneisiin</span><span class="sxs-lookup"><span data-stu-id="383d2-186">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="383d2-187">Kun olet määrittänyt käytännöt, sinä ja työntekijäsi voitte määrittää laitteita:</span><span class="sxs-lookup"><span data-stu-id="383d2-187">Once you set up policies, you and your employees can set up devices:</span></span>

  - <span data-ttu-id="383d2-188">Katso [ohjeet Windows laitteiden Microsoft 365 Business Premium käyttäjille](set-up-windows-devices.md) Windows varten.</span><span class="sxs-lookup"><span data-stu-id="383d2-188">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 

  - <span data-ttu-id="383d2-189">Katso [ohjeet Android-puhelimiin ja iPhoneen Microsoft 365 Business Premium](set-up-mobile-devices.md) mobiililaitteiden Microsoft 365 Business Premium mobiililaitteille.</span><span class="sxs-lookup"><span data-stu-id="383d2-189">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="383d2-190">Postilaatikon koko</span><span class="sxs-lookup"><span data-stu-id="383d2-190">Mailbox Size</span></span>

<span data-ttu-id="383d2-191">Microsoft 365 Business Premium tallennustilaraja on 50 gigatavua, sillä se käyttää Exchange Online 1:tä.</span><span class="sxs-lookup"><span data-stu-id="383d2-191">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="383d2-192">Kun siirto Microsoft 365 Business Premium:lle ja joku käyttäjistä ylittää 50 Gt postilaatikon tallennustilaa, on suositeltavaa määrittää tälle käyttäjälle Exchange Online -käyttöoikeuspaketti 2 ja poistaa Exchange Online -käyttöoikeuspaketti 1, koska molempia ei voi määrittää.</span><span class="sxs-lookup"><span data-stu-id="383d2-192">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>

### <a name="threat-protection"></a><span data-ttu-id="383d2-193">Uhkien suojaus</span><span class="sxs-lookup"><span data-stu-id="383d2-193">Threat protection</span></span>

<span data-ttu-id="383d2-194">Kun olet Microsoft 365 Business Premium, sinulla on Defender for Office 365.</span><span class="sxs-lookup"><span data-stu-id="383d2-194">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="383d2-195">Tutustu [yleiskatsaukseen Office 365 Microsoft Defender for](../security/office-365-security/defender-for-office-365.md) Office 365.</span><span class="sxs-lookup"><span data-stu-id="383d2-195">See [Microsoft Defender for Office 365](../security/office-365-security/defender-for-office-365.md) for an overview.</span></span> <span data-ttu-id="383d2-196">Lisätietoja on kohdassa Turvallisten linkkien [määritys](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), Turvallisten liitteiden määritys ja [Tietojenkalastelun](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5) [esto -määritys Defender for Office 365.](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)</span><span class="sxs-lookup"><span data-stu-id="383d2-196">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="383d2-197">Luottamuksellisuusmerkinnät</span><span class="sxs-lookup"><span data-stu-id="383d2-197">Sensitivity labels</span></span>

<span data-ttu-id="383d2-198">Jos haluat aloittaa luottamuksellisuusotsikoiden käytön, katso [Luottamuksellisuusotsikoiden yleiskatsaus](../compliance/sensitivity-labels.md) ja [luo ja hallitse luottamuksellisuusotsikoiden](../business-video/create-sensitivity-labels.md) videota.</span><span class="sxs-lookup"><span data-stu-id="383d2-198">To start using sensitivity labels, see [Overview of sensitivity labels](../compliance/sensitivity-labels.md) and [create and manage sensitivity labels](../business-video/create-sensitivity-labels.md) video.</span></span>
