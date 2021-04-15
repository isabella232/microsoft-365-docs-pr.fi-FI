---
title: Siirtyminen Microsoft 365 Businessiin Office 365 E3:sta
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
description: Opi siirtämään yrityksesi Microsoft 365 Business Premiumiin Office 365 E3:sta.
ms.openlocfilehash: f2b7962918186f4a1063c5a66596135c2972ec71
ms.sourcegitcommit: 07dea2aa98daf0c4086f8590375167830027c802
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/13/2021
ms.locfileid: "51749996"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="676be-103">Siirtyminen Office 365 E3:sta Microsoft 365 Business Premiumiin</span><span class="sxs-lookup"><span data-stu-id="676be-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span>

<span data-ttu-id="676be-104">Microsoft 365 Business Premium sisältää kaiken, mitä tarvitset pienyritystäsi varten yhdistämällä luokkansa parhaat pilvipohjaiset tuottavuussovellukset yksinkertaiseen laitehallintaan ja tietoturvaan.</span><span class="sxs-lookup"><span data-stu-id="676be-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="676be-105">Jos sinulla on tällä hetkellä Office 365 E3 -tilaus, mutta yrityksessäsi ei ole yli 300 työntekijää, voit siirtyä Microsoft 365 Business Premiumiin suojausominaisuuksien lisäominaisuuksia varten.</span><span class="sxs-lookup"><span data-stu-id="676be-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="676be-106">Siirtyminen on helppoa: Ensin vaihdat käyttöoikeuksia, ja kaikki nykyisen tilauksesi tiedot ja käyttäjätiedot säilytetään.</span><span class="sxs-lookup"><span data-stu-id="676be-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="676be-107">Siirron jälkeen sinun on määritettävä Microsoft 365 Business Premiumiin lisätyt ominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="676be-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="676be-108">Office 365 E3:n ja Microsoft 365 Business Premiumin erot</span><span class="sxs-lookup"><span data-stu-id="676be-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="676be-109">Tässä taulukossa on esitetty Microsoft 365 Business Premiumin ja Office 365 E3:n väliset erot.</span><span class="sxs-lookup"><span data-stu-id="676be-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="676be-110">Ominaisuus</span><span class="sxs-lookup"><span data-stu-id="676be-110">Feature</span></span>    | <span data-ttu-id="676be-111">Microsoft 365 Business Premiumin tuki</span><span class="sxs-lookup"><span data-stu-id="676be-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="676be-112">Tuki Office 365 E3:ssa</span><span class="sxs-lookup"><span data-stu-id="676be-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="676be-113">**Paikallinen**</span><span class="sxs-lookup"><span data-stu-id="676be-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="676be-114">Office-sovellukset<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="676be-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="676be-115">Microsoft 365 -sovellukset yrityksille</span><span class="sxs-lookup"><span data-stu-id="676be-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="676be-116">Microsoft 365 -sovellukset yrityksille</span><span class="sxs-lookup"><span data-stu-id="676be-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="676be-117">**Pilvitallennussovellukset**</span><span class="sxs-lookup"><span data-stu-id="676be-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="676be-118">Exchange Online ja Outlook</span><span class="sxs-lookup"><span data-stu-id="676be-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="676be-119">50 gigatavun tallennustilaraja postilaatikkoa kohden ja rajoittamaton Exchange Online Archiving</span><span class="sxs-lookup"><span data-stu-id="676be-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="676be-120">100 Gigatavun tallennustilaraja postilaatikkoa kohden ja rajoittamaton Exchange Online Archiving</span><span class="sxs-lookup"><span data-stu-id="676be-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="676be-121">Teams</span><span class="sxs-lookup"><span data-stu-id="676be-121">Teams</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:lle](../media/check-mark.png) | 
| <span data-ttu-id="676be-124">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="676be-124">OneDrive for Business</span></span>    | <span data-ttu-id="676be-125">1 Tt tallennustilaraja käyttäjää kohden</span><span class="sxs-lookup"><span data-stu-id="676be-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="676be-126">Rajoittamaton</span><span class="sxs-lookup"><span data-stu-id="676be-126">Unlimited</span></span> | 
| <span data-ttu-id="676be-127">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="676be-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:lle](../media/check-mark.png) | 
| <span data-ttu-id="676be-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="676be-130">StaffHub</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:lle](../media/check-mark.png) | 
| <span data-ttu-id="676be-133">MileIQ</span><span class="sxs-lookup"><span data-stu-id="676be-133">MileIQ</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | | 
| <span data-ttu-id="676be-135">**Threat Protection**</span><span class="sxs-lookup"><span data-stu-id="676be-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="676be-136">Defender for Office 365 Plan 1</span><span class="sxs-lookup"><span data-stu-id="676be-136">Defender for Office 365 Plan 1</span></span> | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | <span data-ttu-id="676be-138">Ei sisälly, mutta voidaan lisätä</span><span class="sxs-lookup"><span data-stu-id="676be-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="676be-139">**Käyttäjätietojen hallinta**</span><span class="sxs-lookup"><span data-stu-id="676be-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="676be-140">Azure Active Directory (Azure AD) -yhdistelmätilien omatoiminen salasanan palautus, Azure AD:n monimenetelmäinen todentaminen (MFA), ehdollinen käyttöoikeus, paikallisen käyttäjätiedot salasanalla kirjoitettavan salasanan palautus</span><span class="sxs-lookup"><span data-stu-id="676be-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    |  | 
| <span data-ttu-id="676be-142">**Laite- ja sovellushallinta**</span><span class="sxs-lookup"><span data-stu-id="676be-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="676be-143">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="676be-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    |  |
| <span data-ttu-id="676be-145">Jaetun tietokoneen aktivointi</span><span class="sxs-lookup"><span data-stu-id="676be-145">Shared computer activation</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:lle](../media/check-mark.png)| 
| <span data-ttu-id="676be-148">Oikeuksien päivittäminen Windows 10 Pro -käyttöoikeuteen Win 7/8.1 Pro -käyttöoikeuksista</span><span class="sxs-lookup"><span data-stu-id="676be-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    || 
| <span data-ttu-id="676be-150">**Tietojen suojaus**</span><span class="sxs-lookup"><span data-stu-id="676be-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="676be-151">Office 365:n tietojen menetyksen estäminen</span><span class="sxs-lookup"><span data-stu-id="676be-151">Office 365 Data Loss Prevention</span></span>|    ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)|![Sisältyy Office 365 E3:lle](../media/check-mark.png)|
|<span data-ttu-id="676be-154">Azure Information Protection Plan 1, BitLocker-pakotus</span><span class="sxs-lookup"><span data-stu-id="676be-154">Azure Information Protection Plan 1, BitLocker enforcement</span></span>|![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)||
|<span data-ttu-id="676be-156">Azure Information Protection Plan 1, luottamuksellisuusmerkinnät</span><span class="sxs-lookup"><span data-stu-id="676be-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)||
|<span data-ttu-id="676be-158">**Client Access License (CAL-oikeudet)**</span><span class="sxs-lookup"><span data-stu-id="676be-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="676be-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="676be-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Sisältyy Office 365 E3:lle](../media/check-mark.png)|

