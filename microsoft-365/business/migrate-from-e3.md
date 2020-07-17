---
title: Siirtyminen Microsoft 365 Businessiin Office 365 E3:sta
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
description: Lue tietoja siitä, miten voit siirtää yrityksesi Microsoft 365 Business Premiumiin Office 365 E3:sta.
ms.openlocfilehash: d72f0c52a745ff973868b6fdaa95efa1a37a3dbd
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/18/2020
ms.locfileid: "45081812"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="a60af-103">Siirtyminen Office 365 E3:sta Microsoft 365 Business Premiumiin</span><span class="sxs-lookup"><span data-stu-id="a60af-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span> 

<span data-ttu-id="a60af-104">Microsoft 365 Business Premiumissa on kaikki mitä tarvitset pienyrityksellesi, ja siinä yhdistyvät luokkansa parhaat pilvipohjaiset tuottavuussovellukset sekä yksinkertainen laitehallinta ja -suojaus.</span><span class="sxs-lookup"><span data-stu-id="a60af-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="a60af-105">Jos sinulla on tällä hetkellä Office 365 E3 -tilaus, mutta sinulla ei ole enempää kuin 300 työntekijää, harkitse siirtymistä Microsoft 365 Business Premiumiin lisäsuojausominaisuuksien saamiseksi.</span><span class="sxs-lookup"><span data-stu-id="a60af-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="a60af-106">Siirtäminen on helppoa: Ensin vaihdat käyttöoikeuksia ja kaikki nykyisen tilauksesi tiedot ja käyttäjätiedot säilytetään.</span><span class="sxs-lookup"><span data-stu-id="a60af-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="a60af-107">Siirron jälkeen sinun on määritettävä Microsoft 365 Business Premiumiin lisätyt ominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="a60af-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="a60af-108">Erot Office 365 E3:n ja Microsoft 365 Business Premiumin välillä</span><span class="sxs-lookup"><span data-stu-id="a60af-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="a60af-109">Tässä taulukossa esitetään Microsoft 365 Business Premiumin ja Office 365 E3:n väliset erot.</span><span class="sxs-lookup"><span data-stu-id="a60af-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="a60af-110">Ominaisuus</span><span class="sxs-lookup"><span data-stu-id="a60af-110">Feature</span></span>    | <span data-ttu-id="a60af-111">Microsoft 365 Business Premiumin tuki</span><span class="sxs-lookup"><span data-stu-id="a60af-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="a60af-112">Office 365 E3:n tuki</span><span class="sxs-lookup"><span data-stu-id="a60af-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="a60af-113">**Paikallinen**</span><span class="sxs-lookup"><span data-stu-id="a60af-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="a60af-114">Office-sovellukset<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="a60af-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="a60af-115">Microsoft 365 -sovellukset yrityksille</span><span class="sxs-lookup"><span data-stu-id="a60af-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="a60af-116">Microsoft 365 -sovellukset yrityksille</span><span class="sxs-lookup"><span data-stu-id="a60af-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="a60af-117">**Pilvituottavuussovellukset**</span><span class="sxs-lookup"><span data-stu-id="a60af-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="a60af-118">Exchange Online ja Outlook</span><span class="sxs-lookup"><span data-stu-id="a60af-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="a60af-119">50 Gt:n tallennustilarajoitus postilaatikkoa kohden ja rajoittamaton Exchange Online -arkistointi</span><span class="sxs-lookup"><span data-stu-id="a60af-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="a60af-120">100 Gt:n tallennustilarajoitus postilaatikkoa kohden ja rajoittamaton Exchange Online -arkistointi</span><span class="sxs-lookup"><span data-stu-id="a60af-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="a60af-121">Joukkueet</span><span class="sxs-lookup"><span data-stu-id="a60af-121">Teams</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:een](../media/check-mark.png) | 
| <span data-ttu-id="a60af-124">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="a60af-124">OneDrive for Business</span></span>    | <span data-ttu-id="a60af-125">1 Tt:n tallennusraja käyttäjää kohden</span><span class="sxs-lookup"><span data-stu-id="a60af-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="a60af-126">Rajoittamaton</span><span class="sxs-lookup"><span data-stu-id="a60af-126">Unlimited</span></span> | 
| <span data-ttu-id="a60af-127">Yammer, SharePoint Online, Suunnittelija, Stream</span><span class="sxs-lookup"><span data-stu-id="a60af-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:een](../media/check-mark.png) | 
| <span data-ttu-id="a60af-130">HenkilökuntaHub</span><span class="sxs-lookup"><span data-stu-id="a60af-130">StaffHub</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:een](../media/check-mark.png) | 
| <span data-ttu-id="a60af-133">Outlook-asiakaspäällikkö, MileIQ</span><span class="sxs-lookup"><span data-stu-id="a60af-133">Outlook Customer Manager, MileIQ</span></span>    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | | 
| <span data-ttu-id="a60af-135">**Uhkien torjunta**</span><span class="sxs-lookup"><span data-stu-id="a60af-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="a60af-136">Office 365 Advanced Threat Protection (ATP) -palvelupaketti 1</span><span class="sxs-lookup"><span data-stu-id="a60af-136">Office 365 Advanced Threat Protection (ATP) Plan 1</span></span> | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | <span data-ttu-id="a60af-138">Ei sisälly, mutta voidaan lisätä</span><span class="sxs-lookup"><span data-stu-id="a60af-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="a60af-139">**Identiteetin hallinta**</span><span class="sxs-lookup"><span data-stu-id="a60af-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="a60af-140">Azure Active Directory (Azure AD) -hybriditilien, Azure multi-factor-todennuksen (MFA), ehdollisen käytön, paikallisten käyttäjätietojen salasanan takaisinkutsun oletusasetusten palauttaminen</span><span class="sxs-lookup"><span data-stu-id="a60af-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    |  | 
| <span data-ttu-id="a60af-142">**Laite- ja sovellushallinta**</span><span class="sxs-lookup"><span data-stu-id="a60af-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="a60af-143">Microsoft Intune, Windowsin automaattiohjaus</span><span class="sxs-lookup"><span data-stu-id="a60af-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    |  |
| <span data-ttu-id="a60af-145">Jaetun tietokoneen aktivointi</span><span class="sxs-lookup"><span data-stu-id="a60af-145">Shared computer activation</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:een](../media/check-mark.png)| 
| <span data-ttu-id="a60af-148">Windows 10 Pron päivitysoikeudet Win 7/8.1 Pro -käyttöoikeuksista</span><span class="sxs-lookup"><span data-stu-id="a60af-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    || 
| <span data-ttu-id="a60af-150">**Tietojen suojaaminen**</span><span class="sxs-lookup"><span data-stu-id="a60af-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="a60af-151">Office 365:n tietojen menetyksen estäminen</span><span class="sxs-lookup"><span data-stu-id="a60af-151">Office 365 Data Loss Prevention</span></span>|    ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)|![Sisältyy Office 365 E3:een](../media/check-mark.png)|
|<span data-ttu-id="a60af-154">Azure Information Protection Plan 1, Bitlocker-valvonta</span><span class="sxs-lookup"><span data-stu-id="a60af-154">Azure Information Protection Plan 1, Bitlocker enforcement</span></span>|![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)||
|<span data-ttu-id="a60af-156">Azure Information Protection Plan 1, Herkkyysmerkinnät</span><span class="sxs-lookup"><span data-stu-id="a60af-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)||
|<span data-ttu-id="a60af-158">**Client Access License (CAL-käyttöoikeudet)**</span><span class="sxs-lookup"><span data-stu-id="a60af-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="a60af-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="a60af-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Sisältyy Office 365 E3:een](../media/check-mark.png)|

