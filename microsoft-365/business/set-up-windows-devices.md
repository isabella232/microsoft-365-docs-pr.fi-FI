---
title: Windows-laitteiden määrittäminen Microsoft 365 Business -käyttäjille
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
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: 'Lue, miten voit määrittää Windows 10 Pro for Microsoft 365-käyttö järjestelmä käyttäjät. '
ms.openlocfilehash: b377c1e69d117b893b256880cd3b9972e33345c7
ms.sourcegitcommit: 8fda7852b2a5baa92b8a365865b014ea6d100bbc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/03/2019
ms.locfileid: "39812874"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a><span data-ttu-id="e04aa-103">Windows-laitteiden määrittäminen Microsoft 365 Business -käyttäjille</span><span class="sxs-lookup"><span data-stu-id="e04aa-103">Set up Windows devices for Microsoft 365 Business users</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e04aa-104">Edellytykset</span><span class="sxs-lookup"><span data-stu-id="e04aa-104">Prerequisites</span></span>

<span data-ttu-id="e04aa-p101">Ennen kuin voit määrittää Windows-laitteet Microsoft 365 Business -käyttäjiä varten, varmista, että kaikissa Windows-laitteissa on Windows 10 Pro -versio 1703 (Creators-päivitys). Windows 10 Pro on edellytys Windows 10 Businessin käyttöönotolle. Se on joukko pilvipalveluja ja laitehallintaominaisuuksia, jotka täydentävät Windows 10 Pro -ohjelmistoa ja mahdollistavat Microsoft 365 Businessin keskitetyn valvonnan ja suojauksen hallinnan.</span><span class="sxs-lookup"><span data-stu-id="e04aa-p101">Before you can set up Windows devices for Microsoft 365 Business users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update). Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business.</span></span>
  