<span data-ttu-id="676be-161"><sup>1</sup> Office-sovellusten Microsoft 365 Business Premium -versio ei sisällä volyymiaktivoinnin ryhmäkäytännön, sovellustelemetrian, päivitysohjausobjektien, laskentataulukon vertailun ja kyselyn tai liiketoimintatietojen kautta.</span><span class="sxs-lookup"><span data-stu-id="676be-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="676be-162">Siirto</span><span class="sxs-lookup"><span data-stu-id="676be-162">Migration</span></span>

<span data-ttu-id="676be-163">Jos haluat siirtää tilauksesi, [katso](../commerce/subscriptions/change-plans-manually.md) ohjeet palvelupaketit manuaalisesti, jos haluat siirtää vain muutamia henkilöitä Microsoft 365 Business Premiumiin.</span><span class="sxs-lookup"><span data-stu-id="676be-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="676be-164">Voit myös päivittää [kaikki automaattisesti tai](../commerce/subscriptions/upgrade-to-different-plan.md)siirtää E3-tilauksesi ja -käyttöoikeutesi Microsoft 365 Business Premium -tilaukseen kumppanin kanssa.</span><span class="sxs-lookup"><span data-stu-id="676be-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="676be-165">Seuraavissa osissa kuvataan, mitä muutoksia on tehtävä (jos niitä on) ja mitä voit tehdä siirron jälkeen.</span><span class="sxs-lookup"><span data-stu-id="676be-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="676be-166">Office 365 E3 -tilauksen määritys ja tiedot</span><span class="sxs-lookup"><span data-stu-id="676be-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="676be-167">Sinun ei tarvitse tehdä muutoksia nykyiseen tilaukseesi tai tietoihin ennen sen muutosta, joka sisältää seuraavat:</span><span class="sxs-lookup"><span data-stu-id="676be-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="676be-168">Tilausmääritykset, kuten DNS-tietueet ja toimialuenimet.</span><span class="sxs-lookup"><span data-stu-id="676be-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="676be-169">Käyttäjä- ja ryhmätilit ja todentamisasetukset, kuten monimenetelmäinen todentaminen tai ehdolliset käyttöoikeuskäytännöt.</span><span class="sxs-lookup"><span data-stu-id="676be-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="676be-170">Tuottavuuspalvelun määritykset ja niiden tiedot, kuten Teams, Exchange Online -postilaatikot, SharePoint Online -sivustot, OneDrive for Business -kansiot ja OneNote-muistikirjat.</span><span class="sxs-lookup"><span data-stu-id="676be-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="676be-171">Office-sovellukset skaalataan automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="676be-171">Office applications will scale automatically.</span></span> <span data-ttu-id="676be-172">Office 365:n modernit käyttöoikeudet tarkistavat käyttäjän käyttöoikeusmäärityksen 72 tunnin välein ja muuntaa Office-sovellukset käyttäjän tilausta vastaavaksi versioksi.</span><span class="sxs-lookup"><span data-stu-id="676be-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="676be-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="676be-173">Windows 10</span></span>

