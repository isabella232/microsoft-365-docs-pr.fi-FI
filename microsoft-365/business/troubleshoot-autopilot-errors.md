---
title: Autopilot-laitteen virheiden vianmääritys
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Opi tekemään vianmääritysvirheitä, jotka saatat nähdä, kun käytät AutoPilot-laitetiedostoja Microsoft 365 Business Premium.
ms.openlocfilehash: b74c57acbaa5682f6db97e7d8a090e6e28a40dcc3246f00cacc7984cb52cc758
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809176"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Autopilot-laitteen virheiden vianmääritys

## <a name="device-file-error-messages"></a>Laitetiedoston virhesanomat

Seuraavassa on tietoja joistakin virheistä, joita saatat nähdä, kun käytät AutoPilot-laitetiedostoja Microsoft 365 Business Premium. 
  
|**Virhekoodi**|**Kokeile korjausta**|
|:-----|:-----|
|Virheellinen pyynnön tekstiosa  <br/> |Tätä virhettä pitäisi tapahtua harvoin. Jos tämä virhe ilmenee, yritä toimintoa uudelleen.  <br/> |
|Laitteen laitteiston hash-arvo ei ole oikein.  <br/> |Jos näet tämän virheen, se tarkoittaa, että yhden laitteen laitteiston hash-arvoa, jonka olet antanut CSV-tiedostoon, ei ole oikein. Tarkista ensin, että arvo on kirjoitettu oikein. Jos uskot, että arvo on oikea, mutta tämä virhe ilmenee edelleen, pyydä apua laitteiston toimittajalta.  <br/> |
|Toiselle vuokraajassa määritetty laite  <br/> |Jos näet tämän virheen, se tarkoittaa, että csv-tiedostossa annettu arvo, joka on joko yhden tai useamman laitteen sarjanumero tai tuoteavain, ei ole oikein. Tarkista ensin, että arvo on kirjoitettu oikein. Jos uskot, että arvo on oikea, mutta tämä virhe ilmenee edelleen, pyydä apua laitteiston toimittajalta.  <br/> |
|CSV-tiedosto sisältää virheellisen sarjanumeron tai tuoteavaimen  <br/> |Jos näet tämän virheen, se tarkoittaa, että toinen organisaatio on jo rekisteröinyt laitteen, jota yrität rekisteröidä. Voit korjata tämän virheen pyytämällä apua laitteiston toimittajalta.  <br/> |
|Tätä laitetta ei tueta määritystä varten AutoPilotilla  <br/> | Tämä virhe tarkoittaa, että laite ei täytä AutoPilot-käyttöönottovaatimuksia. Laitteiden on täytettävä nämä vaatimukset:  <br/>  Windows 10, versio 1703 tai uudempi.  <br/>  Uudet laitteet, joissa ei ole Windows käyttökokemusta.  <br/> |
|Laitetta ei löydy  <br/> |Tämä virhe tarkoittaa, että vähintään yhtä CSV-tiedoston laitetta ei ole rekisteröity organisaatiollesi. Voit korjata ongelman pyytämällä apua laitteiston toimittajalta.  <br/> |
