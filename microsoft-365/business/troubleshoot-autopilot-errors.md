---
title: Autopilot-laitteen virheiden vianmääritys
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Lue tietoja automaattiohjauksen laitetiedostojen käyttämisen yhteydessä microsoft 365 Business Premiumissa mahdollisesti näkyvien virheiden vianmäärityksestä.
ms.openlocfilehash: bec5126696ee322db42e4b7c5cd8e0df485ab2c9
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403406"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Autopilot-laitteen virheiden vianmääritys

## <a name="device-file-error-messages"></a>Laitetiedoston virhesanomat

Tässä on tietoja joistakin virheistä, joita saatat nähdä työskennellessäsi AutoPilot-laitetiedostojen kanssa Microsoft 365 Business Premiumissa. 
  
|**Virhekoodi**|**Yritä korjata**|
|:-----|:-----|
|Virheellinen pyynnön teksti  <br/> |Tämän virheen pitäisi tapahtua harvoin, jos näet tämän virheen, yritä toimintoa uudelleen.  <br/> |
|Laitteen laitteiston hajautusarvo ei ole oikea.  <br/> |Jos näet tämän virheen, se tarkoittaa, että CSV-tiedostossa antamasi arvo yhden laitteen laitteistohajautusarvolle ei ole oikea. Varmista ensin, että arvo on kirjoitettu oikein. Jos olet sitä mieltä, että arvo on oikea, mutta tämä virhe tapahtuu edelleen, pyydä apua laitteiston valmistajalta.  <br/> |
|Toiselle vuokralaiselle määritetty laite  <br/> |Jos näet tämän virheen, se tarkoittaa, että CSV-tiedostossa antamasi arvo yhden tai useamman laitteen sarjanumerolle tai tuotetunnukselle ei ole oikea. Varmista ensin, että arvo on kirjoitettu oikein. Jos olet sitä mieltä, että arvo on oikea, mutta tämä virhe tapahtuu edelleen, pyydä apua laitteiston valmistajalta.  <br/> |
|CSV-tiedosto sisältää virheellisen sarjanumeron tai product key -tunnuksen  <br/> |Jos näet tämän virheen, toinen organisaatio on jo rekisteröinyt laitteen, jota yrität rekisteröidä. Voit korjata tämän virheen kysykää laitevalmistajaltaapua.  <br/> |
|Tätä laitetta ei tueta automaattisen ohjauksen avulla  <br/> | Tämä virhe tarkoittaa, että laite ei täytä AutoPilotin käyttöönottovaatimuksia. Laitteiden on täytettävä nämä vaatimukset:  <br/>  Windows 10, versio 1703 tai uudempi.  <br/>  Uudet laitteet, joita ei ole käyty Windowsin käyttökokemuksen kautta.  <br/> |
|Laitetta ei löydy  <br/> |Tämä virhe tarkoittaa, että yhtä tai useampaa CSV-tiedoston laitetta ei ole rekisteröity organisaatioosi. Voit korjata ongelman kysykää laitevalmistajaltasi apua.  <br/> |
