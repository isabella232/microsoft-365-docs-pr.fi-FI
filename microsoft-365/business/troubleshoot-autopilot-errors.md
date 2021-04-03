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
description: Lue, miten voit tehdä vianmäärityksen, jonka saatat nähdä, kun käytät AutoPilot-laitetiedostoja Microsoft 365 Business Premiumissa.
ms.openlocfilehash: 1078ab74b07952e4bb565555a081b98ecce9db5c
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578083"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Autopilot-laitteen virheiden vianmääritys

## <a name="device-file-error-messages"></a>Laitetiedoston virhesanomat

Seuraavassa on tietoja virheistä, joita saatat nähdä, kun käytät AutoPilot-laitetiedostoja Microsoft 365 Business Premiumissa. 
  
|**Virhekoodi**|**Korjaus kokeilemaan**|
|:-----|:-----|
|Virheellinen pyynnön tekstiosa  <br/> |Tämän virheen pitäisi tapahtua harvoin, jos näet tämän virheen, yritä toimintoa uudelleen.  <br/> |
|Laitteen laitteiston hash-arvo ei ole oikein.  <br/> |Jos näet tämän virheen, se tarkoittaa, että yhden laitteen laitteiston hash-arvo CSV-tiedostossa ei ole oikein. Varmista ensin, että arvo on kirjoitettu oikein. Jos uskot, että arvo on oikea, mutta virhe ilmenee edelleen, pyydä apua laitteiston toimittajalta.  <br/> |
|Toiselle vuokraajassa määritetty laite  <br/> |Jos näet tämän virheen, csv-tiedostossa annettu arvo, joka on joko sarjanumero tai yhden tai useamman laitteen tuoteavain, ei ole oikein. Varmista ensin, että arvo on kirjoitettu oikein. Jos uskot, että arvo on oikea, mutta virhe ilmenee edelleen, pyydä apua laitteiston toimittajalta.  <br/> |
|CSV-tiedosto sisältää virheellisen sarjanumeron tai tuoteavaimen  <br/> |Jos tämä virhe ilmenee, toinen organisaatio on jo rekisteröinyt laitteen, jota yrität rekisteröidä. Voit korjata tämän virheen pyytämällä apua laitteiston toimittajalta.  <br/> |
|Tätä laitetta ei tueta autopilotin määrityksessä  <br/> | Tämä virhe tarkoittaa, että laite ei täytä AutoPilot-käyttöönottovaatimuksia. Laitteiden on täytettävä nämä vaatimukset:  <br/>  Windows 10, versio 1703 tai uudempi.  <br/>  Uudet laitteet, jotka eivät ole käyneet läpi Windowsin käyttökokemusta.  <br/> |
|Laitetta ei löydy  <br/> |Tämä virhe tarkoittaa, että vähintään yhtä CSV-tiedoston laitetta ei ole rekisteröity organisaatiollesi. Voit korjata ongelman pyytämällä apua laitteiston toimittajalta.  <br/> |
