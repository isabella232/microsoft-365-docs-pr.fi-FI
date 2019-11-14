---
title: Autopilot-profiilien luominen ja muokkaaminen
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
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Opi luomaan, muokkaamaan, poistamaan tai poistamaan automaatti ohjauksen profiileja.
ms.openlocfilehash: f7fdc2632e93c48e043fe158842f8395d6a89e14
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320234"
---
# <a name="create-and-edit-autopilot-profiles"></a>Autopilot-profiilien luominen ja muokkaaminen

## <a name="create-a-profile"></a>Uuden sähköpostiprofiilin luominen

Profiilia käytetään laitteeseen tai laiteryhmään
  
1. Valitse Microsoft 365 Business-hallinta keskuksessa **laitteet** \> - **automaatti ohjaus**.
  
2. Valitse **automaatti ohjaus** -sivulla **Profiilit** -väli lehti \> **Luo profiili**.
    
3. Kirjoita **Luo profiili** -sivulla sen profiilin nimi, joka auttaa tunnistamaan sen, esimerkiksi markkinointi. Ota haluamasi asetus käyttöön ja valitse **Tallenna**. Lisä tietoja automaatti ohjauksen profiili asetuksista on kohdassa [tietoja automaatti ohjauksen profiili asetuksista](autopilot-profile-settings.md).
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Profiilin käyttäminen laitteeseen

Kun olet luonut profiilin, voit käyttää sitä laitteessa tai laite ryhmässä. Voit valita olemassa olevan profiilin [vaiheittainen opas](add-autopilot-devices-and-profile.md) ja käyttää sitä uusiin laitteisiin tai korvata olemassa olevan profiilin laitteelle tai laite ryhmälle. 
  
1. Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti. 
    
2. Valitse laitteen nimen vieressä oleva valinta ruutu ja valitse **laite** -paneelista profiili avattavasta **määritetty profiili** -luettelosta \> **Tallenna**.
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Profiilin muokkaaminen tai poistaminen

Kun olet määrittänyt profiilin laitteeseen, voit päivittää sen, vaikka olet jo antanut laitteen käyttäjälle. Kun laite muodostaa internet-yhteyden, se lataa profiilisi uusimman version asennuksen aikana. Jos käyttäjä palauttaa laitteen tehdasasetukset, laite lataa uudelleen profiilin uusimmat päivitykset. 
  
### <a name="edit-a-profile"></a>Profiilin muokkaaminen

1. Valitse **Valmistele Windows** -sivulla **Profiilit**-välilehti. 
    
2. Valitse laitteen nimen vieressä oleva valinta ruutu ja Päivitä **profiili** -paneelissa mikä tahansa käytettävissä oleva asetus \> **Tallenna**.
    
    Jos teet näin, ennen kuin käyttäjä yhdistää laitteen internetiin, profiilia käytetään asennuksessa.
    
### <a name="delete-a-profile"></a>Profiilin poistaminen

1. Valitse **Valmistele Windows** -sivulla **Profiilit**-välilehti. 
    
2. Valitse laitteen nimen vieressä oleva valinta ruutu ja valitse **profiili** -paneelista **Poista profiilin** \> **tallennus**.
    
    Kun poistat profiilin, se poistetaan siitä laitteesta tai laiteryhmästä, johon se määritettiin.
    
### <a name="remove-a-profile"></a>Profiilin poistaminen

1. Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti. 
    
2. Valitse laitteen nimen vieressä oleva valinta ruutu ja valitse **laite** -paneelista **ei mitään** avattavasta **määritetty profiili** -luettelosta \> **Tallenna**.
    
