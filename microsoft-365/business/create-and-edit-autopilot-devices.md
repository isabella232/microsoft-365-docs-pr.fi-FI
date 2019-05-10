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
# <a name="create-and-edit-autopilot-devices"></a>Autopilot-laitteiden luominen ja muokkaaminen

## <a name="upload-a-list-of-devices"></a>Laiteluettelon lataaminen

Voit ladata laitteita [vaiheittaisten ohjeiden](add-autopilot-devices-and-profile.md) mukaan, mutta voi ladata myös **Laitteet**-välilehdessä. 
  
Laitteiden on täytettävä nämä vaatimukset:
  
- Windows 10, versio 1703 tai uudempi.
    
- Uudet laitteet, joita ei ole määritetty Windowsin tervetuloa-ohjelmassa.

1. Valitse Microsoft 365 Business hallintakeskukseen, **laitteiden** \> **automaattiohjauksella**.
  
2. **Automaattiohjauksen** sivulla, valitse **laitteet** -välilehdessä \> **Lisää laitteita**.
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Selaa **Lisää laitteita** , paneeli [laitteen luettelosta CSV-tiedoston](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) , joka on valmistettu \> **Tallenna** \> **Sulje**.
    
    Saat nämä tiedot laitevalmistajalta tai voit käyttää PowerShell-komentosarjaa [Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), joka luo CSV-tiedoston. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Profiilin määrittäminen laitteelle tai laiteryhmälle

1. Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti ja valitse ruutu yhden tai useamman laitteen vierestä. 
    
2. Valitse **Laitteet**-paneelista profiili avattavasta **Määritetty profiili** -luettelosta. 
    
    Jos sinulla ei ole vielä profiileja, katso ohjeita artikkelista [AutoPilot-profiilien luominen ja muokkaaminen](create-and-edit-autopilot-profiles.md). 
    
