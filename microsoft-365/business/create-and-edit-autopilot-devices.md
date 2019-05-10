---
title: Autopilot-laitteiden luominen ja muokkaaminen
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
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Opi ladata laitteiden automaattiohjauksen avulla Microsoft Business-365. Voit määrittää profiilin laitteen tai laitteiden ryhmä.
ms.openlocfilehash: 6492f1469a1ac9ea67750e9ffa071d19c88c743f
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660383"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="3112f-104">Autopilot-laitteiden luominen ja muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="3112f-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="3112f-105">Laiteluettelon lataaminen</span><span class="sxs-lookup"><span data-stu-id="3112f-105">Upload a list of devices</span></span>

<span data-ttu-id="3112f-106">Voit ladata laitteita [vaiheittaisten ohjeiden](add-autopilot-devices-and-profile.md) mukaan, mutta voi ladata myös **Laitteet**-välilehdessä.</span><span class="sxs-lookup"><span data-stu-id="3112f-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="3112f-107">Laitteiden on täytettävä nämä vaatimukset:</span><span class="sxs-lookup"><span data-stu-id="3112f-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="3112f-108">Windows 10, versio 1703 tai uudempi.</span><span class="sxs-lookup"><span data-stu-id="3112f-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="3112f-109">Uudet laitteet, joita ei ole määritetty Windowsin tervetuloa-ohjelmassa.</span><span class="sxs-lookup"><span data-stu-id="3112f-109">New devices that have not been through Windows out-of-box experience.</span></span>

1. <span data-ttu-id="3112f-110">Valitse Microsoft 365 Business hallintakeskukseen, **laitteiden** \> **automaattiohjauksella**.</span><span class="sxs-lookup"><span data-stu-id="3112f-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="3112f-111">**Automaattiohjauksen** sivulla, valitse **laitteet** -välilehdessä \> **Lisää laitteita**.</span><span class="sxs-lookup"><span data-stu-id="3112f-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="3112f-113">Selaa **Lisää laitteita** , paneeli [laitteen luettelosta CSV-tiedoston](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) , joka on valmistettu \> **Tallenna** \> **Sulje**.</span><span class="sxs-lookup"><span data-stu-id="3112f-113">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="3112f-114">Saat nämä tiedot laitevalmistajalta tai voit käyttää PowerShell-komentosarjaa [Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), joka luo CSV-tiedoston.</span><span class="sxs-lookup"><span data-stu-id="3112f-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="3112f-115">Profiilin määrittäminen laitteelle tai laiteryhmälle</span><span class="sxs-lookup"><span data-stu-id="3112f-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="3112f-116">Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti ja valitse ruutu yhden tai useamman laitteen vierestä.</span><span class="sxs-lookup"><span data-stu-id="3112f-116">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="3112f-117">Valitse **Laitteet**-paneelista profiili avattavasta **Määritetty profiili** -luettelosta.</span><span class="sxs-lookup"><span data-stu-id="3112f-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="3112f-118">Jos sinulla ei ole vielä profiileja, katso ohjeita artikkelista [AutoPilot-profiilien luominen ja muokkaaminen](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="3112f-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
