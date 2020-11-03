---
title: Windows-laitteiden määrittäminen Microsoft 365 Business Premium-käyttäjille
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Lue, miten voit määrittää Windows 10 Pro-käyttö järjestelmän Microsoft 365 Business Premium-käyttäjille ja ottaa käyttöön keskitetyn hallinnan ja tieto turvan hallinta toiminnot.
ms.openlocfilehash: c95b9e51c7ec3c440509fe34084d2a030c7f2eec
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841255"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="af498-103">Windows-laitteiden määrittäminen Microsoft 365 Business Premium-käyttäjille</span><span class="sxs-lookup"><span data-stu-id="af498-103">Set up Windows devices for Microsoft 365 Business Premium users</span></span>

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="af498-104">Microsoft 365 Business Premium-käyttäjien Windows-laitteiden määrittämisen edellytykset</span><span class="sxs-lookup"><span data-stu-id="af498-104">Prerequisites for setting up Windows devices for Microsoft 365 Business Premium users</span></span>

<span data-ttu-id="af498-105">Ennen kuin voit määrittää Windows-laitteita Microsoft 365 Business Premium-käyttäjille, varmista, että kaikissa Windows-laitteissa on käytössä Windows 10 Pro, versio 1703 (Creators Update).</span><span class="sxs-lookup"><span data-stu-id="af498-105">Before you can set up Windows devices for Microsoft 365 Business Premium users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update).</span></span> <span data-ttu-id="af498-106">Windows 10 Pro on Windows 10 Businessin käyttöönoton edellytys, joka on pilvi palveluiden ja laite hallinnan ominaisuuksien joukko, joka täydentää Windows 10 Prota ja mahdollistaa Microsoft 365 Business Premiumin keskitetyn hallinnan ja tieto turvan.</span><span class="sxs-lookup"><span data-stu-id="af498-106">Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business Premium.</span></span>
  
