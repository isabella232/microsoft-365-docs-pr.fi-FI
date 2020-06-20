---
title: Microsoft 365 Business Premiumin uhkasuojauksen lisääminen
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
description: Määritä yhteensopivuusominaisuudet, jotka estävät tietojen häviämisen ja auttavat pitämään sinun ja asiakkaidesi arkaluonteiset tiedot turvassa.
ms.openlocfilehash: 18886ff3a0ba5e99e63c70ef083d7a69c75bac91
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785828"
---
# <a name="set-up-compliance-features"></a>Yhteensopivuusominaisuuksien määrittäminen

Microsoft 365 Business Premiumissa on ominaisuuksia, jotka suojaavat tietojasi ja laitteitasi ja auttavat pitämään ja asiakkaidesi arkaluonteiset tiedot turvassa.

## <a name="set-up-dlp-features"></a>DLP-ominaisuuksien määrittäminen

Lisätietoja henkilökohtaisesti tunnistettavien tietojen suojaavan käytännön määrittämisestä on kohdassa [DLP-käytännön luominen mallista](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) mallista. 
  
DLP sisältää monia käyttövalmiita käytäntömalleja monille eri kielille. Esimerkiksi Australian taloudelliset tiedot, Kanadan henkilötietolaki, Yhdysvaltain taloudelliset tiedot ja niin edelleen. Täydellinen luettelo on kohdassa [DLP-käytäntömallien merkinnät.](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) Kaikki nämä mallit voidaan ottaa käyttöön samalla tavalla kuin PII-malliesimerkki. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Sähköpostin säilyttämisen määrittäminen Exchange Online Archivingin avulla

 **Exchange Online Archiving -käyttöoikeusominaisuudet** auttavat ylläpitämään vaatimustenmukaisuutta ja sääntelystandardeja säilyttämällä eDiscoveryn sähköpostisisällön. Se auttaa myös vähentämään riskiä, jos on oikeusjuttu, ja tarjoaa tavan palauttaa tietoja tietoturvaloukkauksen jälkeen tai kun haluat palauttaa poistetut kohteet. Oikeustoimiin liittyvän pidon avulla voit säilyttää käyttäjän kaiken sisällön tai mukauttaa säilytettävää sisältöä säilytyskäytäntöjen avulla.
  
**Riita-asioiden pito:** Voit säilyttää kaiken postilaatikon sisällön, poistetut kohteet mukaan lukien, asettamalla käyttäjän koko postilaatikon oikeustoimiin liittyvään pitoon. 
    
Voit sijoittaa postilaatikon oikeustoimiin liittyvään pitoon hallintakeskuksessa seuraavasti:
    
1. Siirry vasemmassa siirtymisruudussa **Käyttäjät** \> **Aktiiviset käyttäjät -kohtaan**.
    
2. Valitse käyttäjä, jonka postilaatikon haluat sijoittaa oikeustoimiin liittyvään pitoon. Laajenna käyttäjäruudussa **Sähköpostiasetukset**ja valitse **Lisää asetuksia -kohdan**vieristä **Muokkaa Exchange-ominaisuuksia**.
    
3. Valitse käyttäjän postilaatikkosivulla ** postilaatikon ominaisuudet ** vasemmassa siirtymisruudussa ja valitse sitten **Ota** käyttöön -linkki **Oikeustoimiin pito -kohdassa.**
    
4. **Oikeustoimiin liittyvän pidon** valintaikkunassa voit määrittää oikeustoimiin liittyvän pidon keston **Oikeustoimiin liittyvän pidon kesto** -kentässä. Jätä kenttä tyhjäksi, jos haluat asettaa äärettömän pidon. Voit myös lisätä muistiinpanoja ja ohjata postilaatikon omistajan sivustoon, jossa saatat joutua selittämään lisää oikeustoimiin liittyvästä pidosta. \>**Tallenna.**
    
**Säilyttäminen:** Voit ottaa mukautetut säilytyskäytännöt käyttöön esimerkiksi tietyn ajan tai poistaa sisällön pysyvästi säilytysajan lopussa. Lisätietoja on [ohjeaiheessa Säilytyskäytäntöjen yleiskatsaus](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).

## <a name="set-up-sensitivity-labels"></a>Herkkyysotsikoiden määrittäminen

Herkkyystarrojen mukana tulee Azure Information Protection (AIP) -palvelupaketti 1, ja niiden avulla voit luokitella ja vaihtoehtoisesti suojata asiakirjoja ja sähköposteja käyttämällä tarroja. Tunnisteita voivat käyttää automaattisesti järjestelmänvalvojat, jotka määrittävät sääntöjä ja ehtoja, käyttäjät voivat käyttää niitä manuaalisesti tai käyttämällä yhdistelmää, jossa käyttäjille annetaan suosituksia.

Voit määrittää Herkkyystarrat-toiminnolla [tarkastelemaan herkkyystarrojen videon luomista ja hallintaa.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)



### <a name="install-the-azure-information-protection-client-manually"></a>Azure Information Protection -asiakasohjelman asentaminen manuaalisesti

AIP-asiakkaan asentaminen manuaalisesti:

1. Lataa **AzinfoProtection_UL.exe** Microsoft [download centeristä](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Voit varmistaa, että asennus toimi tarkastelemalla Word-asiakirjaa ja varmistamalla, että **Herkkyys-vaihtoehto** on käytettävissä **Aloitus-välilehdessä.**
<br/>![Word-asiakirjan avattava suojaus-välilehti.](../media/word-sensitivity.png)

Lisätietoja on [ohjeaiheessa Asiakkaan asentaminen](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
