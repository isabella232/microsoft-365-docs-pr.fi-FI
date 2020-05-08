---
title: Autopilot-laitteiden luominen ja muokkaaminen
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
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Lue, miten voit ladata laitteita AutoPilotin avulla Microsoft 365 Business Premiumissa. Voit määrittää profiilin laitteelle tai laiteryhmälle.
ms.openlocfilehash: 83c027cfe019e037518c4ca13eb331e5300fc2c1
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165857"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="1c082-104">Autopilot-laitteiden luominen ja muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="1c082-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="1c082-105">Laiteluettelon lataaminen</span><span class="sxs-lookup"><span data-stu-id="1c082-105">Upload a list of devices</span></span>

<span data-ttu-id="1c082-106">Voit ladata laitteita [vaiheittaisen oppaan](add-autopilot-devices-and-profile.md) avulla, mutta voit myös ladata laitteita **Laitteet-välilehdessä.**</span><span class="sxs-lookup"><span data-stu-id="1c082-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="1c082-107">Laitteiden on täytettävä seuraavat vaatimukset:</span><span class="sxs-lookup"><span data-stu-id="1c082-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="1c082-108">Windows 10, versio 1703 tai uudempi</span><span class="sxs-lookup"><span data-stu-id="1c082-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="1c082-109">Uudet laitteet, joita ei ole käyty Windowsin käyttökokemuksen kautta</span><span class="sxs-lookup"><span data-stu-id="1c082-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="1c082-110">Valitse Microsoft 365 -hallintakeskuksessa \> **Laitteet-automaattiohjaus**. **Devices**</span><span class="sxs-lookup"><span data-stu-id="1c082-110">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="1c082-111">Valitse **Automaattiohjaus-sivulla** **Laitteet-välilehti** \> Lisää **laitteita**.</span><span class="sxs-lookup"><span data-stu-id="1c082-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="1c082-113">Siirry **Lisää laitteita -paneelissa** [laiteluettelon CSV-tiedostoon,](https://docs.microsoft.com/microsoft-365/admin/misc/device-list) jonka olet laatinut \> **Tallenna** \> **sulje -tiedoston.**</span><span class="sxs-lookup"><span data-stu-id="1c082-113">On the **Add devices** panel, browse to a [Device list CSV file](https://docs.microsoft.com/microsoft-365/admin/misc/device-list) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="1c082-114">Saat nämä tiedot laitteistotoimittajaltasi tai voit luoda [CSV-tiedoston Get-WindowsAutoPilotInfo PowerShell -komentosarjan](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) avulla.</span><span class="sxs-lookup"><span data-stu-id="1c082-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="1c082-115">Profiilin määrittäminen laitteelle tai laiteryhmälle</span><span class="sxs-lookup"><span data-stu-id="1c082-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="1c082-116">Valitse **Valmistele Windows** -sivulla **Laitteet-välilehti** ja valitse yhden tai useamman laitteen vieressä oleva valintaruutu.</span><span class="sxs-lookup"><span data-stu-id="1c082-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="1c082-117">Valitse **Laitteet**-paneelista profiili avattavasta **Määritetty profiili** -luettelosta.</span><span class="sxs-lookup"><span data-stu-id="1c082-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="1c082-118">Jos sinulla ei ole vielä profiileja, katso ohjeita artikkelista [AutoPilot-profiilien luominen ja muokkaaminen](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="1c082-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
