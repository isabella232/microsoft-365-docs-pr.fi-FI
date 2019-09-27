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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Määritä Office 365 Advanced uhkien torjunta ja suojaa arkaluontoisia tietoja.
ms.openlocfilehash: 8144bcebe8a0cdf28a5e092f592362922ccbdd48
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288741"
---
# <a name="set-up-compliance-features"></a>Yhteensopivuus ominaisuuksien määrittäminen

Microsoft 365-yritys sisältää ominaisuuksia, jotka suojaavat tietojasi ja laitteitasi sekä auttavat pitämään omasi ja asiakkaidesi arkaluonteiset tiedot turvassa.

## <a name="set-up-dlp-features"></a>DLP-ominaisuuksien määrittäminen

Katso [Luo DLP-käytäntö mallista](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) esimerkkinä siitä, miten voit määrittää käytännön suojaamaan henkilökohtaisia tunniste tietoja (pii) vastaan. 
  
DLP sisältää monia valmiita käytäntö malleja monille eri kieli alueilla. Esimerkiksi Australian taloudelliset tiedot, Kanadan henkilö tieto laki, Yhdysvaltain taloudelliset tiedot jne. Katso, [mitä DLP-käytäntö mallit sisältävät](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) täydellisestä luettelosta. Kaikki nämä mallit voidaan ottaa käyttöön samanlaisiksi kuin PII-malli esimerkki. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Sähkö postin säilyttämisen määrittäminen Exchange Online-arkistoinnin avulla

 **Exchange Online-arkistointi** lisenssi ominaisuudet auttavat ylläpitämään yhteensopivuus-ja sääntely standardeja säilyttämällä Sähkö posti sisällön eDiscovery. Se auttaa myös vähentämään riskiä tapa uksessa oikeus juttu ja tarjoaa tapa palauttaa tietoja, kun tieto turva loukkaus, tai kun haluat palauttaa poistetut kohteet. Voit säilyttää kaikki käyttäjän sisällöt tai käyttää säilytys käytäntöjä, kun haluat muokata säilytetä.
  
**Oikeuden käyntien pito:** Voit säilyttää kaiken posti laatikon sisällön, mukaan lukien poistetut kohteet, asettamalla käyttäjän koko posti laatikon oikeus riita-asioihin. 
    
Voit sijoittaa posti laatikon oikeuden käyntiin pitämällä hallinta keskuksessa:
    
1. Siirry vasemmassa siirtymis osassa **käyttäjät** \> **aktiiviset käyttäjät**-kohtaan.
    
2. Valitse käyttäjä, jonka posti laatikon haluat sijoittaa oikeuden käyntien pito-ja käyttäjä ruudussa Laajenna Mail- **Asetukset** ja valitse **Lisää asetuksia** -kohdasta **Muokkaa Exchangen ominaisuuksia**.
    
3. Valitse käyttäjän posti laatikko-sivulla * * posti laatikon ominaisuudet * * vasemmassa NAV-ohjelmassa ja valitse sitten **Ota käyttöön** -linkki kohdassa **oikeuden käynti pito**.
    
4. Voit määrittää **riita-** asioiden pito-valinta ikkunassa oikeuden käynnin keston kesto-kentässä, jätä kenttä tyhjäksi, jos haluat sijoittaa äärettömän **pito ajan.** Voit myös lisätä muistiinpanoja ja ohjata posti laatikon omistajan sivustoon, jossa saatat joutua selittämään lisää riita-asioiden pito \> - **säästä**.
    
**Säilyttäminen:** Voit ottaa käyttöön mukautetut säilytys käytännöt, esimerkiksi säilyttää tietyn ajan tai poistaa sisällön pysyvästi säilytys ajan päätyttyä. Lisä tietoja [on kohdassa säilytys käytäntöjen yleiskatsaus](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-azure-information-protection-features"></a>Azure-tietojen suojaus ominaisuuksien määrittäminen

Azure Information Protection (AIP) auttaa luokittelemaan ja valinnaisesti suojaamaan asia kirjoja ja sähkö posteja käyttämällä tunnisteita. Järjestelmänvalvojat voivat käyttää otsikoita automaattisesti, jos käyttäjät määrittävät säännöt ja ehdot manuaalisesti, tai käyttämällä yhdistelmää, jossa käyttäjille annetaan suosituksia.

Outlookissa verkossa voit käyttää seuraavia sisäänrakennettuja tarroja ja rajoituksia sähkö posteihin:
  
- **Älä välitä**: vastaanottajat voivat lukea viestin, mutta he eivät voi välittää, tulostaa tai kopioida sisältöä
    
- **Salaa**: koko viesti on salattu. Vastaanottajien on vahvistettava henkilöllisyytensä ennen salatun sisällön käyttämistä, eivätkä ne voi poistaa salausta.
    
- **Luottamuksellinen**: antaa organisaation työn tekijöille täydet oikeudet sähkö postin sisältöön ja liitteisiin, mutta ei organisaatiosi ulkopuolisille henkilöille. Tietojen omistajat voivat seurata ja kumota sisältöä missä tahansa vaiheessa.
    
- **Erittäin luottamuksellinen**: tätä rajoitusta voidaan soveltaa erittäin luottamuksellisiin tietoihin, jolloin työn tekijät voivat tarkastella, muokata ja vastata, mutta eivät välittää, tulostaa tai kopioida tietoja. Tietojen omistajat voivat seurata ja kumota sisältöä missä tahansa vaiheessa.

### <a name="make-sure-azure-information-protection-is-activated"></a>Varmista, että Azure-tietojen suojaus on aktivoitu

Voit varmistaa, että AIP on aktivoitu:

1. Kirjaudu sisään [Azure-portaaliin](https://portal.azure.com/).

2. Valitse **Kaikki palvelut** ja kirjoita *Azure-tietojen suojaus* **haku ruutuun**.

3. Kun tulokset ovat näytössä, napsauta Aloita **Azure-tietojen suoja** uksen vieressä, jotta se on suosikki ja helppo löytää myöhemmin.

4. Valitse **Azure-tieto suoja** \> **uksen Akti vointi** ja varmista, että tilaksi on määritetty aktivoitu. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Näytä Azure-tietojen suojaus käytäntö ja oletus otsikot 

Voit tarkastella ja muokata olemassa olevia otsikoita:

1. Valitse Azure-tieto suojan koonti näytössä **luokitusten** \> **otsikot**. <br/>![Azure-tietojen suoja uksen vakio merkinnät.](media/AIPLabels.png)

2. Voit valita minkä tahansa otsikon nähdäksesi vaihto ehtoja, voit muuttaa näyttö nimeä, värejä jne.
 
3. Jos haluat luoda omia tunnisteita, katso [Muokkaa ja luo uusia tarroja](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) . 

### <a name="install-the-azure-information-protection-client-manually"></a>Azure-tieto suoja asiakkaan asentaminen manuaalisesti

Voit asentaa AIP-asiakkaan manuaalisesti:

1. Lataa **Azinfoprotection. exe** [Microsoft Download Centeristä](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Voit varmistaa, että asennus on toiminut tarkastelemalla Word-asia kirjaa ja varmistamalla, että **suojaa** -vaihto ehto on käytettävissä **Aloitus** -väli lehdellä. <br/>![Word-asia kirjan avattava suojaus-väli lehti.](media/Word_Protect.png)

Lisä tietoja [on kohdassa asiakkaan asentaminen](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
