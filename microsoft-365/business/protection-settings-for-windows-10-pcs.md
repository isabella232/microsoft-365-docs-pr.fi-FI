---
title: Laitteiden suojausasetusten määrittäminen Windows 10 -tietokoneita varten
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
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Lue lisä tietoja Microsoft 365 Businessin oletus arvoista ja muista asetuksista Windows 10-laitteiden turvaamiseksi.
ms.openlocfilehash: 5d4bce02df1276dc9b284c7b0709c7dc26b0dbce
ms.sourcegitcommit: 8ca97fa879ae4ea44468be629d6c32b429efeeec
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/16/2019
ms.locfileid: "38676044"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a><span data-ttu-id="71424-103">Laitteiden suojausasetusten määrittäminen Windows 10 -tietokoneita varten</span><span class="sxs-lookup"><span data-stu-id="71424-103">Set device protection settings for Windows 10 PCs</span></span>

## <a name="secure-windows-10-devices"></a><span data-ttu-id="71424-104">Suojatut Windows 10 -laitteet</span><span class="sxs-lookup"><span data-stu-id="71424-104">Secure Windows 10 devices</span></span>

<span data-ttu-id="71424-105">Katso video Windows 10 -laitteiden suojaamisesta Microsoft 365 Businessin avulla:</span><span class="sxs-lookup"><span data-stu-id="71424-105">View a video on how to secure Windows 10 devices with Microsoft 365 Business:</span></span>
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. <span data-ttu-id="71424-106">Siirry hallinta keskukseen-kohtaan <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="71424-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="71424-107">Valitse vasemmasta siirtymis kohdasta **laite** \> **käytännöt** \> - **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="71424-107">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="71424-108">Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle.</span><span class="sxs-lookup"><span data-stu-id="71424-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="71424-109">Valitse **Käytäntötyyppi**, valitse **Windows 10 -laitteen määritys**.</span><span class="sxs-lookup"><span data-stu-id="71424-109">Under **Policy type**, choose **Windows 10 Device Configuration**.</span></span>
    
