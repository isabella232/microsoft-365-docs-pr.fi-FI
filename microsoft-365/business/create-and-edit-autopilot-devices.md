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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Opi lataamaan laitteita automaatti ohjauksen avulla Microsoft 365 Businessissa. Voit määrittää profiilin laitteelle tai laite ryhmälle.
ms.openlocfilehash: 9ae94266f5a41d8d115fc92f0f080a6fdbdc9f15
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288011"
---
# <a name="create-and-edit-autopilot-devices"></a>Autopilot-laitteiden luominen ja muokkaaminen

## <a name="upload-a-list-of-devices"></a>Laiteluettelon lataaminen

Voit ladata laitteita [vaiheittaisten ohjeiden](add-autopilot-devices-and-profile.md) mukaan, mutta voi ladata myös **Laitteet**-välilehdessä. 
  
Laitteiden on täytettävä nämä vaatimukset:
  
- Windows 10, versio 1703 tai uudempi.
    
- Uudet laitteet, joita ei ole määritetty Windowsin tervetuloa-ohjelmassa.

1. Valitse Microsoft 365 Business-hallinta keskuksessa **laitteet** \> - **automaatti ohjaus**.
  
2. Valitse **automaatti ohjaus** -sivulla **laitteet** -väli lehti \> ja **Lisää laitteita**.
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Selaa **laitteet** [-paneelissa laite luettelon CSV-tiedostoon](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) , jonka olet valmistellut \> **Tallenna** \> **Sulje**.
    
    Saat nämä tiedot laitevalmistajalta tai voit käyttää PowerShell-komentosarjaa [Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), joka luo CSV-tiedoston. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Profiilin määrittäminen laitteelle tai laiteryhmälle

1. Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti ja valitse ruutu yhden tai useamman laitteen vierestä. 
    
2. Valitse **Laitteet**-paneelista profiili avattavasta **Määritetty profiili** -luettelosta. 
    
    Jos sinulla ei ole vielä profiileja, katso ohjeita artikkelista [AutoPilot-profiilien luominen ja muokkaaminen](create-and-edit-autopilot-profiles.md). 
    
