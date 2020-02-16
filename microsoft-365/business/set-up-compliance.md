---
title: Lisää Microsoft 365 Businessin uhkien suojausta
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
search.appverid:
- BCS160
- MET150
description: Määritä yhteensopivuusominaisuudet tietojen häviämisen estämiseksi ja arkojen tietojen merkitsemiseksi.
ms.openlocfilehash: d569ff8d84faf82881035f0ed54e5d175605776f
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2020
ms.locfileid: "42064697"
---
# <a name="set-up-compliance-features"></a>Yhteensopivuusominaisuuksien määrittäminen

Microsoft 365 Businessin mukana toimitetaan ominaisuuksia, jotka suojaavat tietojasi ja laitteitasi ja auttavat pitämään omasi ja asiakkaidesi arkaluonteiset tiedot turvassa.

## <a name="set-up-dlp-features"></a>DLP-ominaisuuksien määrittäminen

Lisätietoja on [ohjeaiheessa DLP-käytännön luominen mallista,](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) jossa on esimerkki siitä, miten voit määrittää käytännön, joka suojaa henkilökohtaisilta tiedovoilta. 
  
DLP sisältää monia käyttövalmiita käytäntömalleja monille eri maa-asetustoille. Esimerkiksi Australia Financial Data, Canada Personal Information Act, Yhdysvaltain taloudelliset tiedot ja niin edelleen. Täydellinen luettelo on kohdassa [DLP-käytäntömallien sisältämät](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) tiedot. Kaikki nämä mallit voidaan ottaa käyttöön samalla tavalla kuin PII-malliesimerkki. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Sähköpostin säilyttämisen määrittäminen Exchange Online -arkistoinnin avulla

 **Exchange Online Archiving -käyttöoikeusominaisuudet** auttavat ylläpitämään vaatimustenmukaisuus- ja sääntelystandardeja säilyttämällä eDiscovery-sähköpostin sisällön. Se auttaa myös vähentämään riskiä, jos on oikeusjuttu, ja tarjoaa tavan palauttaa tietoja tietoturvaloukkauksen jälkeen tai kun sinun täytyy palauttaa poistetut kohteet. Oikeustoimiin liittyvän pidon avulla voit säilyttää käyttäjän kaiken sisällön tai mukauttaa säilytettävää sisältöä säilytyskäytäntöjen avulla.
  
**Oikeudenkäyntien pito:** Voit säilyttää kaiken postilaatikon sisällön, poistetut kohteet mukaan lukien, asettamalla käyttäjän koko postilaatikon oikeustoimiin liittyvään pitoon. 
    
Postilaatikon lisääminen oikeustoimiin liittyvään pitoon hallintakeskuksessa:
    
1. Siirry vasemmassa siirtymisruudussa **Käyttäjät aktiiviset** \> **käyttäjät**.
    
2. Valitse käyttäjä, jonka postilaatikon haluat sijoittaa oikeustoimiin liittyvään pitoon. Laajenna käyttäjäruudussa **Sähköpostiasetukset**ja valitse **Lisää asetuksia**-kohdan vierestä Muokkaa **Exchange-ominaisuuksia**.
    
3. Valitse käyttäjän postilaatikkosivulla ** postilaatikon ominaisuudet ** vasemmasta siirtymisruudusta ja valitse sitten **Ota käyttöön** -linkki **kohdassa Oikeustoimiin liittyvä pito**.
    
4. **Oikeustoimiin liittyvän pidon** valintaikkunassa voit määrittää oikeustoimiin liittyvän pidon keston **Oikeustoimiin liittyvän pidon kesto** -kentässä. Jätä kenttä tyhjäksi, jos haluat asettaa äärettömän pidon. Voit myös lisätä muistiinpanoja ja ohjata postilaatikon omistajan verkkosivustoon, jota saatat joutua selittämään lisätietoja oikeustoimiin liittyvästä pidon pidon säilyttämisestä. \>**Tallenna.**
    
**Säilyttäminen:** Voit ottaa käyttöön mukautetut säilytyskäytännöt, esimerkiksi säilyttää tietyn ajan tai poistaa sisältöä pysyvästi säilytysajan lopussa. Lisätietoja on ohjeaiheessa [Säilytyskäytäntöjen yleiskatsaus](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-sensitivity-labels"></a>Herkkyysotsikoiden määrittäminen

Herkkyysotsikot tulevat Azure Information Protection (AIP) -palvelupaketin 1 mukana, ja ne auttavat sinua luokittelemaan ja suojaamaan asiakirjoja ja sähköposteja ja suojaamaan ne valinnaisesti käyttämällä tunnisteita. Otsikoita voivat käyttää automaattisesti järjestelmänvalvojat, jotka määrittävät säännöt ja ehdot manuaalisesti käyttäjät, tai käyttämällä yhdistelmää, jossa käyttäjille annetaan suosituksia.

Voit määrittää herkkyysotsikot [tarkastelemaan herkkyystarrojen videon luomista ja hallintaa.](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)



### <a name="install-the-azure-information-protection-client-manually"></a>Azure Information Protection -asiakasohjelman asentaminen manuaalisesti

AIP-asiakasohjelman asentaminen manuaalisesti:

1. Lataa **AzinfoProtection_UL.exe** [Microsoft download centeristä](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Voit varmistaa, että asennus toimi tarkastelemalla Word-asiakirjaa ja varmistamalla, että **Herkkyys-vaihtoehto** on käytettävissä **Aloitus-välilehdessä.**
<br/>![Word-asiakirjan avattava suojausvälilehti.](../media/word-sensitivity.png)

Lisätietoja on ohjeaiheessa [Asiakkaan asentaminen](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
