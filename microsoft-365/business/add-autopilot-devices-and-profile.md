---
title: Autopilot-laitteiden ja -profiilien lisääminen vaiheittaisen ohjeen avulla
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Opi käyttämään Windows AutoPilotia uusien Windows 10 yrityksesi kanssa, jotta ne ovat valmiina työntekijöiden käyttöön.
ms.openlocfilehash: e178e7df220e89605502d9ed400265bcd963e57e
ms.sourcegitcommit: 17f0aada83627d9defa0acf4db03a2d58e46842f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/24/2021
ms.locfileid: "52636102"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="066a1-103">Autopilot-laitteiden ja -profiilien lisääminen vaiheittaisen ohjeen avulla</span><span class="sxs-lookup"><span data-stu-id="066a1-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="066a1-104">Windows AutoPilotin avulla voit määrittää  uusia Windows 10-laitteita yrityksesi käyttöön, jotta ne ovat valmiita käytettäväksi, kun annat ne työntekijöillesi.</span><span class="sxs-lookup"><span data-stu-id="066a1-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="066a1-105">Laitevaatimukset</span><span class="sxs-lookup"><span data-stu-id="066a1-105">Device requirements</span></span>

<span data-ttu-id="066a1-106">Laitteiden on täytettävä seuraavat vaatimukset:</span><span class="sxs-lookup"><span data-stu-id="066a1-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="066a1-107">Windows 10, versio 1703 tai uudempi</span><span class="sxs-lookup"><span data-stu-id="066a1-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="066a1-108">Uudet laitteet, joita ei ole Windows käyttökokemusta</span><span class="sxs-lookup"><span data-stu-id="066a1-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="066a1-109">Käytä laitteiden ja profiilien määritysopasta</span><span class="sxs-lookup"><span data-stu-id="066a1-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="066a1-110">Jos et ole vielä luonut laiteryhmiä tai -profiileja, paras tapa päästä alkuun on käyttää vaiheittaista opasta.</span><span class="sxs-lookup"><span data-stu-id="066a1-110">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="066a1-111">Voit myös lisätä [laitteita ja](create-and-edit-autopilot-devices.md) [määrittää profiileja](create-and-edit-autopilot-profiles.md) niihin ilman opasta.</span><span class="sxs-lookup"><span data-stu-id="066a1-111">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="066a1-112">Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="066a1-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="066a1-113">Valitse vasemmassa siirtymisruudussa **Laitteet** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="066a1-113">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![Valitse hallintakeskuksessa laitteet ja valitse sitten AutoPilot.](../media/AutoPilot.png)
  
2. <span data-ttu-id="066a1-115">Napsauta **tai napauta AutoPilot-sivulla** **Aloitusopas**.</span><span class="sxs-lookup"><span data-stu-id="066a1-115">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="066a1-117">Siirry **Upload .csv, jossa on laiteluettelo** -sivulla sijaintiin, johon olet valmistellut .CSV ja valitse **sitten** \> **Avaa seuraava.**</span><span class="sxs-lookup"><span data-stu-id="066a1-117">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="066a1-118">Tiedostossa on oltava kolme otsikkoa:</span><span class="sxs-lookup"><span data-stu-id="066a1-118">The file must have three headers:</span></span>
    
    - <span data-ttu-id="066a1-119">Sarake A: Laitteen sarjanumero</span><span class="sxs-lookup"><span data-stu-id="066a1-119">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="066a1-120">Sarake B: Windows-tuotetunnus</span><span class="sxs-lookup"><span data-stu-id="066a1-120">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="066a1-121">Sarake C: Laitteisto-hash</span><span class="sxs-lookup"><span data-stu-id="066a1-121">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="066a1-122">Saat nämä tiedot laitteiston toimittajalta tai voit luoda [CSV-tiedoston Käyttämällä PowerShell-komentosarjaa Get-WindowsAutoPilotInfo.](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo)</span><span class="sxs-lookup"><span data-stu-id="066a1-122">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="066a1-p103">Katso lisätietoja [Laiteluettelon CSV-tiedostosta](../admin/misc/device-list.md). Voit myös ladata esimerkkitiedoston **Lataa laiteluettelon sisältävä .csv-tiedosto** -sivulta.</span><span class="sxs-lookup"><span data-stu-id="066a1-p103">For more information, see [Device list CSV-file](../admin/misc/device-list.md). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="066a1-125">Tämä komentosarja noutaa WMI:n avulla ominaisuuksia, joita asiakas tarvitsee laitteen rekisteröimiseen Autopilotin Windows kanssa.</span><span class="sxs-lookup"><span data-stu-id="066a1-125">This script uses WMI to retrieve properties needed for a customer to register a device with Windows Autopilot.</span></span> <span data-ttu-id="066a1-126">Huomaa, että tuloksena syntyvä CSV-tiedosto ei tavallisesti kerää Windows Product ID (PKID) -arvoa, koska tätä ei tarvita laitteen rekisteröimiseen, ja PKID on tyhjäarvoinen CSV-tulostetiedostossa.</span><span class="sxs-lookup"><span data-stu-id="066a1-126">Note that it is normal for the resulting CSV file to not collect a Windows Product ID (PKID) value since this is not required to register a device and PKID being NULL in the output CSV is totally fine.</span></span> <span data-ttu-id="066a1-127">Vain sarjanumero ja laitteiston hash täytetään.</span><span class="sxs-lookup"><span data-stu-id="066a1-127">Only the serial number and hardware hash will be populated.</span></span>
    
