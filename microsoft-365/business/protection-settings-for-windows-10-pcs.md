---
title: Laitteiden suojausasetusten määrittäminen Windows 10 -tietokoneita varten
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Lisätietoja oletus ja muut asetukset Microsoft 365 Business suojaa Windows 10-laitteiden käytettävissä.
ms.openlocfilehash: ebfe5f59e544b67e5a4f2ecd990031e9221ff8e5
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982143"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a><span data-ttu-id="0e3a2-103">Laitteiden suojausasetusten määrittäminen Windows 10 -tietokoneita varten</span><span class="sxs-lookup"><span data-stu-id="0e3a2-103">Set device protection settings for Windows 10 PCs</span></span>

## <a name="secure-windows-10-devices"></a><span data-ttu-id="0e3a2-104">Suojatut Windows 10 -laitteet</span><span class="sxs-lookup"><span data-stu-id="0e3a2-104">Secure Windows 10 devices</span></span>

<span data-ttu-id="0e3a2-105">Katso video Windows 10 -laitteiden suojaamisesta Microsoft 365 Businessin avulla:</span><span class="sxs-lookup"><span data-stu-id="0e3a2-105">View a video on how to secure Windows 10 devices with Microsoft 365 Business:</span></span>
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. <span data-ttu-id="0e3a2-106">Kirjaudu [Microsoft 365 Businessiin](https://portal.office.com) yleisen järjestelmänvalvojan tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="0e3a2-106">Sign in to [Microsoft 365 Business](https://portal.office.com) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="0e3a2-107">Valitse hallintakeskuksen **Laitekäytännöt**-kortissa **Lisää käytäntö**.</span><span class="sxs-lookup"><span data-stu-id="0e3a2-107">in the admin center, on the **Device policies** card, choose **Add policy**.</span></span>
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. <span data-ttu-id="0e3a2-109">Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle.</span><span class="sxs-lookup"><span data-stu-id="0e3a2-109">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="0e3a2-110">Valitse **Käytäntötyyppi**, valitse **Windows 10 -laitteen määritys**.</span><span class="sxs-lookup"><span data-stu-id="0e3a2-110">Under **Policy type**, choose **Windows 10 Device Configuration**.</span></span>
    
5. <span data-ttu-id="0e3a2-p101">Laajenna **Suojatut Windows 10 -laitteet** \> määritä haluamasi asetukset. Lisätietoja on [Käytettävissä olevat asetukset](protection-settings-for-windows-10-pcs.md#bkmk_availablesettings) -kohdassa.</span><span class="sxs-lookup"><span data-stu-id="0e3a2-p101">Expand **Secure Windows 10 Devices** \> configure the settings how you would like. See [Available settings](protection-settings-for-windows-10-pcs.md#bkmk_availablesettings) for more information.</span></span> 
    
    <span data-ttu-id="0e3a2-113">Voit aina palauttaa oletusasetuksen **Palauta oletusasetukset** -linkin avulla.</span><span class="sxs-lookup"><span data-stu-id="0e3a2-113">You can alway use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. <span data-ttu-id="0e3a2-p102">Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja etsi käyttöoikeusryhmä, joka saa nämä asetukset \> **Valitse**.</span><span class="sxs-lookup"><span data-stu-id="0e3a2-p102">Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="0e3a2-117">Lopuksi tallenna käytäntö valitsemalla **Valmis** ja määritä se laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="0e3a2-117">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="0e3a2-118">Käytettävissä olevat asetukset</span><span class="sxs-lookup"><span data-stu-id="0e3a2-118">Available settings</span></span>

<span data-ttu-id="0e3a2-p103">Kaikki asetukset ovat oletusarvoisesti **käytössä**. Seuraavat asetukset ovat käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="0e3a2-p103">By default all settings are **On**. The following settings are available.</span></span>
  
<span data-ttu-id="0e3a2-121">Katso lisätietoja artikkelista [Miten Microsoft 365 Businessin suojausominaisuudet vastaavat Intunen asetuksia](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="0e3a2-121">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
|||
|:-----|:-----|
|<span data-ttu-id="0e3a2-122">Asetus</span><span class="sxs-lookup"><span data-stu-id="0e3a2-122">Setting</span></span>  <br/> |<span data-ttu-id="0e3a2-123">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="0e3a2-123">Description</span></span>  <br/> |
|<span data-ttu-id="0e3a2-124">Auta suojaamaan tietokoneitasi viruksilta ja muilta uhkilta käyttämällä Windows Defenderin virustentorjuntaa</span><span class="sxs-lookup"><span data-stu-id="0e3a2-124">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="0e3a2-125">Edellyttää, että Windows Defenderin virustentorjunta on otettu käyttöön suojaamaan tietokoneita Internetiin yhdistämisen vaaralta.</span><span class="sxs-lookup"><span data-stu-id="0e3a2-125">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="0e3a2-126">Suojaa tietokoneitasi verkkopohjaisilta uhkilta Microsoft Edgessä</span><span class="sxs-lookup"><span data-stu-id="0e3a2-126">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="0e3a2-127">Ottaa käyttöön Edgen asetukset, jotka auttavat suojaamaan käyttäjiä vahingollisilta sivustoilta ja latauksilta.</span><span class="sxs-lookup"><span data-stu-id="0e3a2-127">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="0e3a2-128">Käytä sääntöjä, jotka pienentävät laitteiden hyökkäyspinta-alaa</span><span class="sxs-lookup"><span data-stu-id="0e3a2-128">Use rules that reduce the attack surface of devices</span></span>  <br/> |<span data-ttu-id="0e3a2-p104">Kun tämä asetus käytössä, hyökkäyspinta-alan pienentäminen estää toiminnot ja sovellukset, joita haittaohjelmat yleensä käyttävät laitteiden saastuttamiseen. Tämä asetus on käytettävissä vain, jos Windows Defenderin virustentorjunta on käytössä. Lisätietoja on artikkelissa [Hyökkäyspinta-alan pienentäminen](https://go.microsoft.com/fwlink/?linkid=870417).  </span><span class="sxs-lookup"><span data-stu-id="0e3a2-p104">When turned On, attack surface reduction helps block actions and apps typically used by malware to infect devices. This setting is only available if Windows Defender Antivirus is set to On. See [Reduce attack surfaces](https://go.microsoft.com/fwlink/?linkid=870417) to learn more.  </span></span><br/> |
|<span data-ttu-id="0e3a2-132">Suojaa kansiot kiristysohjelmilta ja muilta uhilta</span><span class="sxs-lookup"><span data-stu-id="0e3a2-132">Protect folders from threats such as ransomware</span></span>  <br/> |<span data-ttu-id="0e3a2-p105">Tämä asetus hyödyntää hallittua kansioiden käyttöä, jolla yrityksen data suojataan epäilyttävien tai haitallisten sovellusten, kuten kiristysohjelmien, tekemiltä muutoksilta. Tällaisia sovelluksia estetään tekemästä muutoksia suojattuihin kansioihin. Tämä asetus on käytettävissä vain, jos Windows Defenderin virustentorjunta on käytössä. Lisätietoja on artikkelissa [Kansioiden suojaaminen hallitulla kansioiden käytöllä](https://go.microsoft.com/fwlink/?linkid=870418).  </span><span class="sxs-lookup"><span data-stu-id="0e3a2-p105">This setting uses controlled folder access to protect company data from modification by suspicious or malicious apps, such as ransomware. These types of apps are blocked from making changes in protected folders. This setting is only available if Windows Defender Antivirus is set to On. See [Protect folders with COntrolled folder access](https://go.microsoft.com/fwlink/?linkid=870418) to learn more.  </span></span><br/> |
|<span data-ttu-id="0e3a2-137">Estä potentiaalisesti haitallisen sisällön käyttäminen Internetissä</span><span class="sxs-lookup"><span data-stu-id="0e3a2-137">Prevent network access to potentially malicious content on the Internet</span></span>  <br/> |<span data-ttu-id="0e3a2-p106">Tämän asetuksen avulla voit estää lähtevän liikenteen käyttäjäyhteydet huonomaineisiin Internet-sijainteihin, jotka saattavat isännöidä tietojenkalasteluhuijauksia, heikkouksia hyödyntäviä ohjelmia tai muuta haitallista sisältöä. Tämä asetus on käytettävissä vain, jos Windows Defenderin virustentorjunta on käytössä. Lisätietoja on artikkelissa [Verkon suojaaminen](https://go.microsoft.com/fwlink/?linkid=870419).  </span><span class="sxs-lookup"><span data-stu-id="0e3a2-p106">Use this setting to block outbound user connections to low-reputation Internet locations that may host phishing scams, exploits or other malicious content. This setting is only available if Windows Defender Antivirus is set to On. See [Protect your network](https://go.microsoft.com/fwlink/?linkid=870419) for more information.  </span></span><br/> |
|<span data-ttu-id="0e3a2-141">Suojaa tietokoneiden tiedostot ja kansiot luvattomalta käytöltä BitLockerilla</span><span class="sxs-lookup"><span data-stu-id="0e3a2-141">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="0e3a2-p107">BitLocker suojaa datan salaamalla tietokoneen kiintolevyt ja estämällä sen joutumisen vääriin käsiin, jos tietokone katoaa tai varastetaan. Lisätietoja on artikkelissa [Bitlocker: usein kysytyt kysymykset](https://go.microsoft.com/fwlink/?linkid=871000).  </span><span class="sxs-lookup"><span data-stu-id="0e3a2-p107">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen. See [Bitlocker FAQ](https://go.microsoft.com/fwlink/?linkid=871000) for more information.  </span></span><br/> |
|<span data-ttu-id="0e3a2-144">Salli käyttäjille sovellusten lataaminen Microsoft Storesta</span><span class="sxs-lookup"><span data-stu-id="0e3a2-144">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="0e3a2-p108">Sallii käyttäjien ladata ja asentaa sovelluksia Microsoft Storesta. Sovellukset vaihtelevat peleistä tuottavuustyökaluihin, joten asetus on **käytössä**, mutta voit poistaa sen käytöstä lisäsuojausta varten.  </span><span class="sxs-lookup"><span data-stu-id="0e3a2-p108">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="0e3a2-147">Salli käyttäjien käyttää Cortanaa</span><span class="sxs-lookup"><span data-stu-id="0e3a2-147">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="0e3a2-p109">Cortana-toiminto voi olla hyvin hyödyllinen. Se voi ottaa puolestasi asetuksia käyttöön tai poistaa niitä käytöstä ja varmistaa, että ehdit ajoissa tapaamisiin, joten asetus on oletuksena **käytössä**.  </span><span class="sxs-lookup"><span data-stu-id="0e3a2-p109">Cortana can be very helpful! She can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this **On** by default.  </span></span><br/> |
|<span data-ttu-id="0e3a2-150">Salli käyttäjille Windows-vihjeiden ja -mainosten vastaanottaminen Microsoftilta</span><span class="sxs-lookup"><span data-stu-id="0e3a2-150">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="0e3a2-151">Windows-vihjeet voivat olla käteviä ja auttaa perehdyttämään käyttäjiä, kun uusia ominaisuuksia julkaistaan.</span><span class="sxs-lookup"><span data-stu-id="0e3a2-151">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="0e3a2-152">Pidä Windows 10 -laitteet ajan tasalla automaattisesti</span><span class="sxs-lookup"><span data-stu-id="0e3a2-152">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="0e3a2-153">Varmistaa, että Windows 10 -laitteet vastaanottavat automaattisesti päivityksiä.</span><span class="sxs-lookup"><span data-stu-id="0e3a2-153">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
|<span data-ttu-id="0e3a2-154">Sammuta laitteen näyttö, kun se on ollut käyttämättömänä tämän verran</span><span class="sxs-lookup"><span data-stu-id="0e3a2-154">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="0e3a2-p110">Varmistaa, että yritystiedot on suojattu, jos käyttäjä ei tee mitään. Käyttäjä saattaa työskennellä julkisessa paikassa, kuten kahvilassa, ja poistua tai kääntää huomion pois hetkeksi, jolloin laite on alttiina satunnaisille katseille. Tällä asetuksella voit määrittää, miten kauan käyttäjä voi olla toimettomana, ennen kuin näyttö pimenee.</span><span class="sxs-lookup"><span data-stu-id="0e3a2-p110">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
   
  

