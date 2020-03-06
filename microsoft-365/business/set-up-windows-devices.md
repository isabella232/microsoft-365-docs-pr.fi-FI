---
title: Windows-laitteiden määrittäminen Microsoft 365 Business -käyttäjille
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Lue, miten voit määrittää Windows-laitteet, joissa on Windows 10 Pro for Microsoft 365 Business -käyttäjille, jolloin käytössä on keskitetty hallinta- ja suojausvalvonta.
ms.openlocfilehash: 62d909b1e5658131f9381d1a800a70fad6e16cab
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550013"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a><span data-ttu-id="ff0d0-103">Windows-laitteiden määrittäminen Microsoft 365 Business -käyttäjille</span><span class="sxs-lookup"><span data-stu-id="ff0d0-103">Set up Windows devices for Microsoft 365 Business users</span></span>

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-users"></a><span data-ttu-id="ff0d0-104">Edellytykset Windows-laitteiden määrittämiselle Microsoft 365 Business -käyttäjille</span><span class="sxs-lookup"><span data-stu-id="ff0d0-104">Prerequisites for setting up Windows devices for Microsoft 365 Business users</span></span>

<span data-ttu-id="ff0d0-p101">Ennen kuin voit määrittää Windows-laitteet Microsoft 365 Business -käyttäjiä varten, varmista, että kaikissa Windows-laitteissa on Windows 10 Pro -versio 1703 (Creators-päivitys). Windows 10 Pro on edellytys Windows 10 Businessin käyttöönotolle. Se on joukko pilvipalveluja ja laitehallintaominaisuuksia, jotka täydentävät Windows 10 Pro -ohjelmistoa ja mahdollistavat Microsoft 365 Businessin keskitetyn valvonnan ja suojauksen hallinnan.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-p101">Before you can set up Windows devices for Microsoft 365 Business users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update). Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business.</span></span>
  
