---
title: Autopilot-profiilien luominen ja muokkaaminen
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Opi luomaan AutoPilot-profiili ja käyttämään sitä laitteessa sekä muokkaamaan tai poistamaan profiilia tai poistamaan profiili laitteesta.
ms.openlocfilehash: 414243da88fb6f39f8e6067d19d49ffe955f725f
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580250"
---
# <a name="create-and-edit-autopilot-profiles"></a>Autopilot-profiilien luominen ja muokkaaminen

## <a name="create-a-profile"></a>Uuden sähköpostiprofiilin luominen

Profiilia käytetään laitteeseen tai laiteryhmään
  
1. Valitse Microsoft 365 -hallintakeskuksessa **Laitteet** \> **AutoPilot.**
  
2. Valitse **AutoPilot-sivulla** **Profiilit-välilehti** \> **Luo profiili.**
    
3. Kirjoita **Luo profiili -sivulle** profiilille nimi, joka auttaa tunnistamaan sen, esimerkiksi Markkinointi. Ota haluamasi asetus käyttöön ja valitse sitten **Tallenna.** Lisätietoja AutoPilot-profiiliasetuksista on kohdassa Tietoja [AutoPilot-profiiliasetuksista.](autopilot-profile-settings.md)
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Profiilin käyttäminen laitteeseen

Kun olet luonut profiilin, voit käyttää sitä laitteessa tai laiteryhmässä. Voit valita olemassa olevan profiilin vaiheittaiset [ohjeet](add-autopilot-devices-and-profile.md) ja ottaa sen käyttöön uusissa laitteissa tai korvata olemassa olevan profiilin laitteelle tai laiteryhmälle. 
  
1. Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti. 
    
2. Valitse laitteen nimen vieressä olevaa valintaruutua  ja valitse Laite-paneelissa  profiili avattavasta Määritetty profiili -luettelosta \> **Tallenna.**
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Profiilin muokkaaminen tai poistaminen

Kun olet määrittänyt profiilin laitteeseen, voit päivittää sen, vaikka olet jo antanut laitteen käyttäjälle. Kun laite muodostaa internet-yhteyden, se lataa profiilisi uusimman version asennuksen aikana. Jos käyttäjä palauttaa laitteen tehdasasetukset, laite lataa uudelleen profiilin uusimmat päivitykset. 
  
### <a name="edit-a-profile"></a>Profiilin muokkaaminen

1. Valitse **Valmistele Windows** -sivulla **Profiilit**-välilehti. 
    
2. Valitse laitteen nimen vieressä oleva valintaruutu ja  päivitä profiilipaneelissa jokin käytettävissä olevista asetuksista \> **Tallenna.**
    
    Jos teet näin, ennen kuin käyttäjä yhdistää laitteen internetiin, profiilia käytetään asennuksessa.
    
### <a name="delete-a-profile"></a>Profiilin poistaminen

1. Valitse **Valmistele Windows** -sivulla **Profiilit**-välilehti. 
    
2. Valitse laitteen nimen vieressä olevaa valintaruutua ja valitse **Profiili-paneelissa** **Poista profiilitallenna.** \> 
    
    Kun poistat profiilin, se poistetaan siitä laitteesta tai laiteryhmästä, johon se määritettiin.
    
### <a name="remove-a-profile"></a>Profiilin poistaminen

1. Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti. 
    
2. Valitse laitteen nimen vieressä olevaa valintaruutua  ja valitse  Laite-paneelissa Ei mitään avattavasta Määritetty profiili -luettelosta  \> **Tallenna.**
    
