---
title: Suurenna Microsoft 365 Business suojaa uhka
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
search.appverid:
- BCS160
- MET150
description: 'Määrittäminen Office 365: n Advanced Threat Protection ja luottamuksellisten tietojen turvaamiseksi.'
ms.openlocfilehash: 53741a7726222bb32329a401953be72257df95cc
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086314"
---
# <a name="set-up-compliance-features"></a>Määritä yhteensopivuuden ominaisuudet

Microsoft 365 liiketoiminnan mukana ominaisuuksia suojaa tietoja ja laitteita ja auttaa pitämään teille ja asiakkaiden luottamukselliset tiedot turvassa.

## <a name="set-up-dlp-features"></a>DLP-ominaisuuksien määrittäminen

Katso [luominen mallista DLP käytännön](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) esimerkki siitä, kuinka voit määrittää käytännön henkilökohtaisia tietoja (henkilökohtaisia tietoja) vastaan. 
  
DLP mukana monta monta eri kieliversioiden valmis avulla käytännön malleja. Taloudellisia tietoja Australian, Kanadan Personal Information Act, Yhdysvaltain taloudellisten tietojen, esimerkiksi jne. Saat täydellisen luettelon [mitä DLP-Käytäntömallit ovat](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) . Kaikki mallit voidaan ottaa käyttöön henkilökohtaisia tietoja malli esimerkin. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Määritä Exchange Online arkistoida kanssa sähköpostin säilytys

 Käyttöoikeuden ominaisuuksia **Exchange Online arkistoida** auttaa säilyttämään vaatimusten ja standardien säilytät sähköpostin sisällön eDiscovery. Se myös auttaa Jos Oletteko varotoimia ja avulla voit palauttaa tietoja turvallisuusongelmista jälkeen tai kun haluat palauttaa poistettuja kohteita. Voit käyttää oikeudenkäyntiä pitoon säilyttää käyttäjän sisällön tai säilytyskäytännöt avulla voit mukauttaa haluat säilyttää.
  
**Pito oikeudenkäyntiä:** Voit säilyttää kaikki postilaatikon sisältö mukaan lukien poistetut sijoittamalla käyttäjän postilaatikon koko oikeudenkäyntiä, pidä. 
    
Voit sijoittaa oikeudenkäyntiä postilaatikkoon hold Admin Centerissä:
    
1. Siirry vasemman nav- **käyttäjät** \> **aktiivisia käyttäjiä**.
    
2. Valitse käyttäjä, jonka postilaatikon haluat sijoittaa oikeudenkäyntiä pidä laajentaa käyttäjän ruudun **Sähköpostiasetukset** ja valita **Lisää asetuksia** -kohdan vieressä **Muokkaa Exchange-ominaisuudet**.
    
3. Valitse käyttäjän postilaatikko-sivulla ** postilaatikon ominaisuuksia ** vasemman nav-painiketta ja valitsemalla sitten **Ota käyttöön** -linkki **pidossa oikeudellisten toimien**mukaisesti.
    
4. Valintaikkunassa voit määrittää kanne **oikeusjutun pidä** pidä kesto **pidossa oikeudellisten toimien kesto** -kenttään, jätä kenttä tyhjäksi, jos haluat sijoittaa äärettömän pito. Voit myös lisätä muistiinpanoja ja direct mail ruutuun omistaja Web-sivustoon saattaa olla lisätietoja kanne pitää selittää \> **Tallenna**.
    
**Säilyttäminen:** Voit ottaa käyttöön mukautetut säilytyskäytännöt, esimerkiksi säilyttää tietyn ajanjakson ajan tai poistaa sisällön pysyvästi säilytysajan päätyttyä. Lisätietoja on kohdassa [Yleiskatsaus säilytyskäytäntöjä](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-azure-information-protection-features"></a>Määritä Azure tietojen suojauksen ominaisuudet

Azure tietojen suojaus (järjestelmänvalvojan Asennuspiste) auttaa sinua luokitella ja myös suojata asiakirjoja tai sähköpostiviestejä, ja soveltamalla otsikot. Otsikoita voi käyttää automaattisesti järjestelmänvalvojille, jotka määrittävät säännöt ja ehdot, manuaalisesti käyttäjät tai käyttämällä yhdistelmää, jossa käyttäjille annetaan suosituksia.

Outlookin web-voit käyttää sisäänrakennettu seuraavat otsikot ja rajoitukset että sähköpostit:
  
- **Älä lähetä edelleen**: vastaanottajat voivat lukea viestin, mutta ne ei eteenpäin, tulostaa tai kopioida sen sisältöä
    
- **Salaa**: koko viesti on salattu. Vastaanottajien on henkilöllisyytensä ennen salatun sisällön käyttämistä ja salausta ei voi poistaa.
    
- **Luottamuksellinen**: organisaation työntekijät antaa täydet oikeudet, sähköposti ja liitteet, mutta ei oman organisaation ulkopuolisille henkilöille. Tietojen omistajat voivat seurata ja sisältöä milloin tahansa peruuttaa.
    
- **Erittäin luottamuksellisia**: Tämä rajoitus voidaan ottaa käyttöön erittäin luottamuksellisia tietoja, joiden avulla työntekijät voivat tarkastella, muokata, ja vastata, mutta ei välittää, tulostaa tai kopioida tiedot. Tietojen omistajat voivat seurata ja sisältöä milloin tahansa peruuttaa.

### <a name="make-sure-azure-information-protection-is-activated"></a>Varmista, että Azure tietojen suojaus on käytössä.

Tarkista, että järjestelmänvalvojan Asennuspiste on käytössä:

1. Kirjaudu [Azure](https://portal.azure.com/)portaaliin.

2. Valitse **kaikki palvelut** ja kirjoita **Hakukenttään** *Azure tietojen suojaaminen* .

3. Kun näkyviin, napsauta Käynnistä-painiketta, seuraava **Azure tietojen suojaus** jotta suosikki ja helppo löytää myöhemmin.

4. Valitse **Azure tietojen suojaus** \> **Suojaus aktivointi** ja tehdä Varmista, että otat voi aktivoitua. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Näytä Azure tietojen suojaaminen ja käytännön oletusarvon otsikot 

Voit tarkastella ja muokata, olemassa olevat otsikot:

1. Azure-tietojen suojaaminen kojelaudassa, valitse **luokitukset** \> **tarroja**. <br/>![Azure-tietojen suojaaminen vakio-otsikoita.](media/AIPLabels.png)

2. Voit valita kaikki otsikon Näytä asetukset, voit muuttaa nimen, värit jne.
 
3. Katso [Muokkaa ja luo uudet etiketit](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) Jos haluat luoda omia. 

### <a name="install-the-azure-information-protection-client-manually"></a>Tietojen suojaaminen Azure-asiakasohjelman asentaminen manuaalisesti

Manuaalisesti asentaminen järjestelmänvalvojan Asennuspiste-client:

1. **AzInfoProtection.exe** ladata [Microsoft download Centeristä](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Voit varmistaa, että Word-asiakirjan tarkasteleminen ja varmistamalla, että **Suojaa** -vaihtoehto on käytettävissä **Aloitus** -välilehden työskennelleet asennus. <br/>![Suojaus-välilehden avattavan Word-asiakirjan.](media/Word_Protect.png)

Lisätietoja on ohjeaiheessa [Asenna asiakkaan](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
