---
title: Microsoft 365 Businessin määrittäminen ohjatun määritystoiminnon avulla
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Opi neljä vaihetta täyttämällä 365 Microsoft Business määrittäminen.
ms.openlocfilehash: a1c8a41c3e291983276280a063248bdd10a7f85a
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32283891"
---
# <a name="set-up-microsoft-365-business-by-using-the-setup-wizard"></a><span data-ttu-id="04fbe-103">Microsoft 365 Businessin määrittäminen ohjatun määritystoiminnon avulla</span><span class="sxs-lookup"><span data-stu-id="04fbe-103">Set up Microsoft 365 Business by using the setup wizard</span></span>

<span data-ttu-id="04fbe-104">Suorita vaiheet 1-4 alla.</span><span class="sxs-lookup"><span data-stu-id="04fbe-104">Complete steps 1-4 below.</span></span>
  
### <a name="set-up-microsoft-365-business"></a><span data-ttu-id="04fbe-105">Microsoft 365 Businessin määrittäminen</span><span class="sxs-lookup"><span data-stu-id="04fbe-105">Set up Microsoft 365 Business</span></span>

<span data-ttu-id="04fbe-106">Katso video siitä, miten määritetään Microsoft 365 liiketoiminnan, jos sinulla ei ole paikallisen Active Directory:</span><span class="sxs-lookup"><span data-stu-id="04fbe-106">Watch a video on how to set up Microsoft 365 Business when you don't have an on-premises Active Directory:</span></span>
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/0705c337-f3e8-4d28-bb6c-530cd28e99f2?autoplay=false]
  
<span data-ttu-id="04fbe-107">Asetusten määrittämisen vaiheet ovat asetukset, jotka sisältävät paikallisen Active Directoryn tietoja.</span><span class="sxs-lookup"><span data-stu-id="04fbe-107">The set-up steps include information for setups that include local Active Directory.</span></span> <span data-ttu-id="04fbe-108">Jos haluat edelleen käyttää toimialueeseen liittymistä laitteita, lue seuraavista artikkeleista kahdella eri tavalla, käyttöönoton ja kaikki vaiheet on suoritettu, ennen kuin suoritat ohjatun asennuksen:</span><span class="sxs-lookup"><span data-stu-id="04fbe-108">If you want to continue to access domain-joined devices, read the following articles for two different way of enabling that, and complete the steps before you run the Setup wizard:</span></span>
  
- [<span data-ttu-id="04fbe-109">Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi</span><span class="sxs-lookup"><span data-stu-id="04fbe-109">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>](manage-windows-devices.md)
    
    <span data-ttu-id="04fbe-110">-Tämä on suositeltava tapa.</span><span class="sxs-lookup"><span data-stu-id="04fbe-110">-This is the recommended way.</span></span>
    
- [<span data-ttu-id="04fbe-111">Käyttää tiloissa Azure AD liitetty laite 365 Microsoft Business resurssit</span><span class="sxs-lookup"><span data-stu-id="04fbe-111">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>](access-resources.md)
    
### <a name="step-1-personalize-sign-in"></a><span data-ttu-id="04fbe-112">Vaihe 1: Kirjaudu sisään mukauttaminen</span><span class="sxs-lookup"><span data-stu-id="04fbe-112">Step 1: Personalize sign-in</span></span>

