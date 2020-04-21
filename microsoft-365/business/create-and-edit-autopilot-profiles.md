---
title: Autopilot-profiilien luominen ja muokkaaminen
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
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Opi luomaan AutoPilot-profiili ja ottamaan se käyttöön laitteessa sekä muokkaamaan tai poistamaan profiilia tai poistamaan profiili laitteesta.
ms.openlocfilehash: a6e02ab56faeb08718a9831657b55cff0356a4ec
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627370"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="41e2b-103">Autopilot-profiilien luominen ja muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="41e2b-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="41e2b-104">Uuden sähköpostiprofiilin luominen</span><span class="sxs-lookup"><span data-stu-id="41e2b-104">Create a profile</span></span>

<span data-ttu-id="41e2b-105">Profiilia käytetään laitteeseen tai laiteryhmään</span><span class="sxs-lookup"><span data-stu-id="41e2b-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="41e2b-106">Valitse Microsoft 365 -hallintakeskuksessa \> **Laitteet-automaattiohjaus**. **Devices**</span><span class="sxs-lookup"><span data-stu-id="41e2b-106">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="41e2b-107">Valitse **Automaattiohjaus-sivulla** **Profiilit-välilehti** \> **Luo profiili**.</span><span class="sxs-lookup"><span data-stu-id="41e2b-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="41e2b-108">Kirjoita **Luo profiili -sivulle** profiilin nimi, joka auttaa tunnistamaan profiilin, esimerkiksi Markkinointi.</span><span class="sxs-lookup"><span data-stu-id="41e2b-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing.</span></span> <span data-ttu-id="41e2b-109">Ota haluamasi asetus käyttöön ja valitse sitten **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="41e2b-109">Turn on the setting you want, and then choose **Save**.</span></span> <span data-ttu-id="41e2b-110">Lisätietoja automaattiohjauksen profiiliasetuksista on kohdassa [Tietoja autopilotin profiiliasetuksista](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="41e2b-110">For more information about AutoPilot profile settings, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="41e2b-112">Profiilin käyttäminen laitteeseen</span><span class="sxs-lookup"><span data-stu-id="41e2b-112">Apply profile to a device</span></span>

<span data-ttu-id="41e2b-113">Kun olet luonut profiilin, voit ottaa sen käyttöön laitteessa tai laiteryhmässä.</span><span class="sxs-lookup"><span data-stu-id="41e2b-113">After you create a profile, you can apply it to a device or a group of devices.</span></span> <span data-ttu-id="41e2b-114">Voit valita olemassa olevan profiilin [vaiheittaiset ohjeet](add-autopilot-devices-and-profile.md) ja ottaa sen käyttöön uusissa laitteissa tai korvata olemassa olevan profiilin laitteelle tai laiteryhmälle.</span><span class="sxs-lookup"><span data-stu-id="41e2b-114">You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md) and apply it to new devices, or replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="41e2b-115">Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="41e2b-115">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="41e2b-116">Valitse laitteen nimen vieressä oleva valintaruutu ja valitse **Laite-paneelin Avattavasta** **Määritetty profiili** \> -luettelosta **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="41e2b-116">Select the check box next to a device name, and in the **Device** panel, choose a profile from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="41e2b-118">Profiilin muokkaaminen tai poistaminen</span><span class="sxs-lookup"><span data-stu-id="41e2b-118">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="41e2b-p103">Kun olet määrittänyt profiilin laitteeseen, voit päivittää sen, vaikka olet jo antanut laitteen käyttäjälle. Kun laite muodostaa internet-yhteyden, se lataa profiilisi uusimman version asennuksen aikana. Jos käyttäjä palauttaa laitteen tehdasasetukset, laite lataa uudelleen profiilin uusimmat päivitykset.</span><span class="sxs-lookup"><span data-stu-id="41e2b-p103">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="41e2b-122">Profiilin muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="41e2b-122">Edit a profile</span></span>

1. <span data-ttu-id="41e2b-123">Valitse **Valmistele Windows** -sivulla **Profiilit**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="41e2b-123">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="41e2b-124">Valitse laitteen nimen vieressä oleva valintaruutu ja päivitä **Profiili-paneelissa** kaikki \> käytettävissä olevat asetukset **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="41e2b-124">Select the check box next to a device name, and in the **Profile** panel, update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="41e2b-125">Jos teet näin, ennen kuin käyttäjä yhdistää laitteen internetiin, profiilia käytetään asennuksessa.</span><span class="sxs-lookup"><span data-stu-id="41e2b-125">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="41e2b-126">Profiilin poistaminen</span><span class="sxs-lookup"><span data-stu-id="41e2b-126">Delete a profile</span></span>

1. <span data-ttu-id="41e2b-127">Valitse **Valmistele Windows** -sivulla **Profiilit**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="41e2b-127">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="41e2b-128">Valitse laitteen nimen vieressä oleva valintaruutu ja valitse **Profiili-paneelista** Poista **profiili** \> **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="41e2b-128">Select the check box next to a device name, and in the **Profile** panel, select **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="41e2b-129">Kun poistat profiilin, se poistetaan siitä laitteesta tai laiteryhmästä, johon se määritettiin.</span><span class="sxs-lookup"><span data-stu-id="41e2b-129">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="41e2b-130">Profiilin poistaminen</span><span class="sxs-lookup"><span data-stu-id="41e2b-130">Remove a profile</span></span>

1. <span data-ttu-id="41e2b-131">Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="41e2b-131">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="41e2b-132">Valitse laitteen nimen vieressä oleva valintaruutu ja valitse **Laite-paneelin Avattavasta** **Määritetty** profiili \> **-luettelosta**Ei **mitään.**</span><span class="sxs-lookup"><span data-stu-id="41e2b-132">Select the check box next to a device name, and in the **Device** panel, choose **None** from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