<span data-ttu-id="676be-174">Jos Windows ei ole vielä Windows Pro Creator -päivityksessä, [päivitä ne Windows Pro Creators -päivitykseen.](upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="676be-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="676be-175">Käyttäjien laitteiden ja tiedostojen suojaamista varten määritettyjen käytäntöjä</span><span class="sxs-lookup"><span data-stu-id="676be-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="676be-176">Jos määrität Office 365:n mobiililaitteiden hallintakäytännöt ja  -laitteet, kyseiset laitteet näkyvät Laitteet-sivulla Microsoft 365 -hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="676be-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="676be-177">Kaikki määrittämäsi käytännöt näkyvät Intune-portaalin perinteiset [käytännöt -luettelossa.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)</span><span class="sxs-lookup"><span data-stu-id="676be-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="676be-178">Kun olet määrittänyt käyttöoikeudet Microsoft 365 Business Premiumiin, voit alkaa suojata käyttäjien laitteita ja tiedostoja.</span><span class="sxs-lookup"><span data-stu-id="676be-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="676be-179">Jos olet päivittänyt kaikki organisaation käyttäjät Microsoft 365 Business Premiumiin, näet ohjatun määritystoiminnon aloitussivulla ja voit suojata tiedostoja ja mobiililaitteita ohjatun määritystoiminnon ohjeiden mukaisesti Microsoft [365 Business Premiumin](set-up.md) määrittäminen.</span><span class="sxs-lookup"><span data-stu-id="676be-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="676be-180">Voit myös suorittaa nämä vaiheet Laitteet-sivulla:</span><span class="sxs-lookup"><span data-stu-id="676be-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="676be-181">Valitse hallintakeskuksen vasemmassa siirtymispalkin **laitekäytännöt** \> .</span><span class="sxs-lookup"><span data-stu-id="676be-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="676be-182">Valitse **Laitekäytännöt-sivulla** **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="676be-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="676be-183">Anna **käytännön nimi** Lisää käytäntö -ruudussa ja valitse sitten **käytäntötyyppi** avattavasta luettelosta.</span><span class="sxs-lookup"><span data-stu-id="676be-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="676be-184">Voit määrittää sovelluskäytäntöjä Android- ja iPhone-laitteiden sekä Windows 10:n tiedostojen suojaamista varten ja määrittää laitemäärityskäytännöt yrityksen omistamia Windows 10 -laitteita varten.</span><span class="sxs-lookup"><span data-stu-id="676be-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="676be-185">Lisätietoja on seuraavissa linkeissä:</span><span class="sxs-lookup"><span data-stu-id="676be-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="676be-186">Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten</span><span class="sxs-lookup"><span data-stu-id="676be-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="676be-187">Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille</span><span class="sxs-lookup"><span data-stu-id="676be-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="676be-188">Laitteiden suojausasetusten määrittäminen Windows 10 -tietokoneille</span><span class="sxs-lookup"><span data-stu-id="676be-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="676be-189">Kun olet määrittänyt käytännöt, sinä ja työntekijäsi voitte määrittää laitteita:</span><span class="sxs-lookup"><span data-stu-id="676be-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="676be-190">Ohjeet [Windows-laitteille ovat kohdassa Windows-laitteiden asennus Microsoft 365 Business Premium](set-up-windows-devices.md) -käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="676be-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="676be-191">Ohjeita [Android-puhelimiin ja iPhone-puhelimiin](set-up-mobile-devices.md) on kohdassa Mobiililaitteiden määritäminen Microsoft 365 Business Premium -käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="676be-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="676be-192">Postilaatikon koko</span><span class="sxs-lookup"><span data-stu-id="676be-192">Mailbox Size</span></span>

<span data-ttu-id="676be-193">Microsoft 365 Business Premiumin tallennustilaraja on 50 gigatavua, sillä se käyttää Exchange Online -palvelupakettia 1.</span><span class="sxs-lookup"><span data-stu-id="676be-193">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="676be-194">Kun siirto Microsoft 365 Business Premiumiin on suositeltavaa, että joku käyttäjistä ylittää 50 Gt postilaatikon tallennustilaa, on suositeltavaa määrittää käyttäjälle Exchange Online -palvelupaketti 2 ja poistaa Exchange Online -palvelupaketti 1, koska molempia ei voi määrittää.</span><span class="sxs-lookup"><span data-stu-id="676be-194">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>


### <a name="threat-protection"></a><span data-ttu-id="676be-195">Uhkien suojaus</span><span class="sxs-lookup"><span data-stu-id="676be-195">Threat protection</span></span>

<span data-ttu-id="676be-196">Kun olet siirtyminen Microsoft 365 Business Premiumiin, sinulla on Defender for Office 365.</span><span class="sxs-lookup"><span data-stu-id="676be-196">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="676be-197">Tutustu [yleiskatsaukseen microsoft Defender for Office 365:ssä.](../security/office-365-security/defender-for-office-365.md)</span><span class="sxs-lookup"><span data-stu-id="676be-197">See [Microsoft Defender for Office 365](../security/office-365-security/defender-for-office-365.md) for an overview.</span></span> <span data-ttu-id="676be-198">Lisätietoja on kohdassa [Turvallisten](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)linkkien määritys , Turvallisten liitteiden määritys ja [Tietojenkalastelun](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)esto -määritys [Office 365:n Defenderissä.](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)</span><span class="sxs-lookup"><span data-stu-id="676be-198">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="676be-199">Luottamuksellisuusmerkinnät</span><span class="sxs-lookup"><span data-stu-id="676be-199">Sensitivity labels</span></span>

<span data-ttu-id="676be-200">Jos haluat aloittaa luottamuksellisuusotsikoiden käytön, katso [Luottamuksellisuusotsikoiden yleiskatsaus](../compliance/sensitivity-labels.md) ja [luo ja hallitse luottamuksellisuusotsikoiden](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) videota.</span><span class="sxs-lookup"><span data-stu-id="676be-200">To start using sensitivity labels, see [Overview of sensitivity labels](../compliance/sensitivity-labels.md) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>