5. <span data-ttu-id="71424-p101">Laajenna **Suojatut Windows 10 -laitteet** \> määritä haluamasi asetukset. Lisätietoja on [Käytettävissä olevat asetukset](#available-settings) -kohdassa.</span><span class="sxs-lookup"><span data-stu-id="71424-p101">Expand **Secure Windows 10 Devices** \> configure the settings how you would like. See [Available settings](#available-settings) for more information.</span></span> 
    
    <span data-ttu-id="71424-112">Voit aina palauttaa oletusasetuksen **Palauta oletusasetukset** -linkin avulla.</span><span class="sxs-lookup"><span data-stu-id="71424-112">You can alway use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. <span data-ttu-id="71424-p102">Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja etsi käyttöoikeusryhmä, joka saa nämä asetukset \> **Valitse**.</span><span class="sxs-lookup"><span data-stu-id="71424-p102">Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="71424-116">Lopuksi tallenna käytäntö valitsemalla **Valmis** ja määritä se laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="71424-116">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="71424-117">Käytettävissä olevat asetukset</span><span class="sxs-lookup"><span data-stu-id="71424-117">Available settings</span></span>

<span data-ttu-id="71424-p103">Kaikki asetukset ovat oletusarvoisesti **käytössä**. Seuraavat asetukset ovat käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="71424-p103">By default all settings are **On**. The following settings are available.</span></span>
  
<span data-ttu-id="71424-120">Katso lisätietoja artikkelista [Miten Microsoft 365 Businessin suojausominaisuudet vastaavat Intunen asetuksia](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="71424-120">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
|||
|:-----|:-----|
|<span data-ttu-id="71424-121">Asetus</span><span class="sxs-lookup"><span data-stu-id="71424-121">Setting</span></span>  <br/> |<span data-ttu-id="71424-122">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="71424-122">Description</span></span>  <br/> |
|<span data-ttu-id="71424-123">Auta suojaamaan tietokoneitasi viruksilta ja muilta uhkilta käyttämällä Windows Defenderin virustenorjuntaa</span><span class="sxs-lookup"><span data-stu-id="71424-123">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="71424-124">Edellyttää, että Windows Defenderin virustentorjunta on otettu käyttöön suojaamaan tietokoneita Internetiin yhdistämisen vaaralta.</span><span class="sxs-lookup"><span data-stu-id="71424-124">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="71424-125">Auta suojaamaan tietokoneitasi verkkopohjaisilta uhkilta Microsoft Edgessä</span><span class="sxs-lookup"><span data-stu-id="71424-125">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="71424-126">Ottaa käyttöön Edgen asetukset, jotka auttavat suojaamaan käyttäjiä vahingollisilta sivustoilta ja latauksilta.</span><span class="sxs-lookup"><span data-stu-id="71424-126">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="71424-127">Käytä sääntöjä, jotka pienentävät laitteiden hyökkäyspinta-alaa</span><span class="sxs-lookup"><span data-stu-id="71424-127">Use rules that reduce the attack surface of devices</span></span>  <br/> |<span data-ttu-id="71424-p104">Kun tämä asetus käytössä, hyökkäyspinta-alan pienentäminen estää toiminnot ja sovellukset, joita haittaohjelmat yleensä käyttävät laitteiden saastuttamiseen. Tämä asetus on käytettävissä vain, jos Windows Defenderin virustentorjunta on käytössä. Lisätietoja on artikkelissa [Hyökkäyspinta-alan pienentäminen](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/exploit-protection).  </span><span class="sxs-lookup"><span data-stu-id="71424-p104">When turned On, attack surface reduction helps block actions and apps typically used by malware to infect devices. This setting is only available if Windows Defender Antivirus is set to On. See [Reduce attack surfaces](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/exploit-protection) to learn more.  </span></span><br/> |
|<span data-ttu-id="71424-131">Suojaa kansiot kiristysohjelmilta ja muilta uhilta</span><span class="sxs-lookup"><span data-stu-id="71424-131">Protect folders from threats such as ransomware</span></span>  <br/> |<span data-ttu-id="71424-132">Tämä asetus hyödyntää hallittua kansioiden käyttöä, jolla yrityksen data suojataan epäilyttävien tai haitallisten sovellusten, kuten kiristysohjelmien, tekemiltä muutoksilta.</span><span class="sxs-lookup"><span data-stu-id="71424-132">This setting uses controlled folder access to protect company data from modification by suspicious or malicious apps, such as ransomware.</span></span> <span data-ttu-id="71424-133">Tällaisia sovelluksia estetään tekemästä muutoksia suojattuihin kansioihin.</span><span class="sxs-lookup"><span data-stu-id="71424-133">These types of apps are blocked from making changes in protected folders.</span></span> <span data-ttu-id="71424-134">Tämä asetus on käytettävissä vain, jos Windows Defenderin virustentorjunta on käytössä.</span><span class="sxs-lookup"><span data-stu-id="71424-134">This setting is only available if Windows Defender Antivirus is set to On.</span></span> <span data-ttu-id="71424-135">Lisä tietoja [on artikkelissa kansioiden suojaaminen hallitusti kansio-käyttö oikeudet-](https://docs.microsoft.com/configmgr/protect/deploy-use/create-deploy-exploit-guard-policy#bkmk_CFA) kohdassa.</span><span class="sxs-lookup"><span data-stu-id="71424-135">See [Protect folders with Controlled folder access](https://docs.microsoft.com/configmgr/protect/deploy-use/create-deploy-exploit-guard-policy#bkmk_CFA) to learn more.</span></span>  <br/> |
|<span data-ttu-id="71424-136">Estä potentiaalisesti haitallisen sisällön käyttäminen Internetissä</span><span class="sxs-lookup"><span data-stu-id="71424-136">Prevent network access to potentially malicious content on the Internet</span></span>  <br/> |<span data-ttu-id="71424-p106">Tämän asetuksen avulla voit estää lähtevän liikenteen käyttäjäyhteydet huonomaineisiin Internet-sijainteihin, jotka saattavat isännöidä tietojenkalasteluhuijauksia, heikkouksia hyödyntäviä ohjelmia tai muuta haitallista sisältöä. Tämä asetus on käytettävissä vain, jos Windows Defenderin virustentorjunta on käytössä. Lisätietoja on artikkelissa [Verkon suojaaminen](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/configure-real-time-protection-windows-defender-antivirus).  </span><span class="sxs-lookup"><span data-stu-id="71424-p106">Use this setting to block outbound user connections to low-reputation Internet locations that may host phishing scams, exploits or other malicious content. This setting is only available if Windows Defender Antivirus is set to On. See [Protect your network](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/configure-real-time-protection-windows-defender-antivirus) for more information.  </span></span><br/> |
|<span data-ttu-id="71424-140">Suojaa tietokoneiden tiedostot ja kansiot luvattomalta käytöltä BitLockerilla</span><span class="sxs-lookup"><span data-stu-id="71424-140">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="71424-p107">BitLocker suojaa datan salaamalla tietokoneen kiintolevyt ja estämällä sen joutumisen vääriin käsiin, jos tietokone katoaa tai varastetaan. Lisätietoja on artikkelissa [Bitlocker: usein kysytyt kysymykset](https://go.microsoft.com/fwlink/?linkid=871000).  </span><span class="sxs-lookup"><span data-stu-id="71424-p107">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen. See [Bitlocker FAQ](https://go.microsoft.com/fwlink/?linkid=871000) for more information.  </span></span><br/> |
|<span data-ttu-id="71424-143">Salli käyttäjille sovellusten lataaminen Microsoft Storesta</span><span class="sxs-lookup"><span data-stu-id="71424-143">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="71424-p108">Sallii käyttäjien ladata ja asentaa sovelluksia Microsoft Storesta. Sovellukset vaihtelevat peleistä tuottavuustyökaluihin, joten asetus on **käytössä**, mutta voit poistaa sen käytöstä lisäsuojausta varten.  </span><span class="sxs-lookup"><span data-stu-id="71424-p108">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="71424-146">Salli käyttäjien käyttää Cortanaa</span><span class="sxs-lookup"><span data-stu-id="71424-146">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="71424-p109">Cortana-toiminto voi olla hyvin hyödyllinen. Se voi ottaa puolestasi asetuksia käyttöön tai poistaa niitä käytöstä ja varmistaa, että ehdit ajoissa tapaamisiin, joten asetus on oletuksena **käytössä**.  </span><span class="sxs-lookup"><span data-stu-id="71424-p109">Cortana can be very helpful! She can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this **On** by default.  </span></span><br/> |
|<span data-ttu-id="71424-149">Salli käyttäjille Windows-vihjeiden ja -mainosten vastaanottaminen Microsoftilta</span><span class="sxs-lookup"><span data-stu-id="71424-149">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="71424-150">Windows-vihjeet voivat olla käteviä ja auttaa perehdyttämään käyttäjiä, kun uusia ominaisuuksia julkaistaan.</span><span class="sxs-lookup"><span data-stu-id="71424-150">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="71424-151">Pidä Windows 10 -laitteet ajan tasalla automaattisesti</span><span class="sxs-lookup"><span data-stu-id="71424-151">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="71424-152">Varmistaa, että Windows 10 -laitteet vastaanottavat automaattisesti päivityksiä.</span><span class="sxs-lookup"><span data-stu-id="71424-152">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
|<span data-ttu-id="71424-153">Sammuta laitteen näyttö, kun se on ollut käyttämättömänä tämän verran</span><span class="sxs-lookup"><span data-stu-id="71424-153">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="71424-p110">Varmistaa, että yritystiedot on suojattu, jos käyttäjä ei tee mitään. Käyttäjä saattaa työskennellä julkisessa paikassa, kuten kahvilassa, ja poistua tai kääntää huomion pois hetkeksi, jolloin laite on alttiina satunnaisille katseille. Tällä asetuksella voit määrittää, miten kauan käyttäjä voi olla toimettomana, ennen kuin näyttö pimenee.</span><span class="sxs-lookup"><span data-stu-id="71424-p110">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
   
  

