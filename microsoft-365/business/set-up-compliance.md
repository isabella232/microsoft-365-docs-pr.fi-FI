---
title: Nosta uhkien Microsoft 365 Business Premium
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Vaatimustenmukaisuusominaisuuksien avulla voit estää tietojen menettämisen ja pitää asiakkaan ja asiakkaan luottamukselliset tiedot suojattuina.
ms.openlocfilehash: 945f8a283b90b89da2fbe67a073e0807b80d198f
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245080"
---
# <a name="set-up-compliance-features"></a>Yhteensopivuusominaisuuksien täytäminen

Oma Microsoft 365 Business Premium sisältää ominaisuuksia, joilla voit suojata tietojasi ja laitteitasi ja auttaa sinua pitämään sekä asiakkaidesi luottamukselliset tiedot suojattuina.

## <a name="set-up-dlp-features"></a>DLP-ominaisuuksien asetusten

Katso [DLP-käytännön luominen mallista,](../compliance/create-a-dlp-policy-from-a-template.md) jos haluat esimerkiksi määrittää käytännön, joka suojaa henkilökohtaisten tietojen menetykseltä. 
  
DLP sisältää useita käyttövalmiita käytäntömalleja monille eri kielille. Esimerkki: Australia Financial Data, Canada Personal Information Act, Yhdysvaltain taloudelliset tiedot ja niin edelleen. Täydellinen [luettelo on kohdassa Mitä DLP-käytäntömallit](../compliance/what-the-dlp-policy-templates-include.md) sisältävät. Kaikki nämä mallit voidaan ottaa käyttöön samalla tavalla kuin PII-malliesimerkki. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Sähköpostin säilytysajan määrittäminen Exchange Online Archiving

 **Exchange Online Archiving** käyttöoikeuksien ominaisuudet auttavat säilyttämään vaatimustenmukaisuus- ja sääntelystandardit säilyttämällä eDiscoveryn sähköpostisisällön. Se myös vähentää riskiä, jos oikeusjutun on olemassa, ja tarjoaa keinon tietojen palauttamiseen suojausrikkomuksen jälkeen tai silloin, kun haluat palauttaa poistetut kohteet. Oikeuskäytännön avulla voit säilyttää käyttäjän kaiken sisällön tai mukauttaa säilytettävät sisällöt säilytyskäytäntöjen avulla.
  
**Oikeus oikeusistuntoon pito:** Voit säilyttää postilaatikon kaiken sisällön poistetut kohteet mukaan lukien asettamalla käyttäjän koko postilaatikon oikeusistuntoon. 
    
Voit sijoittaa postilaatikon oikeusistuntoon hallintakeskuksessa:
    
1. Valitse vasemmassa siirtymispalkin siirtymispalissa  \> **Käyttäjät, jotka ovat aktiivisia.**
    
2. Valitse käyttäjä, jonka postilaatikon haluat sijoittaa oikeus oikeusistuntoon. Laajenna käyttäjäruudussa **Postiasetukset ja** valitse Lisää asetuksia **-kohdan vierestä** **Muokkaa Exchange ominaisuuksia**.
    
3. Valitse käyttäjän postilaatikkosivulla ** postilaatikon ominaisuudet ** vasemmassa siirtymispalkin siirtymispalissa ja valitse sitten Ota **käyttöön** -linkki oikeus **hallintapito -kohdassa.**
    
4. **Riitautuksen pitovalintaikkunassa** voit määrittää oikeusistuinten pitokentän **keston.** Jätä kenttä tyhjäksi, jos haluat sijoittaa äärettömän pitoon. Voit myös lisätä muistiinpanoja ja ohjata postilaatikon omistajan verkkosivustoon, jossa sinun on ehkä selitettävä enemmän oikeus oikeusistuntoon liittyen. \>**Tallenna**.
    
**Säilytys:** Voit ottaa käyttöön mukautettuja säilytyskäytäntöjä, jos esimerkiksi haluat säilyttää tietyn ajan tai poistaa sisältöä pysyvästi säilytysajan lopussa. Lisätietoja on kohdassa [Säilytyskäytäntöjen yleiskatsaus.](../compliance/retention.md)

## <a name="set-up-sensitivity-labels"></a>Luottamuksellisuusotsikoiden valitseminen

Luottamuksellisuustunnisteet on varustettu Azure Information Protection (AIP) -palvelupaketti 1:llä, ja niiden avulla voit luokitella ja halutessasi suojata asiakirjoja ja sähköposteja käyttämällä tarroja. Järjestelmänvalvojat, jotka määrittävät säännöt ja ehdot, voivat ottaa selitteet käyttöön automaattisesti, käyttäjien manuaalisesti tai yhdistelmällä, jossa käyttäjille annetaan suosituksia.

Jos haluat määrittää luottamuksellisuusotsikot, katso [luottamuksellisuusotsikoiden](../business-video/create-sensitivity-labels.md) luominen ja hallinta -video.



### <a name="install-the-azure-information-protection-client-manually"></a>Azure Information Protection -asiakasohjelman asentaminen manuaalisesti

AIP-asiakasohjelman asentaminen manuaalisesti:

1. Lataa **AzinfoProtection_UL.exe** Microsoft [Download Centeristä.](https://www.microsoft.com/download/details.aspx?id=53018)
 
2. Voit tarkistaa asennuksen toimimisen tarkastelemalla Word-asiakirjaa  ja varmistamalla, että Luottamuksellisuus-vaihtoehto on käytettävissä **Aloitus-välilehdessä.**
<br/>![Word-asiakirjan avattava Suojaus-välilehti.](../media/word-sensitivity.png)

Lisätietoja on kohdassa [Asiakkaan asentaminen.](/azure/information-protection/infoprotect-tutorial-step3)