<span data-ttu-id="af498-107">Jos käytössäsi on Windows-laite, jossa on Windows 7 Pro, Windows 8 Pro tai Windows 8,1 Pro, Microsoft 365 Business Premium-tilauksesi oikeuttaa sinut Windows 10-päivitykseen.</span><span class="sxs-lookup"><span data-stu-id="af498-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business Premium subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="af498-108">Lisätietoja Windows-laitteiden Windows 10 Pro Creators -päivityksen tekemisestä on tämän aiheen ohjeissa: [Windows Pro Creators -päivityksen tekeminen Windows-laitteisiin](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="af498-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="af498-109">Lisä tietoja on kohdassa [Varmista, että laite on yhdistetty Azure](#verify-the-device-is-connected-to-azure-ad) AD:hen, ja tarkista, että päivitys on tehty, tai varmista, että päivitys on toiminut.</span><span class="sxs-lookup"><span data-stu-id="af498-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="af498-110">Katso lyhyt video, jossa on tietoja Windowsin liittämisestä Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="af498-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="af498-111">Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="af498-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="af498-112">Windows 10 -laitteiden liittäminen organisaatiosi Azure AD:hen</span><span class="sxs-lookup"><span data-stu-id="af498-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="af498-113">Kun kaikki organisaatiosi Windows-laitteet on päivitetty Windows 10 Pro Creators-päivitykseen tai Windows 10 Pro Creators-päivitys on jo asennettu, voit liittää nämä laitteet organisaatiosi Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="af498-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="af498-114">Kun laitteet on liitetty, ne päivitetään automaattisesti Windows 10 Business-versioon, joka kuuluu Microsoft 365 Business Premium-tilaukseesi.</span><span class="sxs-lookup"><span data-stu-id="af498-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business Premium subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="af498-115">Uusi tai päivitetty Windows 10 Pro -laite</span><span class="sxs-lookup"><span data-stu-id="af498-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="af498-116">Jos laite on uusi laite, jossa on Windows 10 Pro Creators -päivitys, tai laitteeseen on tehty Windows 10 Pro Creators -päivitys, mutta ei vielä Windows 10 -laitemääritystä, noudata seuraavia ohjeita.</span><span class="sxs-lookup"><span data-stu-id="af498-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="af498-117">Suorita Windows 10 -laitteen asennus, kunnes näyttöön tulee **Miten haluat määrittää?** -sivu.</span><span class="sxs-lookup"><span data-stu-id="af498-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="af498-119">Valitse tässä **kohdassa Määritä organisaatiolle** ja anna sitten Microsoft 365 Business Premiumin käyttäjä nimi ja sala sana.</span><span class="sxs-lookup"><span data-stu-id="af498-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business Premium.</span></span> 
    
3. <span data-ttu-id="af498-120">Viimeistele Windows 10 -laitteen määritys.</span><span class="sxs-lookup"><span data-stu-id="af498-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="af498-p103">Kun olet valmis, käyttäjä yhdistetään organisaatiosi Azure AD:hen. Varmista tämä kohdan [Laitteen Azure AD -yhteyden tarkistaminen](#verify-the-device-is-connected-to-azure-ad) ohjeiden mukaan.</span><span class="sxs-lookup"><span data-stu-id="af498-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="af498-123">Laite, joka on jo määritetty ja jossa on Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="af498-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="af498-124">**Käyttäjien yhdistäminen Azure AD:hen:**</span><span class="sxs-lookup"><span data-stu-id="af498-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="af498-125">Valitse käyttäjän Windows-tietokoneessa, jossa on käytössä Windows 10 Pro -versio 1703 (Creators-päivitys) (katso [edellytykset](pre-requisites-for-data-protection.md)), Windows-näppäin ja valitse sitten Asetukset-kuvake.</span><span class="sxs-lookup"><span data-stu-id="af498-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="af498-127">Vallitse **Asetukset** ja valitse sitten **Tilit**.</span><span class="sxs-lookup"><span data-stu-id="af498-127">In **Settings** , go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="af498-129">Valitse **Omat tiedot** -sivulla **Käytä työpaikan tai koulun resursseja** \> **Yhdistä**.</span><span class="sxs-lookup"><span data-stu-id="af498-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="af498-131">Valitse **Määritä työpaikan tai oppilaitoksen tili** -valintaikkunan **Vaihtoehtoiset toimet** -kohdassa **Liitä tämä laite Azure Active Directoryyn**.</span><span class="sxs-lookup"><span data-stu-id="af498-131">On the **Set up a work or school account** dialog, under **Alternate actions** , choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="af498-133">Kirjoita **Kirjaudu sisään** -sivulla työpaikan tai oppilaitoksen tili \> **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="af498-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="af498-134">Kirjoita salasana **Anna salasana** -sivulla \> **Kirjaudu**.</span><span class="sxs-lookup"><span data-stu-id="af498-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="af498-136">Varmista, että **Tämä on organisaatiosi** -sivulla Tarkista, että tiedot ovat oikein, ja valitse **Liity**.</span><span class="sxs-lookup"><span data-stu-id="af498-136">On the **Make sure this is your organization** page, verify that the information is correct, and choose **Join**.</span></span>
  
   <span data-ttu-id="af498-137">Valitse **Olet valmis!**</span><span class="sxs-lookup"><span data-stu-id="af498-137">On the **You're all set!**</span></span> <span data-ttu-id="af498-138">sivu, valitse jokin kolmesta **Done**.</span><span class="sxs-lookup"><span data-stu-id="af498-138">page, chosse **Done**.</span></span>
  
   ![Valitse Varmista, että tämä on organisaatiosi-näytössä liity](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="af498-140">Jos olet ladannut tiedostoja OneDrive for Businessiin, synkronoi ne takaisin.</span><span class="sxs-lookup"><span data-stu-id="af498-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="af498-141">Jos käytit kolmannen osapuolen työkalua profiilin ja tiedostojen siirtämiseen, synkronoi ne myös uuteen profiiliin.</span><span class="sxs-lookup"><span data-stu-id="af498-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="af498-142">Laitteen Azure AD -yhteyden tarkistaminen</span><span class="sxs-lookup"><span data-stu-id="af498-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="af498-143">Jos haluat tarkistaa synkronoinnin tilan, valitse **Asetukset** -kohdan **Käytä työpaikan tai oppi laitoksen** sivulla **yhdistetty** _ _- \<organization name\> alue, jos haluat näyttää painikkeiden **tiedot** ja **katkaista yhteyden**.</span><span class="sxs-lookup"><span data-stu-id="af498-143">To verify your sync status, on the **Access work or school** page in **Settings** , select the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**.</span></span> <span data-ttu-id="af498-144">Saat synkronoinnin tilan valitsemalla **tiedot** .</span><span class="sxs-lookup"><span data-stu-id="af498-144">Choose **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="af498-145">Valitse **synkronoinnin tila** -sivulla **Synkronoi** , jotta saat uusimmat mobiililaitteiden hallinta käytännöt tieto koneeseen.</span><span class="sxs-lookup"><span data-stu-id="af498-145">On the **Sync status** page, choose **Sync** to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="af498-146">Voit aloittaa Microsoft 365 Business Premium-tilin käytön siirtymällä Windowsin **Käynnistä** -painikkeeseen, napsauttamalla nykyistä tili kuvaasi hiiren kakkos painikkeella ja **vaihtamalla sitten tilin**.</span><span class="sxs-lookup"><span data-stu-id="af498-146">To start using the Microsoft 365 Business Premium account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="af498-147">Kirjaudu sisään käyttämällä organisaatiosi sähköpostiosoitetta ja salasanaa.</span><span class="sxs-lookup"><span data-stu-id="af498-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a><span data-ttu-id="af498-149">Varmista, että tieto kone on päivitetty Windows 10 Business-versioon</span><span class="sxs-lookup"><span data-stu-id="af498-149">Verify the PC is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="af498-150">Varmista, että Azure AD on liittynyt Windows 10-laitteisiin Windows 10 Business-versioon osana Microsoft 365 Business Premium-tilausta.</span><span class="sxs-lookup"><span data-stu-id="af498-150">Verify that your Azure AD joined Windows 10 devices are upgraded to Windows 10 Business as part of your Microsoft 365 Business Premium subscription.</span></span>
  
1. <span data-ttu-id="af498-151">Valitse **Asetukset** \> **Järjestelmä** \> **Tietoja**.</span><span class="sxs-lookup"><span data-stu-id="af498-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="af498-152">Varmista, että **Julkaisu** -kohdassa lukee **Windows 10 Business**.</span><span class="sxs-lookup"><span data-stu-id="af498-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="af498-154">Seuraavat vaiheet</span><span class="sxs-lookup"><span data-stu-id="af498-154">Next steps</span></span>

<span data-ttu-id="af498-155">Lisä tietoja mobiililaitteiden määrittämisestä on kohdassa [mobiililaitteiden määrittäminen microsoft 365 Business Premium-käyttäjille](set-up-mobile-devices.md), laitteen suojaus asetusten ja sovellusten suojaus käytäntöjen määrittäminen on kohdassa [Microsoft 365 for Businessin hallinta](manage.md).</span><span class="sxs-lookup"><span data-stu-id="af498-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 for business](manage.md).</span></span>
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a><span data-ttu-id="af498-156">Lisä tietoja Microsoft 365 Business Premiumin määrittämisestä ja käyttämisestä</span><span class="sxs-lookup"><span data-stu-id="af498-156">For more on setting up and using Microsoft 365 Business Premium</span></span>

[<span data-ttu-id="af498-157">Microsoft 365 for Business-koulutus videot</span><span class="sxs-lookup"><span data-stu-id="af498-157">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
