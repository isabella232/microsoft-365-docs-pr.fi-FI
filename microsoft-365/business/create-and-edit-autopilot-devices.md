---
title: Autopilot-laitteiden luominen ja muokkaaminen
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Opi lataamaan laitteita AutoPilotilla Microsoft 365 Business Premiumissa. Voit määrittää profiilin laitteelle tai laiteryhmälle.
ms.openlocfilehash: 506ff44e3cb6656b19174e82688b5af141ea2b79
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578483"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="a0d6c-104">Autopilot-laitteiden luominen ja muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="a0d6c-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="a0d6c-105">Laiteluettelon lataaminen</span><span class="sxs-lookup"><span data-stu-id="a0d6c-105">Upload a list of devices</span></span>

<span data-ttu-id="a0d6c-106">Voit ladata laitteita [vaiheittaiset](add-autopilot-devices-and-profile.md) ohjeet avulla, mutta voit myös ladata laitteita **Laitteet-välilehdessä.**</span><span class="sxs-lookup"><span data-stu-id="a0d6c-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="a0d6c-107">Laitteiden on täytettävä seuraavat vaatimukset:</span><span class="sxs-lookup"><span data-stu-id="a0d6c-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="a0d6c-108">Windows 10, versio 1703 tai uudempi</span><span class="sxs-lookup"><span data-stu-id="a0d6c-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="a0d6c-109">Uudet laitteet, jotka eivät ole käyneet läpi Windowsin käyttökokemusta</span><span class="sxs-lookup"><span data-stu-id="a0d6c-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="a0d6c-110">Valitse Microsoft 365 -hallintakeskuksessa **Laitteet** \> **AutoPilot.**</span><span class="sxs-lookup"><span data-stu-id="a0d6c-110">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="a0d6c-111">Valitse **AutoPilot-sivulla** **Laitteet-välilehti** \> **Lisää laitteita.**</span><span class="sxs-lookup"><span data-stu-id="a0d6c-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="a0d6c-113">Siirry Lisää **laitteita -paneelissa** laiteluettelon CSV-tiedostoon, jonka valmistit [](../admin/misc/device-list.md) \> **Tallenna** sulje \> **- valmis.**</span><span class="sxs-lookup"><span data-stu-id="a0d6c-113">On the **Add devices** panel, browse to a [Device list CSV file](../admin/misc/device-list.md) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="a0d6c-114">Saat nämä tiedot laitteiston toimittajalta tai voit luoda [CSV-tiedoston Käyttämällä Get-WindowsAutoPilotInfo PowerShell-komentosarjaa.](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo)</span><span class="sxs-lookup"><span data-stu-id="a0d6c-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="a0d6c-115">Profiilin määrittäminen laitteelle tai laiteryhmälle</span><span class="sxs-lookup"><span data-stu-id="a0d6c-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="a0d6c-116">Valitse **Valmistele Windows** -sivulla **Laitteet-välilehti** ja valitse yhden tai useamman laitteen vieressä olevaa valintaruutua.</span><span class="sxs-lookup"><span data-stu-id="a0d6c-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="a0d6c-117">Valitse **Laitteet**-paneelista profiili avattavasta **Määritetty profiili** -luettelosta.</span><span class="sxs-lookup"><span data-stu-id="a0d6c-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="a0d6c-118">Jos sinulla ei ole vielä profiileja, katso ohjeita artikkelista [AutoPilot-profiilien luominen ja muokkaaminen](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="a0d6c-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