<span data-ttu-id="a60af-161"><sup>1</sup> Office-sovellusten Microsoft 365 Business Premium -versio ei sisällä volyymiaktivointia ryhmäkäytännön, sovellustelemetrian, päivitysohjausobjektien, laskentataulukoiden vertailun ja kyselyjen tai yritystietojen avulla.</span><span class="sxs-lookup"><span data-stu-id="a60af-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="a60af-162">Siirron</span><span class="sxs-lookup"><span data-stu-id="a60af-162">Migration</span></span>

<span data-ttu-id="a60af-163">Lisätietoja tilauksen siirtämisestä on [ohjeaiheessa Palvelupakettien muuttaminen manuaalisesti,](../commerce/subscriptions/change-plans-manually.md) jos haluat siirtää vain muutaman henkilön Microsoft 365 Business Premiumiin.</span><span class="sxs-lookup"><span data-stu-id="a60af-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="a60af-164">Voit myös [päivittää kaikki automaattisesti](../commerce/subscriptions/upgrade-to-different-plan.md)tai siirtää E3-tilauksesi ja -käyttöoikeutesi Microsoft 365 Business Premium -tilaukseen yhteistyössä kumppanin kanssa.</span><span class="sxs-lookup"><span data-stu-id="a60af-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="a60af-165">Seuraavissa osissa kuvataan muutokset, jotka sinun on tehtävä, jos sellaisia on, ja mitä voit tehdä siirron jälkeen.</span><span class="sxs-lookup"><span data-stu-id="a60af-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="a60af-166">Office 365 E3 -tilauksen määritys ja tiedot</span><span class="sxs-lookup"><span data-stu-id="a60af-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="a60af-167">Sinun ei tarvitse tehdä muutoksia nykyiseen tilaukseesi tai tietoihin ennen siirtämistä, joka sisältää:</span><span class="sxs-lookup"><span data-stu-id="a60af-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="a60af-168">Tilauksen määritykset, kuten DNS-tietueet ja toimialuenimet.</span><span class="sxs-lookup"><span data-stu-id="a60af-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="a60af-169">Käyttäjä- ja ryhmätilit ja todennusasetukset, kuten monivaiheinen todennus tai ehdollisen käytön käytännöt.</span><span class="sxs-lookup"><span data-stu-id="a60af-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="a60af-170">Tuottavuuspalvelun määritykset ja niiden tiedot, kuten Teams, Exchange Online -postilaatikot, SharePoint Online -sivustot, OneDrive for Business -kansiot ja OneNote-muistikirjat.</span><span class="sxs-lookup"><span data-stu-id="a60af-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="a60af-171">Office-sovellukset skaalautuvat automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="a60af-171">Office applications will scale automatically.</span></span> <span data-ttu-id="a60af-172">Office 365:n nykyaikaiset käyttöoikeudet tarkistavat käyttäjän käyttöoikeusmäärityksen 72 tunnin välein ja muuntavat Office-sovellukset käyttäjätilausta vastaavaksi versioksi.</span><span class="sxs-lookup"><span data-stu-id="a60af-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="a60af-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="a60af-173">Windows 10</span></span>

