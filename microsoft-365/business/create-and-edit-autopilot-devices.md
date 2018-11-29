---
title: Autopilot-laitteiden luominen ja muokkaaminen
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
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Opi ladata laitteiden automaattiohjauksen avulla Microsoft Business-365. Voit määrittää profiilin laitteen tai laitteiden ryhmä.
ms.openlocfilehash: cc1f81e9efd9b16e27b8abfbb0927d241535077e
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982933"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="e3d2c-104">Autopilot-laitteiden luominen ja muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="e3d2c-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="e3d2c-105">Laiteluettelon lataaminen</span><span class="sxs-lookup"><span data-stu-id="e3d2c-105">Upload a list of devices</span></span>

<span data-ttu-id="e3d2c-106">Voit ladata laitteita [vaiheittaisten ohjeiden](add-autopilot-devices-and-profile.md) mukaan, mutta voi ladata myös **Laitteet**-välilehdessä.</span><span class="sxs-lookup"><span data-stu-id="e3d2c-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="e3d2c-107">Laitteiden on täytettävä nämä vaatimukset:</span><span class="sxs-lookup"><span data-stu-id="e3d2c-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="e3d2c-108">Windows 10, versio 1703 tai uudempi.</span><span class="sxs-lookup"><span data-stu-id="e3d2c-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="e3d2c-109">Uudet laitteet, joita ei ole määritetty Windowsin tervetuloa-ohjelmassa.</span><span class="sxs-lookup"><span data-stu-id="e3d2c-109">New devices that have not been through Windows out-of-box experience.</span></span>
    
1. <span data-ttu-id="e3d2c-110">Valitse Microsoft 365 Businessin hallintakeskuksessa **Ota Windows käyttöön AutoPilotin avulla** **Laitetoiminnot**-kortista.</span><span class="sxs-lookup"><span data-stu-id="e3d2c-110">In the Microsoft 365 Business Admin center, choose **Deploy Windows with AutoPilot** on the **Device actions** card.</span></span> 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="e3d2c-112">Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti \> **Lisää laitteita**.</span><span class="sxs-lookup"><span data-stu-id="e3d2c-112">On the **Prepare Windows** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="e3d2c-114">Selaa **Lisää laitteita** , paneeli [laitteen luettelosta CSV-tiedoston](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) , joka on valmistettu \> **Tallenna** \> **Sulje**.</span><span class="sxs-lookup"><span data-stu-id="e3d2c-114">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="e3d2c-115">Saat nämä tiedot laitevalmistajalta tai voit käyttää PowerShell-komentosarjaa [Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), joka luo CSV-tiedoston.</span><span class="sxs-lookup"><span data-stu-id="e3d2c-115">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="e3d2c-116">Profiilin määrittäminen laitteelle tai laiteryhmälle</span><span class="sxs-lookup"><span data-stu-id="e3d2c-116">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="e3d2c-117">Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti ja valitse ruutu yhden tai useamman laitteen vierestä.</span><span class="sxs-lookup"><span data-stu-id="e3d2c-117">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="e3d2c-118">Valitse **Laitteet**-paneelista profiili avattavasta **Määritetty profiili** -luettelosta.</span><span class="sxs-lookup"><span data-stu-id="e3d2c-118">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="e3d2c-119">Jos sinulla ei ole vielä profiileja, katso ohjeita artikkelista [AutoPilot-profiilien luominen ja muokkaaminen](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="e3d2c-119">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
