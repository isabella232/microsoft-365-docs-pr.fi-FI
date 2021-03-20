---
title: Microsoft 365 for Businessin uhkien uhkien suojauksen nostaminen
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
description: Määritä Microsoft Defender for Office 365 ja suojaa arkaluontoiset tiedot tietojen kalastelulta, haittaohjelmilta ja muilta uhilta.
ms.openlocfilehash: 0424fd56e30477f4e8d9e84b7ac78ba6255781fa
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913282"
---
# <a name="increase-threat-protection"></a>Uhkien uhkien suojauksen nostaminen

Tämän artikkelin avulla voit parantaa Microsoft 365 -tilauksesi suojausta tietojen kalastelulta, haittaohjelmilta ja muilta uhilta suojautumista varten. Nämä suositukset soveltuvat organisaatioille, joilla on entistä enemmän tietoturvan tarvetta, kuten lakitoimistot ja terveysalan ammattilaiset.

Tarkista Office 365 Secure Score ennen aloittamista. Office 365 Secure Score analysoi organisaatiosi suojauksen säännöllisten toimintojen ja suojausasetusten perusteella ja määrittää pistemäärän. Aloita merkitsemällä muistiin nykyinen pistemääräsi. Jos haluat kasvattaa pistemäärää, suorita tässä artikkelissa suositellut toimet. Tavoitteena ei ole saavuttaa suurinta pistemäärää, vaan se on tietoinen ympäristösi suojaamisen mahdollisuuksista, jotka eivät vaikuta haitallisesti käyttäjien tuottavuuteen.

Lisätietoja on kohdassa [Microsoft Secure Score.](../security/mtp/microsoft-secure-score.md)

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Nosta sähköpostin haittaohjelmasuojauksen tasoa

Office 365- tai Microsoft 365 -ympäristösi sisältää suojauksen haittaohjelmilta. Voit parantaa tätä suojausta estämällä liitetiedostot tiedostotyypeillä, joita käytetään yleisesti haittaohjelmissa. Voit parantaa haittaohjelmien estoa sähköpostissa:

