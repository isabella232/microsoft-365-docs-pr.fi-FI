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
description: Opi lataamaan laitteet AutoPilotilla Microsoft 365 Business Premium. Voit määrittää profiilin laitteeseen tai laiteryhmään.
ms.openlocfilehash: ae3a760db4b94aac50301685a0c4f468e46ec8e9aa907a1b6fb35e03a9e541f0
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53867032"
---
# <a name="create-and-edit-autopilot-devices"></a>Autopilot-laitteiden luominen ja muokkaaminen

## <a name="upload-a-list-of-devices"></a>Laiteluettelon lataaminen

Voit ladata laitteita [vaiheittaiset ohjeet](add-autopilot-devices-and-profile.md) -oppaassa, mutta voit myös ladata laitteita **Laitteet-välilehdessä.** 
  
Laitteiden on täytettävä seuraavat vaatimukset:
  
- Windows 10, versio 1703 tai uudempi
    
- Uudet laitteet, joita ei ole Windows käyttökokemusta

1. Valitse Microsoft 365 -hallintakeskus  \> **AutoPilot**.
  
2. Valitse **AutoPilot-sivulla** **Laitteet-välilehti** \> **Lisää laitteita**.
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Siirry Lisää **laitteita -paneelissa** laiteluettelon [CSV-tiedostoon, jonka](../admin/misc/device-list.md) latasit Tallenna \>  \> **sulje -ruudussa.**
    
    Saat nämä tiedot laitteiston toimittajalta tai voit luoda [CSV-tiedoston Käyttämällä PowerShell-komentosarjaa Get-WindowsAutoPilotInfo.](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Profiilin määrittäminen laitteelle tai laiteryhmälle

1. Valitse **Valmistele Windows** -sivulla **Laitteet-välilehti** ja valitse yhden tai useamman laitteen vieressä olevaa valintaruutua. 
    
2. Valitse **Laitteet**-paneelista profiili avattavasta **Määritetty profiili** -luettelosta. 
    
    Jos sinulla ei ole vielä profiileja, katso ohjeita artikkelista [AutoPilot-profiilien luominen ja muokkaaminen](create-and-edit-autopilot-profiles.md). 
