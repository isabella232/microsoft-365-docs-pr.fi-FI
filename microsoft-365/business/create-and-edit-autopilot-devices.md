---
title: Autopilot-laitteiden luominen ja muokkaaminen
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
description: Opi lataamaan laitteita automaatti ohjauksen avulla Microsoft 365 Businessissa. Voit määrittää profiilin laitteelle tai laite ryhmälle.
ms.openlocfilehash: 1dd6b1a574166379e29465bf3699e47e3b155e0b
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320254"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="0a2c0-104">Autopilot-laitteiden luominen ja muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="0a2c0-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="0a2c0-105">Laiteluettelon lataaminen</span><span class="sxs-lookup"><span data-stu-id="0a2c0-105">Upload a list of devices</span></span>

<span data-ttu-id="0a2c0-106">Voit käyttää [vaiheittaisia oppaita](add-autopilot-devices-and-profile.md) laitteiden lataamiseen, mutta voit myös ladata laitteita **laitteet** -väli lehdeltä.</span><span class="sxs-lookup"><span data-stu-id="0a2c0-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="0a2c0-107">Laitteiden on täytettävä nämä vaatimukset:</span><span class="sxs-lookup"><span data-stu-id="0a2c0-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="0a2c0-108">Windows 10, versio 1703 tai uudempi</span><span class="sxs-lookup"><span data-stu-id="0a2c0-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="0a2c0-109">Uudet laitteet, jotka eivät ole olleet Windows-käyttö kokemuksen kautta</span><span class="sxs-lookup"><span data-stu-id="0a2c0-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="0a2c0-110">Valitse Microsoft 365 Business-hallinta keskuksessa **laitteet** \> - **automaatti ohjaus**.</span><span class="sxs-lookup"><span data-stu-id="0a2c0-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="0a2c0-111">Valitse **automaatti ohjaus** -sivulla **laitteet** -väli lehti \> ja **Lisää laitteita**.</span><span class="sxs-lookup"><span data-stu-id="0a2c0-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="0a2c0-113">Siirry **Lisää laitteita** -paneelissa sen [laite luettelon CSV-tiedostoon](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) , jonka valmistelit \> **Tallenna** \> **Sulje**.</span><span class="sxs-lookup"><span data-stu-id="0a2c0-113">On the **Add devices** panel, browse to a [Device list CSV file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="0a2c0-114">Voit hankkia nämä tiedot laitteiston toimittajalta, tai voit luoda CSV-tiedoston [Get-WindowsAutoPilotInfo PowerShell-komento sarjan](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) avulla.</span><span class="sxs-lookup"><span data-stu-id="0a2c0-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="0a2c0-115">Profiilin määrittäminen laitteelle tai laiteryhmälle</span><span class="sxs-lookup"><span data-stu-id="0a2c0-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="0a2c0-116">Valitse **Valmistele Windows** -sivulla **laitteet** -väli lehti ja valitse yhden tai useamman laitteen vieressä oleva valinta ruutu.</span><span class="sxs-lookup"><span data-stu-id="0a2c0-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="0a2c0-117">Valitse **Laitteet**-paneelista profiili avattavasta **Määritetty profiili** -luettelosta.</span><span class="sxs-lookup"><span data-stu-id="0a2c0-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="0a2c0-118">Jos sinulla ei ole vielä profiileja, katso ohjeita artikkelista [AutoPilot-profiilien luominen ja muokkaaminen](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="0a2c0-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
