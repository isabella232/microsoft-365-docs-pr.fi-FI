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
ms.openlocfilehash: a3405207cd7d2d6565807ef0f3a51acbcb80409a
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165733"
---
# <a name="set-up-compliance-features"></a>Yhteensopivuusominaisuuksien määrittäminen

Microsoft 365 Business Premiumsisältää ominaisuuksia, jotka suojaavat tietojasi ja laitteitasi ja auttavat pitämään asiakkaiden ja asiakkaidesi arkaluonteiset tiedot turvassa.

## <a name="set-up-dlp-features"></a>DLP-ominaisuuksien määrittäminen

Lisätietoja [dlp-käytännön luomisesta mallista](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) on kohdassa, miten voit määrittää käytännön, joka suojaa henkilökohtaisilta tunnisteilta (PII). 
  
DLP sisältää monia käyttövalmiita käytäntömalleja monille eri kielille. Esimerkiksi Australia Financial Data, Canada Personal Information Act, Yhdysvaltain taloudelliset tiedot ja niin edelleen. Täydellinen luettelo on [kohdassa, mitä DLP-käytäntömallit sisältävät.](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) Kaikki nämä mallit voidaan ottaa käyttöön samalla tavalla kuin pii-malliesimerkki. 
  
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
