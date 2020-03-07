---
title: Autopilot-laitteen virheiden vianmääritys
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: troubleshooting
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Lue tietoja autopilotin laitetiedostojen käsittelemisen aikana Microsoft 365 Businessissa mahdollisesti näkyvien virheiden vianmäärityksestä.
ms.openlocfilehash: dc1abd508156c8525859f6ca7e291ab38fc8859c
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/07/2020
ms.locfileid: "42560696"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Autopilot-laitteen virheiden vianmääritys

## <a name="device-file-error-messages"></a>Laitetiedoston virhesanomat

Tässä on tietoja joistakin virheistä, joita saatat nähdä työskenneltäessä AutoPilot-laitetiedostojen kanssa Microsoft 365 Businessissa. 
  
|**Virhekoodi**|**Korjaa yrittää**|
|:-----|:-----|
|Virheellinen pyynnön teksti  <br/> |Tämän virheen pitäisi tapahtua harvoin, jos näet tämän virheen, yritä toimintoa uudelleen.  <br/> |
|Laitteen hajautusarvo ei ole oikea.  <br/> |Jos näet tämän virheen, se tarkoittaa, että csv-tiedostossa antamasi arvo yhden laitteen laitteistohajautusarvolle ei ole oikea. Varmista ensin, että arvo on kirjoitettu oikein. Jos olet sitä mieltä, että arvo on oikea, mutta tämä virhe on edelleen käynnissä, pyydä apua laitteiston valmistajalta.  <br/> |
|Toiselle vuokraajan laitteelle määritetty laite  <br/> |Jos näet tämän virheen, se tarkoittaa, että CSV-tiedostossa antamasi arvo yhden tai useamman laitteen sarjanumerolle tai tuoteavaimelle ei ole oikea. Varmista ensin, että arvo on kirjoitettu oikein. Jos olet sitä mieltä, että arvo on oikea, mutta tämä virhe on edelleen käynnissä, pyydä apua laitteiston valmistajalta.  <br/> |
|CSV-tiedosto sisältää virheellisen sarjanumeron tai product key -avaimen  <br/> |Jos näet tämän virheen, toinen organisaatio on jo rekisteröinyt laitteen, jota yrität rekisteröidä. Voit korjata tämän virheen kysyt neuvoa laitteiston valmistajalta.  <br/> |
|Tätä laitetta ei tueta asennusta varten autopilotin avulla  <br/> | Tämä virhe tarkoittaa, että laite ei täytä automaattiohjauksen käyttöönottovaatimuksia. Laitteiden on täytettävä nämä vaatimukset:  <br/>  Windows 10, versio 1703 tai uudempi.  <br/>  Uudet laitteet, jotka eivät ole käyneet Windowsin läpi.  <br/> |
|Laitetta ei löydy  <br/> |Tämä virhe tarkoittaa, että vähintään yhtä CSV-tiedoston laitetta ei ole rekisteröity organisaatioosi. Voit korjata ongelman kysyt neuvoa laitteiston valmistajalta.  <br/> |
