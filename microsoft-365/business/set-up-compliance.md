---
title: Lisää Microsoft 365 Business Premiumin uhkasuojausta
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
search.appverid:
- BCS160
- MET150
description: Määritä yhteensopivuusominaisuudet, jotka estävät tietojen häviämisen ja auttavat pitämään asiakkaiden ja asiakkaidesi arkaluonteiset tiedot turvassa.
ms.openlocfilehash: 523d020587bcf16e46263b88ee7654b9c786e7a2
ms.sourcegitcommit: 5476c2578400894640ae74bfe8e93c3319f685bd
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/06/2020
ms.locfileid: "44048061"
---
# <a name="set-up-compliance-features"></a>Yhteensopivuusominaisuuksien määrittäminen

Microsoft 365 Business Premiumsisältää ominaisuuksia, jotka suojaavat tietojasi ja laitteitasi ja auttavat pitämään asiakkaiden ja asiakkaidesi arkaluonteiset tiedot turvassa.

## <a name="set-up-dlp-features"></a>DLP-ominaisuuksien määrittäminen

Lisätietoja [dlp-käytännön luomisesta mallista](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) on kohdassa, miten voit määrittää käytännön, joka suojaa henkilökohtaisilta tunnisteilta (PII). 
  
DLP sisältää monia käyttövalmiita käytäntömalleja monille eri kielille. Esimerkiksi Australia Financial Data, Canada Personal Information Act, Yhdysvaltain taloudelliset tiedot ja niin edelleen. Täydellinen luettelo on [kohdassa, mitä DLP-käytäntömallit sisältävät.](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) Kaikki nämä mallit voidaan ottaa käyttöön samalla tavalla kuin pii-malliesimerkki. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Sähköpostin säilyttämisen määrittäminen Exchange Online -arkistoinnin avulla

 **Exchange OnlineArchiving -käyttöoikeusominaisuudet** auttavat ylläpitämään vaatimustenmukaisuus- ja sääntelystandardeja säilyttämällä eDiscovery-sähköpostin sisällön. Se auttaa myös vähentämään riskiä, jos on oikeusjuttu, ja tarjoaa tavan palauttaa tietoja tietoturvaloukkauksen jälkeen tai kun sinun täytyy palauttaa poistetut kohteet. Oikeustoimiin liittyvän pidon avulla voit säilyttää käyttäjän koko sisällön tai mukauttaa säilytettävääsi sisältöä säilytyskäytäntöjen avulla.
  
**Oikeustoimiin liittyvä pito:** Voit säilyttää kaiken postilaatikon sisällön, poistetut kohteet mukaan lukien, asettamalla käyttäjän koko postilaatikon oikeustoimiin liittyvään pitoon. 
    
Postilaatikon sijoitaminen oikeustoimiin liittyvään pitoon hallintakeskuksessa:
    
1. Valitse vasemmasta siirtymisruudusta **Käyttäjät** \> **aktiiviset käyttäjät**.
    
2. Valitse käyttäjä, jonka postilaatikon haluat sijoittaa oikeustoimiin liittyvään pitoon. Laajenna käyttäjäruudussa **Mailin asetukset**ja valitse **Lisää asetuksia**-kohdan vierestä **Muokkaa Exchange-ominaisuuksia**.
    
3. Valitse käyttäjän postilaatikkosivulla ** postilaatikon ominaisuudet ** vasemmasta siirtymisruudusta ja valitse sitten **Ottaminen-linkki** **Oikeustoimiin liittyväpito**-kohdasta.
    
4. **Oikeustoimiin liittyvän pidon** valintaikkunassa voit määrittää oikeustoimiin liittyvän pidon keston **Oikeustoimiin liittyvän pidon kesto** -kentässä. Jätä kenttä tyhjäksi, jos haluat sijoittaa äärettömän pidon. Voit myös lisätä muistiinpanoja ja ohjata postilaatikon omistajan sivustoon, jota saatat joutua selittämään lisätietoja oikeustoimiin liittyvästä pidon pidon. \>**Tallenna.**
    
**Säilyttäminen:** Voit ottaa käyttöön mukautetut säilytyskäytännöt, esimerkiksi säilyttää tietyn ajan tai poistaa sisältöä pysyvästi säilytysajan lopussa. Lisätietoja on [ohjeaiheessa Säilytyskäytäntöjen yleiskatsaus](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).

## <a name="set-up-sensitivity-labels"></a>Herkkyysotsikoiden määrittäminen

Herkkyysotsikoissa on Azure Information Protection (AIP) Plan 1, ja ne auttavat sinua luokittelemaan ja halutessasi suojaamaan asiakirjoja ja sähköposteja käyttämällä tarroja. Sääntöjä voivat käyttää automaattisesti järjestelmänvalvojat, jotka määrittävät säännöt ja ehdot manuaalisesti käyttäjien toimesta, tai käyttämällä yhdistelmää, jossa käyttäjille annetaan suosituksia.

Voit määrittää herkkyysotsikot tarkastelemaan [luojaa ja hallitsemaan herkkyystarroja- videota.](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)



### <a name="install-the-azure-information-protection-client-manually"></a>Azure Information Protection -asiakkaan asentaminen manuaalisesti

AIP-asiakkaan asentaminen manuaalisesti:

1. Download **AzinfoProtection_UL.exe** polveutua [Mikroskooppi download keskittyä](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Voit varmistaa, että asennus toimi tarkastelemalla Word-asiakirjaa ja varmistamalla, että **Herkkyys-vaihtoehto** on käytettävissä **Aloitus-välilehdessä.**
<br/>![Word-asiakirjan Suojaus-välilehden avattava.](../media/word-sensitivity.png)

Lisätietoja on [ohjeaiheessa Asiakkaan asentaminen](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
