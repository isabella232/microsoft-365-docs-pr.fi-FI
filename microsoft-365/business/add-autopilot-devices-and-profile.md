---
title: Autopilot-laitteiden ja -profiilien lisääminen vaiheittaisen ohjeen avulla
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Tietoja Windowsin automaattiohjauksen avulla voit määrittää yrityksellesi uuden Windows 10 laitteet.
ms.openlocfilehash: 8c4a14b4b9dcbf7a30c1e6e0bdd53418a1ab8a03
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660659"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="ea6c3-103">Autopilot-laitteiden ja -profiilien lisääminen vaiheittaisen ohjeen avulla</span><span class="sxs-lookup"><span data-stu-id="ea6c3-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="ea6c3-104">Windows automaattiohjauksen avulla voit määrittää **uuden** Windows 10-laitteiden yrityksesi niin, että ne ovat valmiita tuottavina käyttöön niin pian kuin ne antavat työntekijöille.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they are ready for productive use as soon as you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="ea6c3-105">Laitevaatimukset</span><span class="sxs-lookup"><span data-stu-id="ea6c3-105">Device requirements</span></span>

<span data-ttu-id="ea6c3-106">Laitteiden on täytettävä nämä vaatimukset:</span><span class="sxs-lookup"><span data-stu-id="ea6c3-106">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="ea6c3-107">Windows 10, versio 1703 tai uudempi.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-107">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="ea6c3-108">Uudet laitteet, joita ei ole määritetty Windowsin tervetuloa-ohjelmassa.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-108">New devices that have not been through Windows out-of-box experience.</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="ea6c3-109">Käytä laitteiden ja profiilien määritysopasta</span><span class="sxs-lookup"><span data-stu-id="ea6c3-109">Use the setup guide to create devices and profiles</span></span>

![Nauha, joka osoittaa https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="ea6c3-111">Jos sinulla ei ole vielä luotuna laiteryhmiä tai -profiileja, aloittaminen on helpointa vaiheittaisen oppaan avulla, mutta voit myös [lisätä laitteita](create-and-edit-autopilot-devices.md) ja [määrittää profiileja](create-and-edit-autopilot-profiles.md) käyttämättä opasta.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-111">If you have no device groups or profiles created yet, the best way to get started is by using the step-by-step guide, but you can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="ea6c3-112">Siirry hallintakeskukseen <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="ea6c3-113">Valitse vasemman nav **laitteet** \> **automaattiohjauksella**.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-113">On the left nav choose **Devices** \> **AutoPilot**.</span></span>

    ![Valitse laitteet ja automaattiohjauksen hallintakeskukseen.](media/AutoPilot.png)
  
2. <span data-ttu-id="ea6c3-115">**Automaattiohjauksen** sivulla Napsauta tai napauta **Käynnistä opas**.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-115">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="ea6c3-p101">Valitse **Lataa laiteluettelon sisältävä .csv-tiedosto** -sivulta sijainti, johon olet valmistellut .csv-tiedoston, ja valitse sitten **Avaa** \> **Seuraava**. Tiedostossa pitäisi olla kolme otsikkoa:</span><span class="sxs-lookup"><span data-stu-id="ea6c3-p101">On the **Upload .csv file with list of devices** page, browse to a locations where you have the prepared .CSV file, then **Open** \> **Next**. The file should have three headers:</span></span>
    
  - <span data-ttu-id="ea6c3-119">Sarake A: Laitteen sarjanumero</span><span class="sxs-lookup"><span data-stu-id="ea6c3-119">Column A: Device Serial Number</span></span>
    
  - <span data-ttu-id="ea6c3-120">Sarake B: Windows-tuotetunnus</span><span class="sxs-lookup"><span data-stu-id="ea6c3-120">Column B: Windows Product ID</span></span>
    
  - <span data-ttu-id="ea6c3-121">Sarake C: Laitteisto-hash</span><span class="sxs-lookup"><span data-stu-id="ea6c3-121">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="ea6c3-122">Saat nämä tiedot laitevalmistajalta tai voit käyttää PowerShell-komentosarjaa [Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), joka luo CSV-tiedoston.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-122">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a CSV file.</span></span> 
    
    <span data-ttu-id="ea6c3-p102">Katso lisätietoja [Laiteluettelon CSV-tiedostosta](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Voit myös ladata esimerkkitiedoston **Lataa laiteluettelon sisältävä .csv-tiedosto** -sivulta.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-p102">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="ea6c3-p103">Voit valita joko olemassa olevan profiilin **Profiilin määrittäminen** -sivulta tai luoda uuden profiilin. Jos sinulla ei ole vielä profiilia, ohjelma pyytää luomaan uuden.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-p103">On the **Assign a profile** page, you can either pick an existing profile, or create a new one. If you don't have one yet, you will be prompted to create a new one.</span></span> 
    
    <span data-ttu-id="ea6c3-127">Profiili on asetuskokoelma, jota voidaan soveltaa yksittäiseen laitteeseen tai laiteryhmään.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-127">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="ea6c3-p104">Oletusominaisuudet ovat pakolliset, ja ne määritetään automaattisesti. Oletusominaisuudet ovat:</span><span class="sxs-lookup"><span data-stu-id="ea6c3-p104">The default features are required and will be set automatically. The default features are:</span></span>
    
  - <span data-ttu-id="ea6c3-130">Cortana, OneDrive ja OEM-rekisteröinti ohitetaan.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-130">Cortana, OneDrive and OEM registration is skipped.</span></span>
    
  - <span data-ttu-id="ea6c3-131">Luo yrityskuvan mukainen kirjautumiskokemus.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-131">Create sign-in experience with your company brand.</span></span>
    
  - <span data-ttu-id="ea6c3-132">Laitteet yhdistetään Azure Active Directory -tileihin ja rekisteröidään automaattisesti Microsoft 365 Business:n hallinnoitavaksi.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-132">Your devices are going to be connected to Azure Active Directory accounts and automatically enrolled to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="ea6c3-133">Katso lisätietoja kohdasta</span><span class="sxs-lookup"><span data-stu-id="ea6c3-133">For more information, see</span></span>
    
    <span data-ttu-id="ea6c3-134">[Tietoja AutoPilot-profiilien asetuksista](autopilot-profile-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="ea6c3-134">[About AutoPilot Profile settings](autopilot-profile-settings.md) .</span></span> 
    
5. <span data-ttu-id="ea6c3-135">Toiset asetukset ovat **Ohita suojausasetukset** ja **Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi**. Nämä molemmat ovat oletusarvoisesti **Poissa käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="ea6c3-136">Valitse **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="ea6c3-p105">**Olet valmis** -sivu osoittaa, että luomaasi (tai valitsemaasi) sivua sovelletaan luomaasi laiteryhmään lataamalla laiteluettelo. Nämä asetukset ovat voimassa, kun laitteen käyttäjät kirjautuvat seuraavan kerran. Valitse **Sulje**.</span><span class="sxs-lookup"><span data-stu-id="ea6c3-p105">**You're done** page indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices. These settings will be in effect when the device users sign in next. Choose **Close**.</span></span>
    