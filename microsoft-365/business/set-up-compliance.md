---
title: Paranna Microsoft 365 Business Premiumin uhkien suojausta
f1.keywords:
- NOCSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Määritä yhteensopivuus ominaisuudet, jotka estävät tietojen menettämisen ja auttavat pitämään asiakkaiden luottamukselliset tiedot turvassa.
ms.openlocfilehash: 2c95ad3f36df28af2c68cd11192bcfe92dfe29e3
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841169"
---
# <a name="set-up-compliance-features"></a>Yhteensopivuus ominaisuuksien määrittäminen

Microsoft 365 Business Premiumin ominaisuuksiin kuuluu tietojen ja laitteiden suojaaminen, ja sen avulla voit pitää asiakkaidemme luottamukselliset tiedot turvassa.

## <a name="set-up-dlp-features"></a>DLP-ominaisuuksien määrittäminen

Lisä tietoja on kohdassa [DLP-käytäntöjen luominen mallista](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) , jossa on esimerkki käytännöstä, jonka avulla voit suoja utua henkilökohtaisten tietojen menettämisen varalta. 
  
DLP sisältää monia käyttövalmiita käytäntöjen malleja useille eri kieli alueille. Esimerkiksi Australian taloudelliset tiedot, Kanadan henkilö tieto laki, USA:n taloudelliset tiedot ja niin edelleen. Katso [, mitä DLP-käytännöt sisältävät](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) täydellisen luettelon. Kaikki nämä mallit voidaan ottaa käyttöön vastaavalla tavalla kuin PII-malli esimerkki. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Sähkö postin säilytyksen määrittäminen Exchange Online-arkistoinnin avulla

 **Exchange Onlinen arkistoinnin** käyttö oikeus ominaisuuksien avulla voit ylläpitää yhteensopivuus-ja säännös standardeja säilyttämällä sähkö postin sisällön eDiscoveryyn. Se myös vähentää riskiä, jos kyseessä on oikeus juttu, ja sen avulla voit palauttaa tietoja, kun tieto turva on rikottu tai kun sinun on palautettava poistetut kohteet. Voit käyttää oikeus toimiin liittyvään pitoon, jos haluat säilyttää kaikki käyttäjän sisällöt, tai käyttää säilytys käytäntöjä, jotka mukauttavat säilytettävän sisällön.
  
**Oikeus toimiin liittyvään pitoon:** Voit säilyttää kaikki posti laatikon sisältö, mukaan lukien poistetut kohteet, asettamalla käyttäjän koko posti laatikon oikeus toimiin liittyvään pitoon. 
    
Jos haluat sijoittaa posti laatikon oikeus toimiin liittyvään pitoon, valitse hallinta keskuksessa:
    
1. Valitse vasemmanpuoleisessa siirtymis ruudussa **käyttäjät** \> **aktiiviset käyttäjät**.
    
2. Valitse käyttäjä, jonka posti laatikon haluat sijoittaa oikeus toimiin liittyvään pitoon. Laajenna käyttäjä ruudussa **Sähkö posti asetukset** ja valitse **lisä asetukset** -kohdan vierestä **Muokkaa Exchangen ominaisuuksia**.
    
3. Valitse käyttäjän posti laatikko-sivulla * * posti laatikon ominaisuudet * * vasemmassa siirtymis ruudussa ja valitse sitten **Ota käyttöön** -linkki **oikeus toimiin liittyvään pitoon**.
    
4. Oikeus toimiin liittyvän **pidon** valinta ikkunassa voit määrittää oikeus toimiin liittyvän pidon keston **oikeus toimiin liittyvän pidon kesto** -kentässä. Jätä kenttä tyhjäksi, jos haluat sijoittaa äärettömään pitoon. Voit myös lisätä muistiinpanoja ja ohjata posti laatikon omistajan sivustoon, josta sinun on ehkä selitettävä lisää oikeus toimiin liittyvästä pidosta. \>**Tallenna**.
    
**Säilyttäminen:** Voit ottaa käyttöön mukautetut säilytys käytännöt, jotka esimerkiksi säilyttävät tietyn ajan tai poistavat sisältöä pysyvästi säilytys ajan päätyttyä. Lisä tietoja on artikkelissa [säilytys käytäntöjen yleiskatsaus](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).

## <a name="set-up-sensitivity-labels"></a>Luottamuksellisuusmerkkien määrittäminen

Herkkyys selitteissä on Azure Information Protectionin (AIP) sopimus 1, ja niiden avulla voit luokitella ja halutessasi suojata asia kirjoja ja sähkö posteja käyttämällä otsikoita. Käyttäjät voivat ottaa nimiöt automaattisesti käyttöön, jotka määrittävät säännöt ja ehdot manuaalisesti käyttäjiltä tai käyttämällä yhdistelmää, jossa käyttäjille annetaan suosituksia.

Voit määrittää herkkyys otsikoita valitsemalla [Luo ja hallitse luottamuksellisuusotsikoita](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) -video.



### <a name="install-the-azure-information-protection-client-manually"></a>Azure Information Protectionin asiakas ohjelman asentaminen manuaalisesti

Jos haluat asentaa AIP-asiakas ohjelman manuaalisesti, toimi seuraavasti:

1. Lataa **AzinfoProtection_UL.exe** [Microsoft Download Centeristä](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Voit varmistaa, että asennus onnistui tarkastelemalla Word-asia kirjaa ja varmistamalla, että **herkkyys** -vaihto ehto on käytettävissä **Aloitus** -väli lehdessä.
<br/>![Word-asia kirjan avattava suojaus-väli lehti.](../media/word-sensitivity.png)

Lisä tietoja on Ohje aiheessa [asiakas ohjelman asentaminen](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