1. Siirry [https://protection.office.com](https://protection.office.com) järjestelmänvalvojan tilin tunnistetiedoilla ja kirjaudu sisään.

2. Valitse Tietoturvakeskuksen &amp; vasemman siirtymisruudun Uhkien hallinta **-kohdassa** **Käytännön haittaohjelmien** \> **torjunta.**

3. Voit muokata koko yrityksen kattavaa käytäntöä kaksoisnapsauttamalla oletuskäytäntöä.

4. Valitse **Asetukset.**

5. Valitse **Yleiset liitetyypit -suodattimessa** **Käytössä.** Estetyt tiedostotyypit näkyvät suoraan tämän ohjausobjektin alapuolella olevassa ikkunassa. Varmista, että lisäät seuraavat tiedostotyypit:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   Voit tarvittaessa lisätä tai poistaa tiedostotyyppejä myöhemmin.

6. Valitse **Tallenna.**

Lisätietoja on [EOP:n haittaohjelmien estossa.](../security/office-365-security/anti-malware-protection.md)

## <a name="protect-against-ransomware"></a>Kiristysohjelmilta suojautuminen

Kiristysohjelmat rajoittavat tietojen käyttöä salaamalla tiedostoja tai lukitsemalla tietokoneen näyttöjä. Sen jälkeen se yrittää kiristystä kiristystä pyytämällä "kiristystä", joka on yleensä salatun valuutan, kuten Crypton, muodossa tietojen käytön vastineeksi.

Voit suojautua kiristysohjelmilta luomalla yhden tai useamman postinkulkusäännön, joka estää kiristysohjelmissa yleisesti käytetyt tiedostotunnisteet. (Olet lisännyt nämä säännöt [nostamaan suojaustasoa haittaohjelmilta sähköpostin vaiheessa.)](#raise-the-level-of-protection-against-malware-in-mail) Voit myös varoittaa käyttäjiä, jotka saavat nämä liitteet sähköpostitse.

Edellisessä vaiheessa estettyjen tiedostojen lisäksi on hyvä luoda sääntö, joka varoittaa käyttäjiä ennen makroja sisältävät Office-liitetiedostojen avaamista. Kiristysohjelmat voidaan piilottaa makrojen sisällä, joten varoita käyttäjiä avaamaan näitä tiedostoja käyttäjiltä, jotka eivät tunne heitä.

Sähköpostin siirtosäännön luominen:

1. Siirry hallintakeskukseen ja valitse <https://admin.microsoft.com> **Hallintakeskukset** \> **Exchange.**

2. Valitse **postinkulkuluokasta** **säännöt.**

3. Valitse **+** ja valitse sitten Luo uusi **sääntö.**

4. Saat **kaikki asetukset** näkyviin valitsemalla valintaikkunan alareunassa Lisää asetuksia.

5. Ota sääntöä varten käyttöön seuraavan taulukon asetukset. Käytä oletusarvoja muille asetuksille, ellet halua muuttaa niitä.

6. Valitse **Tallenna**.

|Asetus|Varoita käyttäjiä ennen Office-tiedostojen liitteiden avaamista||
|---|---|---|
|Nimi|Kiristysohjelmien estosääntö: varoita käyttäjiä|
|Käytä tätä sääntöä, jos . . .|Mikä tahansa liite. . . tiedostotunniste vastaa . . .|
|Sanojen tai lauseiden määritteleminen|Lisää seuraavat tiedostotyypit:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm|
|Tee seuraavat toimet. . .|Vastaanottajalle ilmoittaminen viestillä|
|Viestin tekstin lisääminen|Älä avaa tällaisia tiedostoja henkilöltä, jonka et tiedä, koska ne voivat sisältää haittaohjelmia sisältäviä makroja.|

Lisätietoja on seuraavissa artikkeleissa:

- [Kiristysohjelmat: riskien pienentäminen](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [OneDriven palauttaminen](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Sähköpostin automaattisen edelleenlähetysten pysäyttäminen

Hakkerit, jotka saavat käyttöoikeudet käyttäjän postilaatikkoon, voivat varastaa sähköpostia määrittämällä postilaatikon välittämään sähköpostit automaattisesti. Näin voi käydä myös ilman käyttäjän tietoja. Voit estää tämän määrittämällä postinkulkusäännön.

Jos haluat luoda sähköpostin siirtosäännön, katso [tämä lyhyt video](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) tai toimi seuraavasti:

1. Valitse Microsoft 365 -hallintakeskuksessa **Hallintakeskukset** \> **Exchange.**

2. Valitse **postinkulkuluokasta** **säännöt.**

3. Valitse **+** ja valitse sitten Luo uusi **sääntö.**

4. Jos haluat nähdä kaikki vaihtoehdot, **valitse** valintaikkunan alareunassa Lisää asetuksia.

5. Ota asetukset käyttöön seuraavassa taulukossa. Käytä oletusarvoja muille asetuksille, ellet halua muuttaa niitä.

6. Valitse **Tallenna**.

|Asetus|Varoita käyttäjiä ennen Office-tiedostojen liitteiden avaamista|
|---|---|
|Nimi|Sähköpostin automaattisen edelleenlähetysten estäminen ulkoisiin toimialueisiin|
|Käytä tätä sääntöä, jos ...|Lähettäjä. . . on ulkoinen/sisäinen. . . Organisaation sisällä|
|Lisää ehto|Viestin ominaisuudet. . . sisällytä viestityyppi. . . Automaattinen edelleenlähetys|
|Tee seuraavat toimet...|Estä viesti. . . hylkää viesti ja lisää selitys.|
|Viestin tekstin lisääminen|Tämän organisaation ulkopuolisen sähköpostin automaattinen edelleenlähetys estetään tietoturvasyistä.|


## <a name="protect-your-email-from-phishing-attacks"></a>Sähköpostin suojaaminen tietojenkalasteluhyökkäyksiltä

Jos olet määrittänyt yhden tai useamman mukautetun toimialueen Office 365- tai Microsoft 365 -ympäristöäsi varten, voit määrittää kohdennetun tietojen kalastelun torjunnan. Tietojen kalastelun esto, joka on osa Microsoft Defender for Office 365:tä, voi auttaa suojaamaan organisaatiotasi haitallisilta tekeytymisperusteisilta tietojenkalasteluhyökkäyksiltä ja muista tietojenkalasteluhyökkäyksiltä. Jos et ole määrittänyt mukautettua toimialuetta, sinun ei tarvitse tehdä tätä.

Suosittelemme, että aloitat tämän suojauksen käytön luomalla käytännön tärkeimpien käyttäjien ja mukautetun toimialueen suojaamiseksi.

Jos haluat luoda tietojenkalastelun torjunnan käytännön Microsoft Defender for Office 365:ssä, katso tämä lyhyt  [koulutusvideo](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)tai toimi seuraavasti:

1. Siirry osoitteeseen [https://protection.office.com](https://protection.office.com).

2. Valitse tietoturvakeskuksen &amp; vasemman siirtymisruudun Uhkien hallinta **-kohdassa** **Käytäntö.**

3. Valitse **Käytäntö-sivulla** **Tietojen kalastelun esto.**

4. Valitse **Tietojen kalastelun** esto -sivulla **+ Luo.** Ohjattu toiminto käynnistää tietojenkalastelun torjuntakäytännön määrittämisen.

5. Määritä käytännön nimi, kuvaus ja asetukset seuraavassa taulukossa suositellulla mukaisesti. Lisätietoja on microsoft Defender for [Office 365:n tietojenkalastelun estokäytännössä.](../security/office-365-security/set-up-anti-phishing-policies.md)

6. Kun olet tarkistanut asetukset, valitse Luo **tämä käytäntö tai** **Tallenna.**

|Asetus tai asetus|Suositeltu asetus|
|---|---|
|Nimi|Toimialue ja arvokkain kampanjahenkilökunta|
|Kuvaus|Varmista, että tärkeintä henkilökuntaa ja toimialuettamme ei tekeytetä.|
|Käyttäjien lisääminen suojattavaksi|Valitse **+ Lisää ehto, Vastaanottaja on**. Kirjoita käyttäjänimet tai anna ehdokkaan, kampanjapäällikön ja muiden tärkeiden henkilökunnan jäsenten sähköpostiosoitteet. Voit lisätä enintään 20 sisäistä ja ulkoista osoitetta, jotka haluat suojata tekeytymishenkilöltä.|
|Toimialueiden lisääminen suojattavaksi|Valitse **+ Lisää ehto, Vastaanottajan toimialue on**. Anna Microsoft 365 -tilaukseen liittyvä mukautettu toimialue, jos olet määrittänyt sellaisen. Voit kirjoittaa useamman kuin yhden toimialueen.|
|Toimintojen valinta|Jos käyttäjä on tekeytynyt käyttäjä lähettänyt sähköpostiviestin: Valitse Ohjaa viesti toiseen sähköpostiosoitteeseen ja kirjoita sitten suojauksen järjestelmänvalvojan sähköpostiosoite. Esimerkiksi *<span> 2010-201022 <span> @contoso.com.* Jos sähköpostin lähettää tekeytynyt toimialue: Valitse **Karanteeniviesti.**|
|Postilaatikkotiedot|Postilaatikon tiedot valitaan oletusarvoisesti, kun luot uuden tietojenkalastelun estokäytännön. Jätä tämä asetus **käyttöön,** niin saat parhaan tuloksen.|
|Luotettujen lähettäjien ja toimialueiden lisääminen|Tässä voit lisätä oman toimialueesi tai minkä tahansa muun luotetun toimialueen.|
|Käytössä:|Valitse **Vastaanottajan toimialue on**. Valitse **jokin näistä ja** valitse sitten **Valitse.** Valitse **+ Lisää.** Valitse toimialueen nimen vieressä oleva valintaruutu, esimerkiksi *contoso. <span> <span> com,* luettelosta ja valitse sitten **Lisää.** Valitse **Valmis.**|

## <a name="protect-against-malicious-attachments-and-files-with-safe-attachments"></a>Suojaa haitallisilta liitteiltä ja tiedostoilta turvallisten liitteiden avulla

Ihmiset lähettävät, vastaanottavat ja jakavat säännöllisesti liitteitä, kuten asiakirjoja, esityksiä, laskentataulukoita ja paljon muuta. Sähköpostiviestin avulla ei ole aina helppo tietää, onko liite turvallinen vai haitallinen. Microsoft Defender for Office 365 sisältää turvallisten liitteiden suojauksen, mutta tämä suojaus ei ole oletusarvoisesti käytössä. Suosittelemme, että luot uuden säännön tämän suojauksen käytön aloittamista varten. Tämä suojaus kattaa tiedostot SharePointissa, OneDrivessa ja Microsoft Teamsissa.

Voit luoda turvallisten liitteiden käytännön joko katsomalla [tämän lyhyen videon](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)tai toimimalla seuraavasti:

1. Siirry ja [https://protection.office.com](https://protection.office.com) kirjaudu sisään järjestelmänvalvojan tililläsi.

2. Valitse tietoturvakeskuksen &amp; vasemman siirtymisruudun Uhkien hallinta **-kohdassa** **Käytäntö.**

3. Valitse Käytäntö-sivulla **Turvalliset liitteet.**

4. Käytä tätä suojausta laajalti Turvalliset liitteet -sivulla valitsemalla Ota ATP käyttöön **SharePointissa, OneDrivessa ja Microsoft Teamsissa** -valintaruutu.

5. Luo **+** uusi käytäntö valitsemalla tämä.

6. Ota asetukset käyttöön seuraavassa taulukossa.

7. Kun olet tarkistanut asetukset, valitse **Luo tämä käytäntö** tai **Tallenna.**

|Asetus tai asetus|Suositeltu asetus|
|---|---|
|Nimi|Estä nykyiset ja tulevat sähköpostiviestit, joissa on havaittu haittaohjelma.|
|Kuvaus|Estä nykyiset ja tulevat sähköpostiviestit ja liitteet tunnistetuilla haittaohjelmilla.|
|Liitteiden tuntemattomien haittaohjelmien vastausten tallentaminen|Valitse **Estä – estä nykyiset ja tulevat sähköpostiviestit ja liitteet, joissa on havaittu haittaohjelma.**|
|Liitteen uudelleenohjaus tunnistuksen aikana|Ota uudelleenohjaus käyttöön (valitse tämä ruutu) Kirjoita järjestelmänvalvojan tili tai postilaatikon määritys karanteeniin.          Käytä yllä olevaa valintaa, jos liitteiden haittaohjelmien tarkistus aikaistaa tai tapahtuu virhe (valitse tämä ruutu).|
|Käytössä:|Vastaanottajan toimialue on . . . valitse toimialueesi.|

Lisätietoja on kohdassa Tietojenkalastelun [torjuntakäytäntöjen määritys Microsoft Defender for Office 365:ssä.](../security/office-365-security/set-up-anti-phishing-policies.md)

## <a name="protect-against-phishing-attacks-with-safe-links"></a>Tietojenkalasteluhyökkäyksiltä suojautuminen turvallisten linkkien avulla

Hakkerit piilottelevat joskus vahingollisia sivustoja sähköposteihin tai muihin tiedostoihin linkityksissä. Office 365:n Microsoft Defenderiin kuuluvat turvalliset linkit voivat auttaa suojaamaan organisaatiotasi antamalla sähköpostiosoitteiden ja Office-tiedostojen verkko-osoitteiden (URL-osoitteiden) napsautuksen aikavahvistuksen. Suojaus määritetään Turvallisten linkkien käytännöt -kohdassa.

Suosittelemme, että toimit seuraavasti:

- Voit parantaa suojausta muokkaamalla oletuskäytäntöä.

- Lisää uusi käytäntö, joka on kohdennettu toimialueen kaikille vastaanottajille.

Voit määrittää turvalliset linkit [katsomalla tämän lyhyen koulutusvideon](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)tai noudattamalla seuraavia ohjeita:

1. Siirry ja [https://protection.office.com](https://protection.office.com) kirjaudu sisään järjestelmänvalvojan tililläsi.

2. Valitse tietoturvakeskuksen &amp; vasemman siirtymisruudun Uhkien hallinta **-kohdassa** **Käytäntö.**

3. Valitse Käytäntö-sivulla **Turvalliset linkit.**

Oletuskäytännön muokkaaminen:

1. Valitse Turvalliset linkit **-sivun Koko organisaatiota** koskevat käytännöt -kohdassa **oletuskäytäntö.**

2. Valitse **Asetuksista, jotka koskevat sisältöä sähköpostia** lukuun ottamatta, **Microsoft 365 -sovellukset yrityksille, Office for iOS ja Android.**

3. Valitse **Tallenna**.

Voit luoda uuden käytännön, joka on kohdennettu toimialueen kaikille vastaanottajille:

1. Luo uusi käytäntö valitsemalla Turvalliset **linkit**-sivun koko organisaatiota koskevat **+** käytännöt.

2. Ota käyttöön seuraavassa taulukossa luetellut asetukset.

3. Valitse **Tallenna**.

|Asetus tai asetus|Suositeltu asetus|
|---|---|
|Nimi|Turvalliset linkit -käytäntö kaikille toimialueen vastaanottajille|
|Valitse viestien tuntemattomille mahdollisesti vahingollisille URL-osoitteille haluamasi toiminto|Valitse **Käytössä – URL-osoitteet** kirjoitetaan uudelleen ja tarkistetaan tunnettujen haittalinkkien luettelosta, kun käyttäjä napsauttaa linkkiä.|
|Ladattavan sisällön skannaaminen turvallisten liitteiden avulla|Valitse tämä ruutu.|
|Käytössä:|Vastaanottajan toimialue on . . . valitse toimialueesi.|

Lisätietoja on kohdassa [Turvalliset linkit.](../security/office-365-security/atp-safe-links.md)

## <a name="go-to-intune-admin-center"></a>Siirry Intune-hallintakeskukseen

1. Kirjaudu [Azure-portaaliin.](https://portal.azure.com/)

2. Valitse **Kaikki palvelut** ja kirjoita *Intune* **hakuruutuun.**

3. Kun tulokset ovat näkyvissä, valitse **Microsoft Intunen** vieressä alku, jotta se on suosikki ja helppo löytää myöhemmin.

Hallintakeskuksen lisäksi voit Intunen avulla rekisteröidä ja hallita organisaatiosi laitteita. Lisätietoja on kohdassa [Windows-laitteiden rekisteröintimenetelmän](/intune/enrollment/enrollment-method-capab) ja Intunen hallitsemista laitteista [ilmoittamisvaihtoehdot.](/intune/enrollment-options)