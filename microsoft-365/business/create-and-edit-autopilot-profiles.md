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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Opi luomaan, muokkaamaan, poistamaan tai poistamaan automaatti ohjauksen profiileja.
ms.openlocfilehash: 35967cb1f6e2cdeea9d7c42a529526410fa8b586
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593987"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="26d5a-103">Autopilot-profiilien luominen ja muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="26d5a-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="26d5a-104">Uuden sähköpostiprofiilin luominen</span><span class="sxs-lookup"><span data-stu-id="26d5a-104">Create a profile</span></span>

<span data-ttu-id="26d5a-105">Profiilia käytetään laitteeseen tai laiteryhmään</span><span class="sxs-lookup"><span data-stu-id="26d5a-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="26d5a-106">Valitse Microsoft 365 Business-hallinta keskuksessa **laitteet** \> - **automaatti ohjaus**.</span><span class="sxs-lookup"><span data-stu-id="26d5a-106">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="26d5a-107">Valitse **automaatti ohjaus** -sivulla **Profiilit** -väli lehti \> **Luo profiili**.</span><span class="sxs-lookup"><span data-stu-id="26d5a-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="26d5a-108">Kirjoita **Luo profiili** -sivulla sen profiilin nimi, joka auttaa tunnistamaan sen, esimerkiksi markkinointi.</span><span class="sxs-lookup"><span data-stu-id="26d5a-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing.</span></span> <span data-ttu-id="26d5a-109">Ota haluamasi asetus käyttöön ja valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="26d5a-109">Turn on the setting you want, and then choose **Save**.</span></span> <span data-ttu-id="26d5a-110">Lisä tietoja automaatti ohjauksen profiili asetuksista on kohdassa [tietoja automaatti ohjauksen profiili asetuksista](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="26d5a-110">For more information about AutoPilot profile settings, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="26d5a-112">Profiilin käyttäminen laitteeseen</span><span class="sxs-lookup"><span data-stu-id="26d5a-112">Apply profile to a device</span></span>

<span data-ttu-id="26d5a-113">Kun olet luonut profiilin, voit käyttää sitä laitteessa tai laite ryhmässä.</span><span class="sxs-lookup"><span data-stu-id="26d5a-113">After you create a profile, you can apply it to a device or a group of devices.</span></span> <span data-ttu-id="26d5a-114">Voit valita olemassa olevan profiilin [vaiheittainen opas](add-autopilot-devices-and-profile.md) ja käyttää sitä uusiin laitteisiin tai korvata olemassa olevan profiilin laitteelle tai laite ryhmälle.</span><span class="sxs-lookup"><span data-stu-id="26d5a-114">You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md) and apply it to new devices, or replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="26d5a-115">Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="26d5a-115">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="26d5a-116">Valitse laitteen nimen vieressä oleva valinta ruutu ja valitse **laite** -paneelista profiili avattavasta **määritetty profiili** -luettelosta \> **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="26d5a-116">Select the check box next to a device name, and in the **Device** panel, choose a profile from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="26d5a-118">Profiilin muokkaaminen tai poistaminen</span><span class="sxs-lookup"><span data-stu-id="26d5a-118">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="26d5a-p103">Kun olet määrittänyt profiilin laitteeseen, voit päivittää sen, vaikka olet jo antanut laitteen käyttäjälle. Kun laite muodostaa internet-yhteyden, se lataa profiilisi uusimman version asennuksen aikana. Jos käyttäjä palauttaa laitteen tehdasasetukset, laite lataa uudelleen profiilin uusimmat päivitykset.</span><span class="sxs-lookup"><span data-stu-id="26d5a-p103">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="26d5a-122">Profiilin muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="26d5a-122">Edit a profile</span></span>

1. <span data-ttu-id="26d5a-123">Valitse **Valmistele Windows** -sivulla **Profiilit**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="26d5a-123">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="26d5a-124">Valitse laitteen nimen vieressä oleva valinta ruutu ja Päivitä **profiili** -paneelissa mikä tahansa käytettävissä oleva asetus \> **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="26d5a-124">Select the check box next to a device name, and in the **Profile** panel, update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="26d5a-125">Jos teet näin, ennen kuin käyttäjä yhdistää laitteen internetiin, profiilia käytetään asennuksessa.</span><span class="sxs-lookup"><span data-stu-id="26d5a-125">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="26d5a-126">Profiilin poistaminen</span><span class="sxs-lookup"><span data-stu-id="26d5a-126">Delete a profile</span></span>

1. <span data-ttu-id="26d5a-127">Valitse **Valmistele Windows** -sivulla **Profiilit**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="26d5a-127">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="26d5a-128">Valitse laitteen nimen vieressä oleva valinta ruutu ja valitse **profiili** -paneelista **Poista profiilin** \> **tallennus**.</span><span class="sxs-lookup"><span data-stu-id="26d5a-128">Select the check box next to a device name, and in the **Profile** panel, select **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="26d5a-129">Kun poistat profiilin, se poistetaan siitä laitteesta tai laiteryhmästä, johon se määritettiin.</span><span class="sxs-lookup"><span data-stu-id="26d5a-129">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="26d5a-130">Profiilin poistaminen</span><span class="sxs-lookup"><span data-stu-id="26d5a-130">Remove a profile</span></span>

1. <span data-ttu-id="26d5a-131">Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti.</span><span class="sxs-lookup"><span data-stu-id="26d5a-131">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="26d5a-132">Valitse laitteen nimen vieressä oleva valinta ruutu ja valitse **laite** -paneelista **ei mitään** avattavasta **määritetty profiili** -luettelosta \> **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="26d5a-132">Select the check box next to a device name, and in the **Device** panel, choose **None** from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
