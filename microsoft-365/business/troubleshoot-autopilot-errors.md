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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Tietoja automaatti ohjauksen laite virheiden vian määrityksestä.
ms.openlocfilehash: 8390f695a3e11386ae2617da4061bed1d8214375
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594204"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Autopilot-laitteen virheiden vianmääritys

## <a name="device-file-error-messages"></a>Laite tiedoston virhe sanomat

Tässä on tietoja joistakin virheistä, joita saatat nähdä työskennellessään automaatti ohjauksen laite tiedostojen kanssa Microsoft 365 Businessissa. 
  
|**Virhekoodi**|**Fix kokeilla**|
|:-----|:-----|
|Virheellinen pyynnön leipä teksti  <br/> |Tämän virheen pitäisi tapahtua harvoin, jos näet tämän virheen, yritä toimintoa uudelleen.  <br/> |
|Laitteen laitteiston hajautus arvo ei ole oikea.  <br/> |Jos näet tämän virheen, se tarkoittaa, että yhden laitteen laitteiston hajautus arvon CSV-tiedostossa antama arvo ei ole oikea. Tarkista ensin, että arvo on kirjoitettu oikein. Jos arvelet, että arvo on oikea, mutta tämä virhe tapahtuu edelleen, pyydä apua laitteiston toimittajalta.  <br/> |
|Toiseen vuokraajaan liitetty laite  <br/> |Jos näet tämän virheen, se tarkoittaa, että CSV-tiedostossa annettu arvo joko yhden tai useamman laitteen sarja numeroa tai Product Key-tunnusta varten ei ole oikea. Tarkista ensin, että arvo on kirjoitettu oikein. Jos arvelet, että arvo on oikea, mutta tämä virhe tapahtuu edelleen, pyydä apua laitteiston toimittajalta.  <br/> |
|CSV-tiedostossa on virheellinen sarja numero tai Product Key-tunnus  <br/> |Jos näet tämän virheen, se tarkoittaa, että laite, jota yrität rekisteröidä, on jo toisen organisaation rekisteröimää. Voit korjata tämän virheen pyytämällä laitteiston toimittajalta apua.  <br/> |
|Tätä laitetta ei tueta asennuksessa käyttämällä automaatti ohjausta  <br/> | Tämä virhe tarkoittaa, että laite ei vastaa automaatti ohjauksen käyttöönoton vaatimuksia. Laitteiden on täytettävä nämä vaatimukset:  <br/>  Windows 10, versio 1703 tai uudempi.  <br/>  Uudet laitteet, jotka eivät ole olleet Windows out-of-Box-kokemuksen kautta.  <br/> |
|Laitetta ei löydy  <br/> |Tämä virhe tarkoittaa sitä, että yhtä tai useampaa CSV-tiedostossa olevaa laitetta ei ole rekisteröity organisaatioosi. Voit korjata tämän ongelman pyytämällä laitteiston toimittajalta apua.  <br/> |
