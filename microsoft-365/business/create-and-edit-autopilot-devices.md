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
ms.openlocfilehash: f2a7f801ae471352595a36b355a874b2de653326
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627390"
---
# <a name="create-and-edit-autopilot-devices"></a>Autopilot-laitteiden luominen ja muokkaaminen

## <a name="upload-a-list-of-devices"></a>Laiteluettelon lataaminen

Voit ladata laitteita [vaiheittaisen oppaan](add-autopilot-devices-and-profile.md) avulla, mutta voit myös ladata laitteita **Laitteet-välilehdessä.** 
  
Laitteiden on täytettävä seuraavat vaatimukset:
  
- Windows 10, versio 1703 tai uudempi
    
- Uudet laitteet, joita ei ole käyty Windowsin käyttökokemuksen kautta

1. Valitse Microsoft 365 -hallintakeskuksessa \> **Laitteet-automaattiohjaus**. **Devices**
  
2. Valitse **Automaattiohjaus-sivulla** **Laitteet-välilehti** \> Lisää **laitteita**.
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Siirry **Lisää laitteita -paneelissa** [laiteluettelon CSV-tiedostoon,](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) jonka olet laatinut \> **Tallenna** \> **sulje -tiedoston.**
    
    Saat nämä tiedot laitteistotoimittajaltasi tai voit luoda [CSV-tiedoston Get-WindowsAutoPilotInfo PowerShell -komentosarjan](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) avulla. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Profiilin määrittäminen laitteelle tai laiteryhmälle

1. Valitse **Valmistele Windows** -sivulla **Laitteet-välilehti** ja valitse yhden tai useamman laitteen vieressä oleva valintaruutu. 
    
2. Valitse **Laitteet**-paneelista profiili avattavasta **Määritetty profiili** -luettelosta. 
    
    Jos sinulla ei ole vielä profiileja, katso ohjeita artikkelista [AutoPilot-profiilien luominen ja muokkaaminen](create-and-edit-autopilot-profiles.md). 
    
