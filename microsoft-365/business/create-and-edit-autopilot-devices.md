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
# <a name="create-and-edit-autopilot-devices"></a>Autopilot-laitteiden luominen ja muokkaaminen

## <a name="upload-a-list-of-devices"></a>Laiteluettelon lataaminen

Voit ladata laitteita [vaiheittaiset](add-autopilot-devices-and-profile.md) ohjeet avulla, mutta voit myös ladata laitteita **Laitteet-välilehdessä.** 
  
Laitteiden on täytettävä seuraavat vaatimukset:
  
- Windows 10, versio 1703 tai uudempi
    
- Uudet laitteet, jotka eivät ole käyneet läpi Windowsin käyttökokemusta

1. Valitse Microsoft 365 -hallintakeskuksessa **Laitteet** \> **AutoPilot.**
  
2. Valitse **AutoPilot-sivulla** **Laitteet-välilehti** \> **Lisää laitteita.**
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Siirry Lisää **laitteita -paneelissa** laiteluettelon CSV-tiedostoon, jonka valmistit [](../admin/misc/device-list.md) \> **Tallenna** sulje \> **- valmis.**
    
    Saat nämä tiedot laitteiston toimittajalta tai voit luoda [CSV-tiedoston Käyttämällä Get-WindowsAutoPilotInfo PowerShell-komentosarjaa.](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Profiilin määrittäminen laitteelle tai laiteryhmälle

1. Valitse **Valmistele Windows** -sivulla **Laitteet-välilehti** ja valitse yhden tai useamman laitteen vieressä olevaa valintaruutua. 
    
2. Valitse **Laitteet**-paneelista profiili avattavasta **Määritetty profiili** -luettelosta. 
    
    Jos sinulla ei ole vielä profiileja, katso ohjeita artikkelista [AutoPilot-profiilien luominen ja muokkaaminen](create-and-edit-autopilot-profiles.md). 