<span data-ttu-id="a60af-174">Jos Windows ei ole vielä Windows Pro Creator -päivityksessä, [päivitä ne Windows Pro Creators -päivitykseen](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="a60af-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="a60af-175">Käyttäjälaitteiden ja tiedostojen suojaaminen käytäntöjen määrittäminen</span><span class="sxs-lookup"><span data-stu-id="a60af-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="a60af-176">Jos määrität Office 365:n MDM-käytännöt ja -laitteet, nämä laitteet näkyvät Microsoft 365 -hallintakeskuksen **Laitteet-sivulla.**</span><span class="sxs-lookup"><span data-stu-id="a60af-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="a60af-177">Kaikki määrittämäsi käytännöt näkyvät [Intune-portaalin](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)klassisten käytäntöjen luettelossa.</span><span class="sxs-lookup"><span data-stu-id="a60af-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="a60af-178">Kun olet määrittänyt käyttöoikeudet Microsoft 365 Business Premiumiin, voit alkaa suojata käyttäjien laitteita ja tiedostoja.</span><span class="sxs-lookup"><span data-stu-id="a60af-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="a60af-179">Jos olet päivittänyt kaikki organisaation jäsenet Microsoft 365 Business Premiumiin, näet ohjatun asennustoiminnon kotisivulla ja voit suojata tiedostoja ja mobiililaitteita [noudattamalla Ohjatun asennustoiminnon ohjatun asennustoiminnon](set-up.md) määritystoimintoa.</span><span class="sxs-lookup"><span data-stu-id="a60af-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="a60af-180">Voit suorittaa nämä vaiheet myös Laitteet-sivulla:</span><span class="sxs-lookup"><span data-stu-id="a60af-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="a60af-181">Siirry hallintakeskuksen vasemmassa siirtymisruudussa **Devices** \> **Laitekäytännöt -kohtaan**.</span><span class="sxs-lookup"><span data-stu-id="a60af-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="a60af-182">Valitse **Laitekäytännöt-sivulla** **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="a60af-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="a60af-183">Anna **lisää käytäntö** -ruudussa käytännön nimi ja valitse sitten avattavasta valikosta **käytäntötyyppi.**</span><span class="sxs-lookup"><span data-stu-id="a60af-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="a60af-184">Voit määrittää sovelluskäytännöt tiedostojen suojaamiseksi Android- ja iPhone-laitteissa sekä Windows 10:ssä ja voit määrittää laitteen määrityskäytännöt yrityksen omistamille Windows 10 -laitteille.</span><span class="sxs-lookup"><span data-stu-id="a60af-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="a60af-185">Lisätietoja on seuraavissa linkeissä:</span><span class="sxs-lookup"><span data-stu-id="a60af-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="a60af-186">Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten</span><span class="sxs-lookup"><span data-stu-id="a60af-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="a60af-187">Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille</span><span class="sxs-lookup"><span data-stu-id="a60af-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="a60af-188">Laitteen suojausasetusten määrittäminen Windows 10 -tietokoneille</span><span class="sxs-lookup"><span data-stu-id="a60af-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="a60af-189">Kun olet määrittänyt käytännöt, sinä ja työntekijäsi voitte määrittää laitteita:</span><span class="sxs-lookup"><span data-stu-id="a60af-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="a60af-190">Lisätietoja Windows-laitteiden vaiheista [on ohjeaiheessa Windows-laitteiden määrittäminen Microsoft 365 Business Premium -käyttäjille.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="a60af-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="a60af-191">Lisätietoja Android-puhelimista ja iPhoneista on ohjeaiheessa [Mobiililaitteiden määrittäminen Microsoft 365 Business Premium -käyttäjille.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="a60af-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 

### <a name="threat-protection"></a><span data-ttu-id="a60af-192">Uhkien torjunta</span><span class="sxs-lookup"><span data-stu-id="a60af-192">Threat protection</span></span>

<span data-ttu-id="a60af-193">Kun olet siirtynyt Microsoft 365 Business Premiumiin, sinulla on Office 365 ATP.</span><span class="sxs-lookup"><span data-stu-id="a60af-193">After migrating to Microsoft 365 Business Premium, you have Office 365 ATP.</span></span> <span data-ttu-id="a60af-194">Yleiskatsaus on [kohdassa Office 365 ATP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)</span><span class="sxs-lookup"><span data-stu-id="a60af-194">See [Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for an overview.</span></span> <span data-ttu-id="a60af-195">Lisätietoja on ohjeaiheessa [ATP-turvallisten linkkien määrittäminen](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [ATP:n turvallisten liitteiden määrittäminen](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)ja [ATP-tietojenkalastelun torjunta](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span><span class="sxs-lookup"><span data-stu-id="a60af-195">To set up, see [set up ATP safe links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up ATP safe attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up ATP anti-phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="a60af-196">Luottamuksellisuusmerkinnät</span><span class="sxs-lookup"><span data-stu-id="a60af-196">Sensitivity labels</span></span>

<span data-ttu-id="a60af-197">Lisätietoja herkkyystarrojen käyttämisestä on [ohjeaiheessa Herkkyystarrojen yleiskatsaus](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) sekä [herkkyysmerkintöjen](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) videon luominen ja hallinta.</span><span class="sxs-lookup"><span data-stu-id="a60af-197">To start using sensitivity labels, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>
