---
title: Autopilot-profiilien luominen ja muokkaaminen
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Lue, Luo, Muokkaa, poista tai poista profiileja automaattiohjauksella. '
ms.openlocfilehash: 85fc897b2f428afae8d55feeb577021adaa30f72
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277097"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="6f64d-103">Autopilot-profiilien luominen ja muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="6f64d-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="6f64d-104">Uuden sähköpostiprofiilin luominen</span><span class="sxs-lookup"><span data-stu-id="6f64d-104">Create a profile</span></span>

<span data-ttu-id="6f64d-105">Profiilia käytetään laitteeseen tai laiteryhmään</span><span class="sxs-lookup"><span data-stu-id="6f64d-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="6f64d-106">Valitse Microsoft 365 Business hallintakeskukseen, **laitteiden** \> **automaattiohjauksella**.</span><span class="sxs-lookup"><span data-stu-id="6f64d-106">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="6f64d-107">Valitse **profiilit** -välilehti **automaattiohjauksella** , sivulla \> **Luo profiili**.</span><span class="sxs-lookup"><span data-stu-id="6f64d-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="6f64d-108">Kirjoita **Luo profiili** -sivulla nimi, jonka avulla tunnistaa sen, kuten Markkinointi. Ota käyttöön haluamasi asetus (katso kohtaa [Tietoja AutoPilot-profiilien asetuksista](autopilot-profile-settings.md)) ja valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="6f64d-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing, turn on the setting you want (see [About AutoPilot Profile settings](autopilot-profile-settings.md) for more information), and choose **Save**.</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="6f64d-110">Profiilin käyttäminen laitteeseen</span><span class="sxs-lookup"><span data-stu-id="6f64d-110">Apply profile to a device</span></span>

<span data-ttu-id="6f64d-p101">Kun olet luonut profiilin, voit käyttää sitä laitteeseen tai laiteryhmään. Voit valita olemassa olevan profiilin [vaiheittaisten ohjeiden](add-autopilot-devices-and-profile.md) avulla, voit käyttää sitä uusiin laitteisiin tai voit korvata laitteen tai laiteryhmän olemassa olevan profiilin.</span><span class="sxs-lookup"><span data-stu-id="6f64d-p101">After you create a profile you can apply it to a device or a group of devices. You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md), you can apply it to new devices, or you can replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="6f64d-113">Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="6f64d-113">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="6f64d-114">Valitse valintaruutu laitteen nimen vierestä ja valitse **Laite**-paneeli. Valitse profiili avattavasta **Määritetty profiili** -valikosta \> **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="6f64d-114">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="6f64d-116">Profiilin muokkaaminen tai poistaminen</span><span class="sxs-lookup"><span data-stu-id="6f64d-116">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="6f64d-p102">Kun olet määrittänyt profiilin laitteeseen, voit päivittää sen, vaikka olet jo antanut laitteen käyttäjälle. Kun laite muodostaa internet-yhteyden, se lataa profiilisi uusimman version asennuksen aikana. Jos käyttäjä palauttaa laitteen tehdasasetukset, laite lataa uudelleen profiilin uusimmat päivitykset.</span><span class="sxs-lookup"><span data-stu-id="6f64d-p102">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="6f64d-120">Profiilin muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="6f64d-120">Edit a profile</span></span>

1. <span data-ttu-id="6f64d-121">Valitse **Valmistele Windows** -sivulla **Profiilit**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="6f64d-121">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="6f64d-122">Valitse valintaruutu laitteen nimen vierestä ja päivitä **Profiili**-paneelissa haluamasi asetukset \> **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="6f64d-122">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="6f64d-123">Jos teet näin, ennen kuin käyttäjä yhdistää laitteen internetiin, profiilia käytetään asennuksessa.</span><span class="sxs-lookup"><span data-stu-id="6f64d-123">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="6f64d-124">Profiilin poistaminen</span><span class="sxs-lookup"><span data-stu-id="6f64d-124">Delete a profile</span></span>

1. <span data-ttu-id="6f64d-125">Valitse **Valmistele Windows** -sivulla **Profiilit**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="6f64d-125">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="6f64d-126">Valitse valintaruutu laitteen nimen vierestä ja valitse **Profiili**-paneelissa **Poista profiili** \> **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="6f64d-126">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="6f64d-127">Kun poistat profiilin, se poistetaan siitä laitteesta tai laiteryhmästä, johon se määritettiin.</span><span class="sxs-lookup"><span data-stu-id="6f64d-127">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="6f64d-128">Profiilin poistaminen</span><span class="sxs-lookup"><span data-stu-id="6f64d-128">Remove a profile</span></span>

1. <span data-ttu-id="6f64d-129">Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="6f64d-129">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="6f64d-130">Valitse valintaruutu laitteen nimen vierestä ja valitse **Laite**-paneelissa **Ei mitään** avattavasta **Määritetty profiili** -valikosta \> **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="6f64d-130">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span></span>
    
