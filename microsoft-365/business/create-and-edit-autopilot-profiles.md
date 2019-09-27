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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Opi luomaan, muokkaamaan, poistamaan tai poistamaan automaatti ohjauksen profiileja. '
ms.openlocfilehash: 8fae8af5e7aa7b866745d0b34a4fe11862de6e9d
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287771"
---
# <a name="create-and-edit-autopilot-profiles"></a>Autopilot-profiilien luominen ja muokkaaminen

## <a name="create-a-profile"></a>Uuden sähköpostiprofiilin luominen

Profiilia käytetään laitteeseen tai laiteryhmään
  
1. Valitse Microsoft 365 Business-hallinta keskuksessa **laitteet** \> - **automaatti ohjaus**.
  
2. Valitse **automaatti ohjaus** -sivulla **Profiilit** -väli lehti \> **Luo profiili**.
    
3. Kirjoita **Luo profiili** -sivulla nimi, jonka avulla tunnistaa sen, kuten Markkinointi. Ota käyttöön haluamasi asetus (katso kohtaa [Tietoja AutoPilot-profiilien asetuksista](autopilot-profile-settings.md)) ja valitse **Tallenna**.
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Profiilin käyttäminen laitteeseen

Kun olet luonut profiilin, voit käyttää sitä laitteeseen tai laiteryhmään. Voit valita olemassa olevan profiilin [vaiheittaisten ohjeiden](add-autopilot-devices-and-profile.md) avulla, voit käyttää sitä uusiin laitteisiin tai voit korvata laitteen tai laiteryhmän olemassa olevan profiilin. 
  
1. Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti. 
    
2. Valitse valintaruutu laitteen nimen vierestä ja valitse **Laite**-paneeli. Valitse profiili avattavasta **Määritetty profiili** -valikosta \> **Tallenna**.
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Profiilin muokkaaminen tai poistaminen

Kun olet määrittänyt profiilin laitteeseen, voit päivittää sen, vaikka olet jo antanut laitteen käyttäjälle. Kun laite muodostaa internet-yhteyden, se lataa profiilisi uusimman version asennuksen aikana. Jos käyttäjä palauttaa laitteen tehdasasetukset, laite lataa uudelleen profiilin uusimmat päivitykset. 
  
### <a name="edit-a-profile"></a>Profiilin muokkaaminen

1. Valitse **Valmistele Windows** -sivulla **Profiilit**-välilehti. 
    
2. Valitse valintaruutu laitteen nimen vierestä ja päivitä **Profiili**-paneelissa haluamasi asetukset \> **Tallenna**.
    
    Jos teet näin, ennen kuin käyttäjä yhdistää laitteen internetiin, profiilia käytetään asennuksessa.
    
### <a name="delete-a-profile"></a>Profiilin poistaminen

1. Valitse **Valmistele Windows** -sivulla **Profiilit**-välilehti. 
    
2. Valitse valintaruutu laitteen nimen vierestä ja valitse **Profiili**-paneelissa **Poista profiili** \> **Tallenna**.
    
    Kun poistat profiilin, se poistetaan siitä laitteesta tai laiteryhmästä, johon se määritettiin.
    
### <a name="remove-a-profile"></a>Profiilin poistaminen

1. Valitse **Valmistele Windows** -sivulla **Laitteet**-välilehti. 
    
2. Valitse valintaruutu laitteen nimen vierestä ja valitse **Laite**-paneelissa **Ei mitään** avattavasta **Määritetty profiili** -valikosta \> **Tallenna**.
    
