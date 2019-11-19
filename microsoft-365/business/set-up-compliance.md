---
title: Lisää uhkien suojausta Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Määritä yhteensopivuus ominaisuuksia tietojen menettämisen estämiseksi ja arkaluonteisten tietojen otsikoiksi.
ms.openlocfilehash: 6fae95e8c5e6d133e3163dbdfd3c09cfede11382
ms.sourcegitcommit: 5d11f516e78ea4a74145e19ba2300f0792c8bac1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/19/2019
ms.locfileid: "38715118"
---
# <a name="set-up-compliance-features"></a>Yhteensopivuus ominaisuuksien määrittäminen

Microsoft 365-yritys sisältää ominaisuuksia, jotka suojaavat tietojasi ja laitteitasi sekä auttavat pitämään omasi ja asiakkaidesi arkaluonteiset tiedot turvassa.

## <a name="set-up-dlp-features"></a>DLP-ominaisuuksien määrittäminen

Katso [Luo DLP-käytäntö mallista](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) esimerkkinä siitä, miten voit määrittää käytännön suojaamaan henkilökohtaisia tunniste tietoja (pii) vastaan. 
  
DLP sisältää monia valmiita käytäntö malleja monille eri kieli alueilla. Esimerkiksi Australian taloudelliset tiedot, Kanadan henkilö tieto laki, Yhdysvaltain taloudelliset tiedot ja niin vielä. Katso, [mitä DLP-käytäntö mallit sisältävät](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) täydellisestä luettelosta. Kaikki nämä mallit voidaan ottaa käyttöön samanlaisiksi kuin PII-malli esimerkki. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Sähkö postin säilyttämisen määrittäminen Exchange Online-arkistoinnin avulla

 **Exchange Online-arkistointi** lisenssi ominaisuudet auttavat ylläpitämään yhteensopivuus-ja sääntely standardeja säilyttämällä Sähkö posti sisällön eDiscovery. Se myös auttaa vähentämään riskiä, jos on oikeus juttu, ja tarjoaa tapa palauttaa tietoja, kun tieto turva loukkaus tai kun haluat palauttaa poistetut kohteet. Voit säilyttää kaikki käyttäjän sisällöt tai käyttää säilytys käytäntöjä, kun haluat muokata säilytetä.
  
**Oikeuden käyntien pito:** Voit säilyttää kaiken posti laatikon sisällön, mukaan lukien poistetut kohteet, asettamalla käyttäjän koko posti laatikon oikeus riita-asioihin. 
    
Voit sijoittaa posti laatikon oikeuden käyntiin pitämällä hallinta keskuksessa:
    
1. Siirry vasemmassa siirtymis osassa **käyttäjät** \> **aktiiviset käyttäjät**-kohtaan.
    
2. Valitse käyttäjä, jonka posti laatikon haluat sijoittaa riita-asioihin. Laajenna käyttäjä ruudussa **mailin asetukset**ja valitse **Lisää asetuksia**-kohdasta **Muokkaa Exchangen ominaisuuksia**.
    
3. Valitse käyttäjän posti laatikko-sivulla * * posti laatikon ominaisuudet * * vasemmassa NAV-ohjelmassa ja valitse sitten **Ota käyttöön** -linkki kohdassa **oikeuden käynti pito**.
    
4. Voit määrittää **oikeuden käynnin pito-valinta ikkunassa** oikeuden käyntien keston **oikeuden käynnin** keston kentässä. Jätä kenttä tyhjäksi, jos haluat sijoittaa äärettömän pito-arvon. Voit myös lisätä muistiinpanoja ja ohjata posti laatikon omistajaa verkkosivustolle, jota saatat joutua selittämään lisää riita-asioiden pito paikasta. \>**Tallenna**.
    
**Säilyttäminen:** Voit ottaa käyttöön mukautetut säilytys käytännöt, esimerkiksi säilyttää tietyn ajan tai poistaa sisällön pysyvästi säilytys ajan päätyttyä. Lisä tietoja [on kohdassa säilytys käytäntöjen yleiskatsaus](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-sensitivity-labels"></a>Määritä herkkyys otsikot

Herkkyys tunnisteissa on Azure Information Protection (AIP)-suunnitelma 1, ja ne auttavat luokittelemaan ja valinnaisesti suojaamaan asia kirjasi ja sähkö postit käyttämällä tunnisteita. Järjestelmänvalvojat voivat käyttää otsikoita automaattisesti, jos käyttäjät määrittävät säännöt ja ehdot manuaalisesti, tai käyttämällä yhdistelmää, jossa käyttäjille annetaan suosituksia.

Jos haluat määrittää herkkyys otsikot, katso [Luo ja hallitse herkkyys tarroja](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.



### <a name="install-the-azure-information-protection-client-manually"></a>Azure-tieto suoja asiakkaan asentaminen manuaalisesti

Voit asentaa AIP-asiakkaan manuaalisesti:

1. Lataa **AzinfoProtection_UL. exe** [Microsoft Download Centeristä](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Voit varmistaa, että asennus on toiminut tarkastelemalla Word-asia kirjaa ja varmistamalla, että **herkkyys** asetus on käytettävissä **Aloitus** -väli lehdellä.
<br/>![Word-asia kirjan avattava suojaus-väli lehti.](media/word-sensitivity.png)

Lisä tietoja on kohdassa [Asenna asiakas](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