<span data-ttu-id="ff0d0-107">Jos käytössäsi on Windows-laitteita, joissa on Windows 7 Pro, Windows 8 Pro tai Windows 8.1 Pro, Microsoft 365 Business -tilaus oikeuttaa sinut Windows 10 -päivitykseen.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="ff0d0-108">Lisätietoja Windows-laitteiden Windows 10 Pro Creators -päivityksen tekemisestä on tämän aiheen ohjeissa: [Windows Pro Creators -päivityksen tekeminen Windows-laitteisiin](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="ff0d0-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="ff0d0-109">Lisätietoja on ohjeaiheessa [Laitteen on yhdistetty Azure AD:hen,](#verify-the-device-is-connected-to-azure-ad) jotta voit varmistaa, että päivitys on muodostettu, tai varmista, että päivitys toimi.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="ff0d0-110">Katso lyhyt video Windowsin yhdistämisestä Microsoft 365:een.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="ff0d0-111">Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="ff0d0-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="ff0d0-112">Windows 10 -laitteiden liittäminen organisaatiosi Azure AD:hen</span><span class="sxs-lookup"><span data-stu-id="ff0d0-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="ff0d0-113">Kun kaikki organisaatiosi Windows-laitteet on joko päivitetty Windows 10 Pro Creators Updateksi tai niissä on jo Windows 10 Pro Creators Update , voit liittyä näihin laitteisiin organisaatiosi Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="ff0d0-114">Kun laitteet on liitetty, ne päivitetään automaattisesti Windows 10 Businessiin, joka on osa Microsoft 365 Business -tilaustasi.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="ff0d0-115">Uusi tai päivitetty Windows 10 Pro -laite</span><span class="sxs-lookup"><span data-stu-id="ff0d0-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="ff0d0-116">Jos laite on uusi laite, jossa on Windows 10 Pro Creators -päivitys, tai laitteeseen on tehty Windows 10 Pro Creators -päivitys, mutta ei vielä Windows 10 -laitemääritystä, noudata seuraavia ohjeita.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="ff0d0-117">Suorita Windows 10 -laitteen asennus, kunnes näyttöön tulee **Miten haluat määrittää?** -sivu.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="ff0d0-119">Valitse sitten **Määritä organisaatiolle** ja anna Microsoft 365 Business -käyttäjänimesi ja -salasanasi.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business.</span></span> 
    
3. <span data-ttu-id="ff0d0-120">Viimeistele Windows 10 -laitteen määritys.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="ff0d0-p103">Kun olet valmis, käyttäjä yhdistetään organisaatiosi Azure AD:hen. Varmista tämä kohdan [Laitteen Azure AD -yhteyden tarkistaminen](#verify-the-device-is-connected-to-azure-ad) ohjeiden mukaan.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="ff0d0-123">Laite, joka on jo määritetty ja jossa on Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="ff0d0-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="ff0d0-124">**Käyttäjien yhdistäminen Azure AD:hen:**</span><span class="sxs-lookup"><span data-stu-id="ff0d0-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="ff0d0-125">Valitse käyttäjän Windows-tietokoneessa, jossa on käytössä Windows 10 Pro -versio 1703 (Creators-päivitys) (katso [edellytykset](pre-requisites-for-data-protection.md)), Windows-näppäin ja valitse sitten Asetukset-kuvake.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="ff0d0-127">Vallitse **Asetukset** ja valitse sitten **Tilit**.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-127">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="ff0d0-129">Valitse **Omat tiedot** -sivulla **Käytä työpaikan tai koulun resursseja** \> **Yhdistä**.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="ff0d0-131">Valitse **Määritä työpaikan tai oppilaitoksen tili** -valintaikkunan **Vaihtoehtoiset toimet** -kohdassa **Liitä tämä laite Azure Active Directoryyn**.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-131">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="ff0d0-133">Kirjoita **Kirjaudu sisään** -sivulla työpaikan tai oppilaitoksen tili \> **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="ff0d0-134">Kirjoita salasana **Anna salasana** -sivulla \> **Kirjaudu**.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="ff0d0-136">Varmista **Varmista, että tämä on organisaatiosi** -sivulla, että tiedot ovat oikein, ja valitse **Liity**.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-136">On the **Make sure this is your organization** page, verify that the information is correct, and click **Join**.</span></span>
  
   <span data-ttu-id="ff0d0-p104">Valitse **Olet valmis!** -sivulla **Valmis**.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-p104">On the **You're all set!** page, click **Done**.</span></span>
  
   ![On the Make sure this is your organization screen, click Join](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="ff0d0-140">Jos olet ladannut tiedostoja OneDrive for Businessiin, synkronoi ne takaisin.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="ff0d0-141">Jos käytit kolmannen osapuolen työkalua profiilin ja tiedostojen siirtämiseen, synkronoi ne myös uuteen profiiliin.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="ff0d0-142">Laitteen Azure AD -yhteyden tarkistaminen</span><span class="sxs-lookup"><span data-stu-id="ff0d0-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="ff0d0-p106">Tarkista synkronointitilasi napsauttamalla **Asetukset**-valintaikkunan **Käytä työpaikan tai koulun resursseja** -sivulla **Yhdistä kohteeseen** _ \<organization name\> _ -alueella, jolloin painikkeet **Tiedot** ja **Katkaise yhteys** tulevat näkyviin. Tuo synkronointitilasi näkyviin valitsemalla **Tiedot**.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-p106">To verify your sync status, on the **Access work or school** page in **Settings**, click in the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**. Click on **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="ff0d0-145">Valitse Synkronointitila-sivulla Synkronoi, jolloin saat uusimmat mobiililaitteiden hallintakäytännöt PC-tietokoneeseen.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-145">On the Sync status page, click Sync to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="ff0d0-146">Voit aloittaa Microsoft 365 Business -tilin \*\*\*\* käytön siirtymällä Windowsin Käynnistä-valikkoon, napsauttamalla nykyistä tilikuvaahiiren kakkospainikkeella ja **vaihtamalla sitten tilin vaihtamista**.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-146">To start using the Microsoft 365 Business account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="ff0d0-147">Kirjaudu sisään käyttämällä organisaatiosi sähköpostiosoitetta ja salasanaa.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a><span data-ttu-id="ff0d0-149">Windows 10 Business -päivityksen olemassaolon tarkistaminen laitteessa</span><span class="sxs-lookup"><span data-stu-id="ff0d0-149">Verify the device is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="ff0d0-150">Varmista, että Azure Active Directoryyn liitettyihin Windows 10 -laitteisiin on päivitetty Windows 10 Business osana Microsoft 365 Business -tilausta.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-150">Verify that your Azure AD joined Windows 10 devices were upgraded to Windows 10 Business as part of your Microsoft 365 Business subscription.</span></span>
  
1. <span data-ttu-id="ff0d0-151">Valitse **Asetukset** \> **Järjestelmä** \> **Tietoja**.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="ff0d0-152">Varmista, että **Julkaisu**-kohdassa lukee **Windows 10 Business**.</span><span class="sxs-lookup"><span data-stu-id="ff0d0-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="ff0d0-154">Seuraavat vaiheet</span><span class="sxs-lookup"><span data-stu-id="ff0d0-154">Next steps</span></span>

<span data-ttu-id="ff0d0-155">Mobiililaitteiden määritysohjeet ovat kohdassa [Mobiililaitteiden määrittäminen Microsoft 365 Business -käyttäjille](set-up-mobile-devices.md). Laitteiden ja sovellusten suojauskäytäntöjen määritysohjeet ovat kohdassa [Microsoft 365 Businessin hallinta](manage.md).</span><span class="sxs-lookup"><span data-stu-id="ff0d0-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 Business](manage.md).</span></span>
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business"></a><span data-ttu-id="ff0d0-156">Lisätietoja Microsoft 365 Businessin määrittämisestä ja käyttämisestä</span><span class="sxs-lookup"><span data-stu-id="ff0d0-156">For more on setting up and using Microsoft 365 Business</span></span>

[<span data-ttu-id="ff0d0-157">Microsoft 365 Business -koulutusvideot</span><span class="sxs-lookup"><span data-stu-id="ff0d0-157">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