<span data-ttu-id="e04aa-107">Jos käytössäsi on Windows-laitteita, joissa on Windows 7 Pro, Windows 8 Pro tai Windows 8.1 Pro, Microsoft 365 Business -tilaus oikeuttaa sinut Windows 10 -päivitykseen.</span><span class="sxs-lookup"><span data-stu-id="e04aa-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="e04aa-108">Lisätietoja Windows-laitteiden Windows 10 Pro Creators -päivityksen tekemisestä on tämän aiheen ohjeissa: [Windows Pro Creators -päivityksen tekeminen Windows-laitteisiin](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="e04aa-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="e04aa-109">Tarkista, että sinulla on päivitys, ja varmista, että päivitys toimi, tarkistamalla, [että laite on yhdistetty Azure AD-verkkoon](#verify-the-device-is-connected-to-azure-ad) .</span><span class="sxs-lookup"><span data-stu-id="e04aa-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="e04aa-110">Katso lyhyt video Windowsin yhdistämisestä Microsoft 365: een.</span><span class="sxs-lookup"><span data-stu-id="e04aa-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="e04aa-111">Jos olet löytänyt tämän videon hyödyllisiksi, tutustu [koko koulutus sarjaan pien yrityksille ja niille, jotka ovat Microsoft 365-yrityksen uusia](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="e04aa-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="e04aa-112">Windows 10 -laitteiden liittäminen organisaatiosi Azure AD:hen</span><span class="sxs-lookup"><span data-stu-id="e04aa-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="e04aa-113">Kun kaikki organisaatiosi Windows-laitteet on joko päivitetty Windows 10 Pro Creators-päivitykseen tai jo käytössä on Windows 10 Pro Creators Update, voit liittyä näihin laitteisiin organisaatiosi Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="e04aa-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="e04aa-114">Kun laitteet on liitetty, ne päivitetään automaattisesti Windows 10 Business-versioon, joka on osa Microsoft 365 Business-tilausta.</span><span class="sxs-lookup"><span data-stu-id="e04aa-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="e04aa-115">Uusi tai päivitetty Windows 10 Pro -laite</span><span class="sxs-lookup"><span data-stu-id="e04aa-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="e04aa-116">Jos laite on uusi laite, jossa on Windows 10 Pro Creators -päivitys, tai laitteeseen on tehty Windows 10 Pro Creators -päivitys, mutta ei vielä Windows 10 -laitemääritystä, noudata seuraavia ohjeita.</span><span class="sxs-lookup"><span data-stu-id="e04aa-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="e04aa-117">Suorita Windows 10 -laitteen asennus, kunnes näyttöön tulee **Miten haluat määrittää?** -sivu.</span><span class="sxs-lookup"><span data-stu-id="e04aa-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="e04aa-119">Valitse sitten **Määritä organisaatiolle** ja anna Microsoft 365 Business -käyttäjänimesi ja -salasanasi.</span><span class="sxs-lookup"><span data-stu-id="e04aa-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business.</span></span> 
    
3. <span data-ttu-id="e04aa-120">Viimeistele Windows 10 -laitteen määritys.</span><span class="sxs-lookup"><span data-stu-id="e04aa-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="e04aa-p103">Kun olet valmis, käyttäjä yhdistetään organisaatiosi Azure AD:hen. Varmista tämä kohdan [Laitteen Azure AD -yhteyden tarkistaminen](#verify-the-device-is-connected-to-azure-ad) ohjeiden mukaan.</span><span class="sxs-lookup"><span data-stu-id="e04aa-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="e04aa-123">Laite, joka on jo määritetty ja jossa on Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="e04aa-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="e04aa-124">**Käyttäjien yhdistäminen Azure AD:hen:**</span><span class="sxs-lookup"><span data-stu-id="e04aa-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="e04aa-125">Valitse käyttäjän Windows-tietokoneessa, jossa on käytössä Windows 10 Pro -versio 1703 (Creators-päivitys) (katso [edellytykset](pre-requisites-for-data-protection.md)), Windows-näppäin ja valitse sitten Asetukset-kuvake.</span><span class="sxs-lookup"><span data-stu-id="e04aa-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="e04aa-127">Vallitse **Asetukset** ja valitse sitten **Tilit**.</span><span class="sxs-lookup"><span data-stu-id="e04aa-127">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="e04aa-129">Valitse **Omat tiedot** -sivulla **Käytä työpaikan tai koulun resursseja** \> **Yhdistä**.</span><span class="sxs-lookup"><span data-stu-id="e04aa-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="e04aa-131">Valitse **Määritä työpaikan tai oppilaitoksen tili** -valintaikkunan **Vaihtoehtoiset toimet** -kohdassa **Liitä tämä laite Azure Active Directoryyn**.</span><span class="sxs-lookup"><span data-stu-id="e04aa-131">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="e04aa-133">Kirjoita **Kirjaudu sisään** -sivulla työpaikan tai oppilaitoksen tili \> **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="e04aa-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="e04aa-134">Kirjoita salasana **Anna salasana** -sivulla \> **Kirjaudu**.</span><span class="sxs-lookup"><span data-stu-id="e04aa-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="e04aa-136">Varmista, että **Tämä on organisaatiosi** sivu, varmista, että tiedot ovat oikein, ja valitse **Liity**.</span><span class="sxs-lookup"><span data-stu-id="e04aa-136">On the **Make sure this is your organization** page, verify that the information is correct, and click **Join**.</span></span>
  
   <span data-ttu-id="e04aa-p104">Valitse **Olet valmis!** -sivulla **Valmis**.</span><span class="sxs-lookup"><span data-stu-id="e04aa-p104">On the **You're all set!** page, click **Done**.</span></span>
  
   ![On the Make sure this is your organization screen, click Join](media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="e04aa-140">Jos olet ladannut tiedostoja OneDrive for Businessiin, synkronoi ne takaisin.</span><span class="sxs-lookup"><span data-stu-id="e04aa-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="e04aa-141">Jos olet käyttänyt kolmannen osapuolen työkalua profiilin ja tiedostojen siirtämisessä, synkronoi ne myös uuteen profiiliin.</span><span class="sxs-lookup"><span data-stu-id="e04aa-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="e04aa-142">Laitteen Azure AD -yhteyden tarkistaminen</span><span class="sxs-lookup"><span data-stu-id="e04aa-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="e04aa-p106">Tarkista synkronointitilasi napsauttamalla **Asetukset**-valintaikkunan **Käytä työpaikan tai koulun resursseja** -sivulla **Yhdistä kohteeseen** _ \<organization name\> _ -alueella, jolloin painikkeet **Tiedot** ja **Katkaise yhteys** tulevat näkyviin. Tuo synkronointitilasi näkyviin valitsemalla **Tiedot**.</span><span class="sxs-lookup"><span data-stu-id="e04aa-p106">To verify your sync status, on the **Access work or school** page in **Settings**, click in the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**. Click on **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="e04aa-145">Valitse Synkronointitila-sivulla Synkronoi, jolloin saat uusimmat mobiililaitteiden hallintakäytännöt PC-tietokoneeseen.</span><span class="sxs-lookup"><span data-stu-id="e04aa-145">On the Sync status page, click Sync to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="e04aa-146">Jos haluat aloittaa Microsoft 365-yritys tilin käyttämisen, siirry Windowsin **Käynnistä** -painikkeeseen, napsauta hiiren kakkos painikkeella nykyistä tili kuvaasi ja **Vaihda sitten tiliä**.</span><span class="sxs-lookup"><span data-stu-id="e04aa-146">To start using the Microsoft 365 Business account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="e04aa-147">Kirjaudu sisään käyttämällä organisaatiosi sähköpostiosoitetta ja salasanaa.</span><span class="sxs-lookup"><span data-stu-id="e04aa-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a><span data-ttu-id="e04aa-149">Windows 10 Business -päivityksen olemassaolon tarkistaminen laitteessa</span><span class="sxs-lookup"><span data-stu-id="e04aa-149">Verify the device is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="e04aa-150">Varmista, että Azure Active Directoryyn liitettyihin Windows 10 -laitteisiin on päivitetty Windows 10 Business osana Microsoft 365 Business -tilausta.</span><span class="sxs-lookup"><span data-stu-id="e04aa-150">Verify that your Azure AD joined Windows 10 devices were upgraded to Windows 10 Business as part of your Microsoft 365 Business subscription.</span></span>
  
1. <span data-ttu-id="e04aa-151">Valitse **Asetukset** \> **Järjestelmä** \> **Tietoja**.</span><span class="sxs-lookup"><span data-stu-id="e04aa-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="e04aa-152">Varmista, että **Julkaisu**-kohdassa lukee **Windows 10 Business**.</span><span class="sxs-lookup"><span data-stu-id="e04aa-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="e04aa-154">Seuraavat vaiheet</span><span class="sxs-lookup"><span data-stu-id="e04aa-154">Next steps</span></span>

<span data-ttu-id="e04aa-155">Mobiililaitteiden määritysohjeet ovat kohdassa [Mobiililaitteiden määrittäminen Microsoft 365 Business -käyttäjille](set-up-mobile-devices.md). Laitteiden ja sovellusten suojauskäytäntöjen määritysohjeet ovat kohdassa [Microsoft 365 Businessin hallinta](manage.md).</span><span class="sxs-lookup"><span data-stu-id="e04aa-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 Business](manage.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="e04aa-156">Katso myös</span><span class="sxs-lookup"><span data-stu-id="e04aa-156">See also</span></span>

[<span data-ttu-id="e04aa-157">Microsoft 365-liike toiminnan koulutus videot</span><span class="sxs-lookup"><span data-stu-id="e04aa-157">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