4. <span data-ttu-id="066a1-128">Profiilin **määrittäminen -sivulla** voit joko valita olemassa olevan profiilin tai luoda uuden.</span><span class="sxs-lookup"><span data-stu-id="066a1-128">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="066a1-129">Jos sinulla ei vielä ole sitä, sinua pyydetään luomaan sellainen.</span><span class="sxs-lookup"><span data-stu-id="066a1-129">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="066a1-130">Profiili on asetuskokoelma, jota voidaan soveltaa yksittäiseen laitteeseen tai laiteryhmään.</span><span class="sxs-lookup"><span data-stu-id="066a1-130">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="066a1-131">Oletusominaisuudet ovat pakollisia, ja ne määritetään automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="066a1-131">The default features are required and are set automatically.</span></span> <span data-ttu-id="066a1-132">Oletusominaisuudet ovat:</span><span class="sxs-lookup"><span data-stu-id="066a1-132">The default features are:</span></span>
    
    - <span data-ttu-id="066a1-133">Ohita Cortana, OneDrive ja OEM-rekisteröinti.</span><span class="sxs-lookup"><span data-stu-id="066a1-133">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="066a1-134">Luo yrityskuvan mukainen kirjautumiskokemus.</span><span class="sxs-lookup"><span data-stu-id="066a1-134">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="066a1-135">Näyttöyhteys laitteet ja Azure Active Directory tilit ja rekisteröi ne automaattisesti hallinnoitavaksi Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="066a1-135">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business Premium.</span></span>
    
    <span data-ttu-id="066a1-136">Lisätietoja on kohdassa Tietoja [AutoPilot-profiilin asetuksista.](autopilot-profile-settings.md)</span><span class="sxs-lookup"><span data-stu-id="066a1-136">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="066a1-137">Toiset asetukset ovat **Ohita suojausasetukset** ja **Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi**. Nämä molemmat ovat oletusarvoisesti **Poissa käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="066a1-137">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="066a1-138">Valitse **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="066a1-138">Choose **Next**.</span></span>
    
6. <span data-ttu-id="066a1-139">**Kun olet valmis,** luomaasi (tai valitsemaasi) profiilia käytetään luomaasi laiteryhmään lataamalla laiteluettelo.</span><span class="sxs-lookup"><span data-stu-id="066a1-139">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="066a1-140">Asetukset ovat voimassa, kun laitteen käyttäjät kirjautuvat seuraavan kerran.</span><span class="sxs-lookup"><span data-stu-id="066a1-140">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="066a1-141">Valitse **Sulje**.</span><span class="sxs-lookup"><span data-stu-id="066a1-141">Choose **Close**.</span></span>

## <a name="related-content"></a><span data-ttu-id="066a1-142">Aiheeseen liittyvä sisältö</span><span class="sxs-lookup"><span data-stu-id="066a1-142">Related content</span></span>

<span data-ttu-id="066a1-143">[Tietoja AutoPilot-profiilin asetuksista](autopilot-profile-settings.md) (artikkeli)</span><span class="sxs-lookup"><span data-stu-id="066a1-143">[About AutoPilot Profile settings](autopilot-profile-settings.md) (article)</span></span>\
<span data-ttu-id="066a1-144">[Laitteiden ja sovellustietojen suojaamista koskevat vaihtoehdot](../admin/devices/choose-device-security.md) (artikkeli)</span><span class="sxs-lookup"><span data-stu-id="066a1-144">[Options for protecting your devices and app data](../admin/devices/choose-device-security.md) (article)</span></span>
