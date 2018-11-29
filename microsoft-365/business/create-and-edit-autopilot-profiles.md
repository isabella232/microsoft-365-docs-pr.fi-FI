---
title: Autopilot-profiilien luominen ja muokkaaminen
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Lue, Luo, Muokkaa, poista tai poista profiileja automaattiohjauksella. '
ms.openlocfilehash: 4658a27e5f2c64a52f8a7d08b3fc13df5e239dc3
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983133"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="ffd72-103">Autopilot-profiilien luominen ja muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="ffd72-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="ffd72-104">Uuden sähköpostiprofiilin luominen</span><span class="sxs-lookup"><span data-stu-id="ffd72-104">Create a profile</span></span>

<span data-ttu-id="ffd72-105">Profiilia käytetään laitteeseen tai laiteryhmään</span><span class="sxs-lookup"><span data-stu-id="ffd72-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="ffd72-106">Valitse Microsoft 365 Businessin hallintakeskuksessa **Ota Windows käyttöön AutoPilotin avulla** **Laitetoiminnot**-kortista.</span><span class="sxs-lookup"><span data-stu-id="ffd72-106">In the Microsoft 365 Business Admin center, choose **Deploy Windows with AutoPilot** on the **Device actions** card.</span></span> 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="ffd72-108">Valitse **Valmistele Windows** -sivulla **Profiilit**-välilehti \> **Luo profiili**.</span><span class="sxs-lookup"><span data-stu-id="ffd72-108">On the **Prepare Windows** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="ffd72-109">Kirjoita **Luo profiili** -sivulla nimi, jonka avulla tunnistaa sen, kuten Markkinointi. Ota käyttöön haluamasi asetus (katso kohtaa [Tietoja AutoPilot-profiilien asetuksista](autopilot-profile-settings.md)) ja valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="ffd72-109">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing, turn on the setting you want (see [About AutoPilot Profile settings](autopilot-profile-settings.md) for more information), and choose **Save**.</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="ffd72-111">Profiilin käyttäminen laitteeseen</span><span class="sxs-lookup"><span data-stu-id="ffd72-111">Apply profile to a device</span></span>

<span data-ttu-id="ffd72-p101">Kun olet luonut profiilin, voit käyttää sitä laitteeseen tai laiteryhmään. Voit valita olemassa olevan profiilin [vaiheittaisten ohjeiden](add-autopilot-devices-and-profile.md) avulla, voit käyttää sitä uusiin laitteisiin tai voit korvata laitteen tai laiteryhmän olemassa olevan profiilin.</span><span class="sxs-lookup"><span data-stu-id="ffd72-p101">After you create a profile you can apply it to a device or a group of devices. You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md), you can apply it to new devices, or you can replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="ffd72-114">Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="ffd72-114">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="ffd72-115">Valitse valintaruutu laitteen nimen vierestä ja valitse **Laite**-paneeli. Valitse profiili avattavasta **Määritetty profiili** -valikosta \> **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="ffd72-115">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="ffd72-117">Profiilin muokkaaminen tai poistaminen</span><span class="sxs-lookup"><span data-stu-id="ffd72-117">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="ffd72-p102">Kun olet määrittänyt profiilin laitteeseen, voit päivittää sen, vaikka olet jo antanut laitteen käyttäjälle. Kun laite muodostaa internet-yhteyden, se lataa profiilisi uusimman version asennuksen aikana. Jos käyttäjä palauttaa laitteen tehdasasetukset, laite lataa uudelleen profiilin uusimmat päivitykset.</span><span class="sxs-lookup"><span data-stu-id="ffd72-p102">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="ffd72-121">Profiilin muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="ffd72-121">Edit a profile</span></span>

1. <span data-ttu-id="ffd72-122">Valitse **Valmistele Windows** -sivulla **Profiilit**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="ffd72-122">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="ffd72-123">Valitse valintaruutu laitteen nimen vierestä ja päivitä **Profiili**-paneelissa haluamasi asetukset \> **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="ffd72-123">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="ffd72-124">Jos teet näin, ennen kuin käyttäjä yhdistää laitteen internetiin, profiilia käytetään asennuksessa.</span><span class="sxs-lookup"><span data-stu-id="ffd72-124">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="ffd72-125">Profiilin poistaminen</span><span class="sxs-lookup"><span data-stu-id="ffd72-125">Delete a profile</span></span>

1. <span data-ttu-id="ffd72-126">Valitse **Valmistele Windows** -sivulla **Profiilit**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="ffd72-126">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="ffd72-127">Valitse valintaruutu laitteen nimen vierestä ja valitse **Profiili**-paneelissa **Poista profiili** \> **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="ffd72-127">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="ffd72-128">Kun poistat profiilin, se poistetaan siitä laitteesta tai laiteryhmästä, johon se määritettiin.</span><span class="sxs-lookup"><span data-stu-id="ffd72-128">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="ffd72-129">Profiilin poistaminen</span><span class="sxs-lookup"><span data-stu-id="ffd72-129">Remove a profile</span></span>

1. <span data-ttu-id="ffd72-130">Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="ffd72-130">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="ffd72-131">Valitse valintaruutu laitteen nimen vierestä ja valitse **Laite**-paneelissa **Ei mitään** avattavasta **Määritetty profiili** -valikosta \> **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="ffd72-131">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span></span>
    
