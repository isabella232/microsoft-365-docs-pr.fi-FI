---
title: Autopilot-laitteiden ja -profiilien lisääminen vaiheittaisen ohjeen avulla
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Lue, miten voit määrittää uusia Windows 10 -laitteita yrityksellesi Windowsin automaattiohjauksen avulla.
ms.openlocfilehash: e5774b1e2079a5249e0f6e9e7142de19268253b5
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2020
ms.locfileid: "42068525"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="86e97-103">Autopilot-laitteiden ja -profiilien lisääminen vaiheittaisen ohjeen avulla</span><span class="sxs-lookup"><span data-stu-id="86e97-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="86e97-104">Windowsin automaattiohjauksen avulla voit määrittää **yrityksellesi uusia** Windows 10 -laitteita, jotta ne ovat käyttövalmiita, kun annat ne työntekijöillesi.</span><span class="sxs-lookup"><span data-stu-id="86e97-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="86e97-105">Laitevaatimukset</span><span class="sxs-lookup"><span data-stu-id="86e97-105">Device requirements</span></span>

<span data-ttu-id="86e97-106">Laitteiden on täytettävä seuraavat vaatimukset:</span><span class="sxs-lookup"><span data-stu-id="86e97-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="86e97-107">Windows 10, versio 1703 tai uudempi</span><span class="sxs-lookup"><span data-stu-id="86e97-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="86e97-108">Uudet laitteet, jotka eivät ole käyneet Windowsin kautta.</span><span class="sxs-lookup"><span data-stu-id="86e97-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="86e97-109">Käytä laitteiden ja profiilien määritysopasta</span><span class="sxs-lookup"><span data-stu-id="86e97-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="86e97-110">[![Selite, jossa ilmoitetaan, että hallintakeskus muuttuu. Lisätietoja löytyy osoitteesta aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="86e97-110">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="86e97-111">Jos et ole vielä luonut laiteryhmiä tai profiileja, paras tapa aloittaa vaiheittaiset ohjeet vaiheittaiset ohjeet.</span><span class="sxs-lookup"><span data-stu-id="86e97-111">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="86e97-112">Voit myös [lisätä laitteita](create-and-edit-autopilot-devices.md) ja määrittää niihin [profiileja](create-and-edit-autopilot-profiles.md) käyttämättä opasta.</span><span class="sxs-lookup"><span data-stu-id="86e97-112">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="86e97-113">Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="86e97-113">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="86e97-114">Valitse vasemmasta siirtymisruudusta **Laitteet** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="86e97-114">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![Valitse hallintakeskuksessa laitteet ja sitten Automaattinen ohjaus.](../media/AutoPilot.png)
  
2. <span data-ttu-id="86e97-116">Valitse **AutoPilot-sivulla** **Aloitusopas**.</span><span class="sxs-lookup"><span data-stu-id="86e97-116">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="86e97-118">Siirry **Lataa .csv-tiedosto laiteluettelolla** -sivulla sijaintiin, jossa olet valmistellut . CSV-tiedosto ja sitten **Avaa** \> **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="86e97-118">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="86e97-119">Tiedostossa on oltava kolme otsikkoa:</span><span class="sxs-lookup"><span data-stu-id="86e97-119">The file must have three headers:</span></span>
    
    - <span data-ttu-id="86e97-120">Sarake A: Laitteen sarjanumero</span><span class="sxs-lookup"><span data-stu-id="86e97-120">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="86e97-121">Sarake B: Windows-tuotetunnus</span><span class="sxs-lookup"><span data-stu-id="86e97-121">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="86e97-122">Sarake C: Laitteisto-hash</span><span class="sxs-lookup"><span data-stu-id="86e97-122">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="86e97-123">Saat nämä tiedot laitteiston toimittajalta tai voit luoda [CSV-tiedoston Get-WindowsAutoPilotInfo PowerShell -komentosarjan](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) avulla.</span><span class="sxs-lookup"><span data-stu-id="86e97-123">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="86e97-p103">Katso lisätietoja [Laiteluettelon CSV-tiedostosta](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Voit myös ladata esimerkkitiedoston **Lataa laiteluettelon sisältävä .csv-tiedosto** -sivulta.</span><span class="sxs-lookup"><span data-stu-id="86e97-p103">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="86e97-126">Määritä **profiili** -sivulla voit joko valita aiemmin luodun profiilin tai luoda uuden profiilin.</span><span class="sxs-lookup"><span data-stu-id="86e97-126">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="86e97-127">Jos sinulla ei vielä ole sellaista, sinua pyydetään luomaan sellainen.</span><span class="sxs-lookup"><span data-stu-id="86e97-127">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="86e97-128">Profiili on asetuskokoelma, jota voidaan soveltaa yksittäiseen laitteeseen tai laiteryhmään.</span><span class="sxs-lookup"><span data-stu-id="86e97-128">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="86e97-129">Oletusominaisuudet ovat pakollisia, ja ne määritetään automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="86e97-129">The default features are required and are set automatically.</span></span> <span data-ttu-id="86e97-130">Oletusominaisuudet ovat:</span><span class="sxs-lookup"><span data-stu-id="86e97-130">The default features are:</span></span>
    
    - <span data-ttu-id="86e97-131">Ohita Cortanan, OneDriven ja OEM-laitevalmistajan rekisteröinti.</span><span class="sxs-lookup"><span data-stu-id="86e97-131">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="86e97-132">Luo yrityskuvan mukainen kirjautumiskokemus.</span><span class="sxs-lookup"><span data-stu-id="86e97-132">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="86e97-133">Yhdistä laitteesi Azure Active Directory -tileihin ja rekisteröi ne automaattisesti Microsoft 365 Businessin hallinnoimiksi.</span><span class="sxs-lookup"><span data-stu-id="86e97-133">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="86e97-134">Lisätietoja on kohdassa [Tietoja autopilotin profiiliasetuksista](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="86e97-134">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="86e97-135">Toiset asetukset ovat **Ohita suojausasetukset** ja **Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi**. Nämä molemmat ovat oletusarvoisesti **Poissa käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="86e97-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="86e97-136">Valitse **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="86e97-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="86e97-137">**Olet valmis,** osoittaa, että luomasi (tai valitsemasi profiili) otetaan käyttöön luomassasi laiteryhmässä lataamalla laiteluettelo.</span><span class="sxs-lookup"><span data-stu-id="86e97-137">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="86e97-138">Asetukset tulevat voimaan, kun laitteen käyttäjät kirjautuvat sisään seuraavaksi.</span><span class="sxs-lookup"><span data-stu-id="86e97-138">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="86e97-139">Valitse **Sulje**.</span><span class="sxs-lookup"><span data-stu-id="86e97-139">Choose **Close**.</span></span>
    