1. <span data-ttu-id="04fbe-p102">Kirjaudu sisään [Microsoft 365 Businessiin](https://portal.microsoft.com) käyttämällä yleisen järjestelmänvalvojan tunnistetietojasi. Siirry hallintakeskukseen valitsemalla **Järjestelmänvalvoja**-ruutu.</span><span class="sxs-lookup"><span data-stu-id="04fbe-p102">Sign in to [Microsoft 365 Business](https://portal.microsoft.com) by using your global admin credentials. Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="04fbe-115">Käynnistä ohjattu toiminto valitsemalla hallintakeskuksessa **Aloita määritys** (tilasi mukaan näkyvissä oleva vaihtoehto voi olla **Jatka määritystä**).</span><span class="sxs-lookup"><span data-stu-id="04fbe-115">Choose **Start setup** (depending on your state you may see **Continue setup** instead) in the admin center to start the wizard.</span></span> 
    
3. <span data-ttu-id="04fbe-116">Kirjoita toimialuenimi, jota haluat käyttää (kuten contoso.com).</span><span class="sxs-lookup"><span data-stu-id="04fbe-116">Enter the domain name you want to use (like contoso.com).</span></span>
    
    <span data-ttu-id="04fbe-117">Jatka eteenpäin ja kirjoita toimialueesi, vaikka olisit vahvistanut sen esimerkiksi Azure AD Connectin käytön aikana.</span><span class="sxs-lookup"><span data-stu-id="04fbe-117">Go ahead and enter your domain even if you have verified it while using Azure AD Connect, for example.</span></span> <span data-ttu-id="04fbe-118">Seuraavat kaksi vaihetta ei sovelleta, jos olet käyttänyt AD Azure Yhdistä tarkistamaan toimialueesi.</span><span class="sxs-lookup"><span data-stu-id="04fbe-118">The following two steps do not apply to you if you used Azure AD Connect to verify your domain.</span></span>
    
4. <span data-ttu-id="04fbe-119">Noudata ohjatun toiminnon [luoda DNS-tietueet on mahdollisesti DNS Office 365 videopalvelujen tarjoajan](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) , joka tarkistaa, että omistat toimialueen.</span><span class="sxs-lookup"><span data-stu-id="04fbe-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) that verifies you own the domain.</span></span> 
    
    <span data-ttu-id="04fbe-120">Voit tarkastella esimerkiksi video [Video: uusi Admin Centerissä asennusohjelma Office 365](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8).</span><span class="sxs-lookup"><span data-stu-id="04fbe-120">You can view an example video of [Video: Setup Office 365 in the new Admin Center](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8).</span></span> <span data-ttu-id="04fbe-121">Huomaa, että tämä video ei sisällä ohjeita tietojen suojaukseen Microsoft 365 Business:n avulla.</span><span class="sxs-lookup"><span data-stu-id="04fbe-121">Note that this video does not include the data protection steps of Microsoft 365 Business.</span></span>
    
    ![Screenshot of the Business Cloud Suite setup wizard.](media/3c4fd40c-2de1-4a87-8ee0-78d3928c7bb7.png)
  
### <a name="step-2-add-users-and-assign-licenses"></a><span data-ttu-id="04fbe-123">Vaihe 2: Lisää käyttäjiä ja määrittää käyttöoikeuksia</span><span class="sxs-lookup"><span data-stu-id="04fbe-123">Step 2: Add users and assign licenses</span></span>

1. <span data-ttu-id="04fbe-124">Voit lisätä käyttäjiä tässä, tai voit [lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="04fbe-124">You can add users here, or you can [add users later](add-users-m365b.md) in the admin center.</span></span> 
    
    <span data-ttu-id="04fbe-125">Lisättäville käyttäjille määritetään automaattisesti Microsoft 365 Business-käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="04fbe-125">Any users you add get automatically assigned a Microsoft 365 Business license.</span></span>
    
2. <span data-ttu-id="04fbe-p105">Jos Microsoft 365 Business-tilauksessasi on aiemmin luotuja käyttäjiä (jos esimerkiksi olet käyttänyt Azure AD Connectia), näkyviin tulee vaihtoehto, jolla voit määrittää heille käyttöoikeudet. Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="04fbe-p105">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you will get an option to assign licenses to them now. Go ahead and add licenses to them as well.</span></span>
    
3. <span data-ttu-id="04fbe-p106">Näkyviin tulee myös vaihtoehto, jolla voit jakaa tunnistetiedot lisäämiesi uusien käyttäjien kanssa. Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.</span><span class="sxs-lookup"><span data-stu-id="04fbe-p106">You will also get an option to share credentials with the new users you added. You can choose to print them out, email them, or download them.</span></span>
    
4. <span data-ttu-id="04fbe-130">Ohita sähköpostiviestien siirtäminen valitsemalla **Siirrä sähköpostiviestejä** -sivulla **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="04fbe-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 
    
    <span data-ttu-id="04fbe-131">Jos siirrät toisen sähköpostin tarjoajalta ja haluat kopioida tiedot myöhemmin, voit [Siirtyminen sähköpostin ja yhteystietojen Office 365: ssä](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="04fbe-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>
    
    ![Screenshot of two new users added in the setup wizard](media/8f729967-5c65-4ceb-b737-18119db40564.png)
  
### <a name="step-3-connect-your-domain"></a><span data-ttu-id="04fbe-133">Vaihe 3: Yhdistä toimialueeseen</span><span class="sxs-lookup"><span data-stu-id="04fbe-133">Step 3: Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="04fbe-134">Jos haluat käyttää toimialueen .onmicrosoft tai käyttää AD-Yhdistä Azure, et näe tässä vaiheessa.</span><span class="sxs-lookup"><span data-stu-id="04fbe-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect, you will not see this step.</span></span> 
  
<span data-ttu-id="04fbe-135">Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.</span><span class="sxs-lookup"><span data-stu-id="04fbe-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="04fbe-136">Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa.</span><span class="sxs-lookup"><span data-stu-id="04fbe-136">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="04fbe-137">Jos näin ei ole, [Muuta nameservers määrittäminen Office 365: ssä registrar mahdollisesti toimialueen kanssa](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="04fbe-137">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span>
    
2. <span data-ttu-id="04fbe-138">Sähköposti ja muut palvelut määritetään automaattisesti puolestasi</span><span class="sxs-lookup"><span data-stu-id="04fbe-138">Email and other services will be set up for you</span></span>
    
### <a name="step-4-manage-devices-and-work-files"></a><span data-ttu-id="04fbe-139">Vaihe 4: Hallitse laitteita ja käyttää tiedostoja</span><span class="sxs-lookup"><span data-stu-id="04fbe-139">Step 4: Manage devices and work files</span></span>

1. <span data-ttu-id="04fbe-140">Määritä **Suojaa työtiedostot mobiililaitteissa** -sivulla **Suojaa työtiedostot, kun laitteet katoavat tai varastetaan** -asetukseksi ja **Hallitse, miten käyttäjät voivat käyttää Office-tiedostoja mobiililaitteissa** -asetukseksi **Käytössä**.</span><span class="sxs-lookup"><span data-stu-id="04fbe-140">On the **Protect work files on your mobile devices** page set both **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** settings to **On**.</span></span> <span data-ttu-id="04fbe-141">Voit myös käyttää kunkin osa asetuksen napsauttamalla kunkin asetuksen vieressä olevan nuolen.</span><span class="sxs-lookup"><span data-stu-id="04fbe-141">You can also access each sub-setting by clicking the chevrons next to each setting.</span></span>
  
  <span data-ttu-id="04fbe-142">Kaikki käyttöoikeudet käyttäjien työtä tiedostot on nyt suojattu iOS ja Android-laitteet, niin pian kuin he [asentaa Office apps](set-up-mobile-devices.md) (ja todentaa käyttöoikeutensa Microsoft 365 Business kanssa).</span><span class="sxs-lookup"><span data-stu-id="04fbe-142">All of your licensed users' work files are now protected on iOS and Android devices, as soon as they [install Office apps](set-up-mobile-devices.md) (and authenticate with their Microsoft 365 Business credentials).</span></span> 
  
  ![Screenshot of protect work files on your mobile devices page](media/3139a9aa-6228-4e74-8166-c6a886d7319f.PNG)
  
2. <span data-ttu-id="04fbe-144">**Laitteen kokoonpanotietoja määrittämällä Windows 10** -sivulla Määritä **Suojatun Windows 10-laitteiden** **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="04fbe-144">On the **Set Windows 10 device configuration** page, set **Secure Windows 10 Devices** setting to **On**.</span></span>
  
   <span data-ttu-id="04fbe-145">Voit myös käyttää kunkin osa asetusta napsauttamalla sen vieressä olevaa merkkiä.</span><span class="sxs-lookup"><span data-stu-id="04fbe-145">You can also access each sub-setting by clicking the chevron next to it.</span></span>
  
3. <span data-ttu-id="04fbe-146">Määritä **Windows 10 laitteet asentaa Office** **Kyllä** jos kaikilla käyttäjillä on Windows (10) tietokonetta, ja joko ei ole olemassa Office asentaa tai pika-asennus Office asennetaan.</span><span class="sxs-lookup"><span data-stu-id="04fbe-146">Set the **Install Office on Windows 10 Devices** setting to **Yes** if all of your users have Windows 10 computers, and either no existing Office installs, or click-to-run Office installs.</span></span> <span data-ttu-id="04fbe-147">Jos näin ei ole, Määritä tämän asetuksen arvoksi **ei**.</span><span class="sxs-lookup"><span data-stu-id="04fbe-147">If this is not the case, set this option to **No**.</span></span> <span data-ttu-id="04fbe-148">Voit [asentaa automaattisesti Office](auto-install-or-uninstall-office.md) -hallintakeskukseen, kun olet valmistellut käyttäjien tietokoneissa.</span><span class="sxs-lookup"><span data-stu-id="04fbe-148">You can [automatically install Office](auto-install-or-uninstall-office.md) later from the admin center after you have prepared the user computers.</span></span> <span data-ttu-id="04fbe-149">Lisätietoja on kohdassa [Office-asiakasohjelman asennuksen valmisteleminen](prepare-for-office-client-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="04fbe-149">For instructions, see [prepare for Office client installation](prepare-for-office-client-deployment.md).</span></span>
  
    <span data-ttu-id="04fbe-150">Työtiedostojen lisensoidut käyttäjät Windows 10-laitteiden suunniteltu niin pian kuin ne [liittyä Windows 10-laitteisiinsa](set-up-windows-devices.md) Microsoft 365 Business Azure AD-toimialueen tai [asentaa Windowsin uuteen tietokoneeseen 10](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) , kun samanaikaisesti liittyä Microsoft-365 Business Azure AD-toimialueesta.</span><span class="sxs-lookup"><span data-stu-id="04fbe-150">The licensed users' work files on Windows 10 devices will be projected as soon as they [join their Windows 10 device](set-up-windows-devices.md) to a Microsoft 365 Business Azure AD domain or [install Windows 10 on a new computer](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) while simultaneously joining the Microsoft 365 Business Azure AD domain.</span></span> 
  
4. <span data-ttu-id="04fbe-151">Valitse **Seuraava** ja olet valmis asennuksen kanssa.</span><span class="sxs-lookup"><span data-stu-id="04fbe-151">Click **Next** and you are done with setup.</span></span> 
  
    <span data-ttu-id="04fbe-152">Jätä meille palautetta voit auttaa meitä parantamaan kokemusta tässä vaiheessa.</span><span class="sxs-lookup"><span data-stu-id="04fbe-152">Please leave us feedback at this step to help us improve the experience.</span></span>
  
    ![Screenshot of Prepare Windows 10 devices page](media/bff701c1-48a3-44f4-aa95-9d959d57c85b.PNG)
  
## <a name="additional-security-settings"></a><span data-ttu-id="04fbe-154">Muita tietoturva-asetuksia</span><span class="sxs-lookup"><span data-stu-id="04fbe-154">Additional security settings</span></span>

<span data-ttu-id="04fbe-155">Suojaus ja yhteensopivuus-asetus ohjatun asennuksen lisäksi voit määrittää myös seuraavia lisäasetuksia:</span><span class="sxs-lookup"><span data-stu-id="04fbe-155">In addition to the security and compliance setting in the setup wizard, you can also set up the following additional settings:</span></span>
  
- <span data-ttu-id="04fbe-156">Määritä liitteiden vastaan.</span><span class="sxs-lookup"><span data-stu-id="04fbe-156">Set up protection against unsafe attachments.</span></span> <span data-ttu-id="04fbe-157">**Advanced Threat Protection** (ATP) tunnistaa haitallista sisältöä, ja estää epäluotettavien liitetiedostojen toimittamisen suojaaminen tietojen kalastelussa ja ransomware tartuntoja vastaan.</span><span class="sxs-lookup"><span data-stu-id="04fbe-157">**Advanced Threat Protection** (ATP) identifies malicious content and then blocks delivery of unsafe attachments, helping protect you against phishing schemes and ransomware infections.</span></span> <span data-ttu-id="04fbe-158">Liitetiedostojen suojaus aktivoimaan Katso [määrittäminen Office 365: n ATP Turvalliset liitetiedostot käytäntöjä](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).</span><span class="sxs-lookup"><span data-stu-id="04fbe-158">To activate attachment protection, see [Set up Office 365 ATP Safe Attachments policies](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).</span></span>
    
- <span data-ttu-id="04fbe-159">Suojaa ympäristön, kun käyttäjät napsauttavat haitallisia linkkejä.</span><span class="sxs-lookup"><span data-stu-id="04fbe-159">Protect your environment when users click malicious links.</span></span> <span data-ttu-id="04fbe-160">ATP tarkistaa linkkejä sähköpostitse, kun käyttäjä napsauttaa niitä.</span><span class="sxs-lookup"><span data-stu-id="04fbe-160">ATP examines links in email at the time a user clicks them.</span></span> <span data-ttu-id="04fbe-161">Jos linkkiä ei ole turvallinen, käyttäjä saa varoituksen ei päästä sivustoon tai ilmoittanut, että sivusto on estetty.</span><span class="sxs-lookup"><span data-stu-id="04fbe-161">If a link is unsafe, the user is warned not to visit the site or informed that the site has been blocked.</span></span> <span data-ttu-id="04fbe-162">Tämä auttaa suojautumaan tietojen kalastelussa.</span><span class="sxs-lookup"><span data-stu-id="04fbe-162">This helps protect against phishing schemes.</span></span> <span data-ttu-id="04fbe-163">[Määrittäminen Office 365: n ATP turvallinen linkit käytännöt](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) tai [määrittäminen Office 365: n ATP turvallinen linkit käytäntöjä](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).</span><span class="sxs-lookup"><span data-stu-id="04fbe-163">[Set up Office 365 ATP Safe Links policies](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) or [Set up Office 365 ATP Safe Links policies](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).</span></span>
    
- <span data-ttu-id="04fbe-164">Voit säilyttää kaikki postilaatikon sisältö, mukaan lukien poistetut sijoittamalla käyttäjän koko Postilaatikko- **Pidä oikeudenkäyntiä**.</span><span class="sxs-lookup"><span data-stu-id="04fbe-164">You can preserve all mailbox content including deleted items by putting a user's entire mailbox on **litigation hold**.</span></span> <span data-ttu-id="04fbe-165">Lisätietoja on kohdassa</span><span class="sxs-lookup"><span data-stu-id="04fbe-165">For instructions, see</span></span> 
- <span data-ttu-id="04fbe-166">[Määritä sähköposti pidätyksen kanssa Exchange Online arkistoida](security-features.md#set-up-email-retention-with-exchange-online-archiving).</span><span class="sxs-lookup"><span data-stu-id="04fbe-166">[Set up email retention with Exchange Online Archiving](security-features.md#set-up-email-retention-with-exchange-online-archiving).</span></span>
    
- <span data-ttu-id="04fbe-167">Määritä mukautetut **säilytyskäytännöt**, esimerkiksi tietyn ajanjakson aikana säilyttää tai poistaa sisällön pysyvästi säilytysajan päätyttyä.</span><span class="sxs-lookup"><span data-stu-id="04fbe-167">Set up customized **retention policies**, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="04fbe-168">Voit ottaa käyttöön mukautetut säilytyskäytännöt arvopapereihin ja compliance Centeriin, siirry **Data hallinnon** \> **pidätys**ja noudata sitten ohjatun toiminnon ohjeita.</span><span class="sxs-lookup"><span data-stu-id="04fbe-168">You can enable customized retention policies in the Securities and compliance center, go to **Data governance** \> **Retention**, and then follow the steps in the wizard.</span></span> <span data-ttu-id="04fbe-169">Lisätietoja on kohdassa [Yleiskatsaus säilytyskäytäntöjä](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="04fbe-169">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>
    
## <a name="next-steps"></a><span data-ttu-id="04fbe-170">Seuraavat vaiheet</span><span class="sxs-lookup"><span data-stu-id="04fbe-170">Next steps</span></span>

<span data-ttu-id="04fbe-171">Käyttöoikeudet omaavilla käyttäjillä seuraava vaihe on laitteiden määrittäminen.</span><span class="sxs-lookup"><span data-stu-id="04fbe-171">For the users that have their licenses, the next step is to set up devices.</span></span><br/> <span data-ttu-id="04fbe-172">Tutustu [Windows-laitteiden määrittäminen Microsoft 365 Business -käyttäjille](set-up-windows-devices.md) ja [Mobiililaitteiden määrittäminen Microsoft 365 Business -käyttäjille](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="04fbe-172">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) and [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span> <br/><span data-ttu-id="04fbe-173">Kohdassa [Microsoft 365 Businessin hallinta](manage.md) on linkit aiheisiin, joissa on ohjeet laitteiden ja sovellusten suojauskäytäntöjen määrittämiseen ja tietojen poistamiseen käyttäjien laitteista.</span><span class="sxs-lookup"><span data-stu-id="04fbe-173">See [Manage Microsoft 365 Business](manage.md) for links to topics on how to set device and app protection polices, and how to remove data from user devices.</span></span> 
  


