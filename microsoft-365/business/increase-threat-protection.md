---
title: Uhkien uhkien Microsoft 365 for Businessissa
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
description: Määritä Microsoft Defender for Office 365 ja suojaa arkaluontoiset tiedot tietojen kalastelulta, haittaohjelmilta ja muilta uhilta.
ms.openlocfilehash: 4b5142efbf4392f017cd9b96f6a9c36ef2000bb7
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245140"
---
# <a name="increase-threat-protection"></a>Uhkien uhkien uhkien uhki

Tämän artikkelin avulla voit parantaa tilauksesi suojausta tietojen kalastelulta, haittaohjelmilta ja muilta uhilta Microsoft 365 suojaamiseksi. Nämä suositukset sopivat organisaatioille, joilla on entistä enemmän tietoturvan tarvetta, kuten lakitoimistot ja terveysalan työt.

Ennen kuin aloitat, tarkista Office 365 Secure Score. Office 365 Secure Score analysoi organisaatiosi suojauksen säännöllisten toimintojen ja suojausasetusten perusteella ja antaa pistemäärän. Aloita merkitsemällä nykyinen pistemäärä muistiin. Jos haluat kasvattaa pistemäärää, suorita tässä artikkelissa suositellut toimet. Tavoitteena ei ole saavuttaa enimmäispisteystä, vaan mahdollisuus suojata ympäristöäsi, sillä se ei vaikuta merkittävästi käyttäjien tuottavuuteen.

Lisätietoja on kohdassa [Microsoft Secure Score.](../security/defender/microsoft-secure-score.md)

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Nosta sähköpostin haittaohjelmasuojaustasoa

Oma Office 365 tai Microsoft 365 ympäristösi sisältää suojauksen haittaohjelmia vastaan. Voit parantaa tätä suojausta estämällä liitetiedostot tiedostotyypeillä, joita käytetään yleisesti haittaohjelmien kanssa. Voit parantaa haittaohjelmien suojausta sähköpostissa:

1. Siirry [https://protection.office.com](https://protection.office.com) järjestelmänvalvojan tilin tunnistetiedoilla ja kirjaudu sisään.

2. Valitse Tietoturvakeskuksen vasemman siirtymisruudun Uhkien &amp; hallinta -kohdassa **Policy**  \> **Anti-Malware (Käytännön haittaohjelmien torjunta).**

3. Voit muokata koko yrityksen kattavaa käytäntöä kaksoisnapsauttamalla oletuskäytäntöä.

4. Valitse **Asetukset**.

5. Valitse **Yleisimmät liitetyypit -suodatin**-kohdassa **Käytössä**. Estetyt tiedostotyypit näkyvät tämän ohjausobjektin alapuolella olevassa ikkunassa. Varmista, että lisäät seuraavat tiedostotyypit:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   Tarvittaessa voit lisätä tai poistaa tiedostotyyppejä myöhemmin.

6. Valitse **Tallenna.**

Lisätietoja on kohdassa [Haittaohjelmien torjunta EOP:ssä.](../security/office-365-security/anti-malware-protection.md)

## <a name="protect-against-ransomware"></a>Kiristysohjelmilta suojautuminen

Kiristysohjelmat rajoittavat tietojen käyttöä salaamalla tiedostoja tai lukitsemalla tietokoneen näyttöjä. Tämän jälkeen se yrittää kiristysta kiristysta pyytämällä kiristysta, joka on yleensä salattuina, kuten Bitcoinina, tietojen käyttöön vastineeksi.

Voit suojautua kiristysohjelmilta luomalla yhden tai useamman postinkulkusäännön, joka estää kiristysohjelmissa yleisesti käytetyt tiedostotunnisteet. (Olet lisännyt nämä säännöt [nostamaan suojaustasoa haittaohjelmilta sähköposti vaiheessa.)](#raise-the-level-of-protection-against-malware-in-mail) Voit myös varoittaa käyttäjiä, jotka saavat nämä liitteet sähköpostitse.

Edellisessä vaiheessa estettyjen tiedostojen lisäksi on hyvä luoda sääntö, joka varoittaa käyttäjiä ennen makroja Office-liitetiedostojen avaamista. Kiristysohjelmat voidaan piilottaa makrojen sisään, joten varoita käyttäjiä avaamaan näitä tiedostoja henkilöltä, jonka eivät tunne.

Sähköpostin siirtosäännön luominen:

1. Siirry hallintakeskukseen -kohdassa ja <https://admin.microsoft.com> valitse **hallintakeskukset** \> **Exchange**.

2. Valitse **Postinkulku-luokasta** **säännöt**.

3. Valitse **+** ja valitse sitten Luo uusi **sääntö**.

4. Valitse **valintaikkunan** alareunassa Lisää asetuksia, niin näet kaikki asetukset.

5. Ota säännön asetukset käyttöön seuraavassa taulukossa. Käytä oletusarvoja muille asetuksille, ellet halua muuttaa niitä.

6. Valitse **Tallenna**.

|Asetus|Varoita käyttäjiä ennen Office liitteiden avaamista||
|---|---|---|
|Nimi|Kiristysohjelmien estosääntö: varoita käyttäjiä|
|Käytä tätä sääntöä, jos . . .|Mikä tahansa liite . . . tiedostotunniste vastaa tunnistetta . . .|
|Sanojen tai lauseiden määritteleminen|Lisää seuraavat tiedostotyypit:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm|
|Tee seuraavat toimet. . .|Vastaanottajalle ilmoittaminen viestillä|
|Viestin tekstin lisääminen|Älä avaa tällaisia tiedostoja henkilöltä, jonka et tiedä, koska ne saattavat sisältää haittaohjelmia sisältäviä makroja.|

Lisätietoja on seuraavissa artikkeleissa:

- [Kiristysohjelmat: riskien pienentäminen](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [Palauta OneDrive](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Sähköpostin automaattisen edelleenlähetysten pysäyttäminen

Hakkerit, jotka saavat käyttöoikeudet käyttäjän postilaatikkoon, voivat varastaa sähköpostia määrittämällä postilaatikon välittämään sähköpostit automaattisesti. Näin voi käydä myös ilman käyttäjän tuntemusta. Voit estää tämän määrittämällä postinkulkusäännön.

Jos haluat luoda sähköpostin siirtosäännön, katso [tämä lyhyt video tai](../business-video/stop-email-auto-forward.md) toimi seuraavasti:

1. Valitse Microsoft 365 hallintakeskuksessa **Hallintakeskukset Exchange.** \> 

2. Valitse **Postinkulku-luokasta** **säännöt**.

3. Valitse **+** ja valitse sitten Luo uusi **sääntö**.

4. Jos haluat nähdä kaikki vaihtoehdot, **valitse** valintaikkunan alareunassa Lisää asetuksia.

5. Ota asetukset käyttöön seuraavassa taulukossa. Käytä oletusarvoja muille asetuksille, ellet halua muuttaa niitä.

6. Valitse **Tallenna**.

|Asetus|Varoita käyttäjiä ennen Office liitteiden avaamista|
|---|---|
|Nimi|Sähköpostin automaattisen edelleenlähetysten estäminen ulkoisiin toimialueisiin|
|Käytä tätä sääntöä, jos ...|Lähettäjä . . . on ulkoinen/sisäinen. . . Organisaation sisällä|
|Lisää ehto|Viestin ominaisuudet . . . sisällytä viestityyppi . . . Automaattinen edelleenlähetys|
|Tee seuraavat toimet...|Estä viesti . . . hylkää viestin ja lisää selitys.|
|Viestin tekstin lisääminen|Tämän organisaation ulkopuolinen sähköpostin automaattinen edelleenlähetys estetään tietoturvasyistä.|


## <a name="protect-your-email-from-phishing-attacks"></a>Sähköpostin suojaaminen tietojenkalasteluhyökkäyksiltä

Jos olet määrittänyt yhden tai useamman mukautetun toimialueen Office 365 tai Microsoft 365, voit määrittää kohdennetun tietojenkalastelun torjuntasuojauksen. Microsoft Defender for Office 365 :tä koskeva tietojenkalastelun torjunta voi auttaa suojaamaan organisaatiotasi haitallisilta tekeytymisperusteisilta tietojen kalasteluhyökkäyksiltä ja muilta tietojen kalasteluhyökkäyksiltä. Jos et ole määrittänyt mukautettua toimialuetta, sinun ei tarvitse tehdä tätä.

Suosittelemme, että aloitat tämän suojauksen käytön luomalla käytännön tärkeimpien käyttäjien ja mukautetun toimialueen suojaamiseksi.

Jos haluat luoda tietojenkalastelun torjuntakäytännön Microsoft Defender for Office 365, katso tämä lyhyt [koulutusvideo](../business-video/setup-anti-phishing.md)tai toimi seuraavasti:

1. Siirry osoitteeseen [https://protection.office.com](https://protection.office.com).

2. Valitse Tietoturvakeskuksen &amp; vasemman siirtymisruudun Uhkien hallinta -kohdassa **Käytäntö**. 

3. Valitse **Käytäntö-sivulla** **Tietojen kalastelun torjunta**.

4. Valitse **Tietojen kalastelun** esto **-sivulla + Luo**. Ohjattu toiminto käynnistyy, ja sen avulla voit määrittää tietojenkalastelun torjuntakäytännön.

5. Määritä käytännön nimi, kuvaus ja asetukset seuraavassa taulukossa suositellulla mukaisesti. Lisätietoja on kohdassa Tietoja Microsoft [Defenderin tietojenkalastelun vastaisten tietojen kalastelun torjunnan Office 365 asetuksista.](../security/office-365-security/set-up-anti-phishing-policies.md)

6. Kun olet tarkistanut asetukset, valitse **Luo tämä käytäntö tai** **Tallenna**.

|Asetus tai asetus|Suositeltu asetus|
|---|---|
|Nimi|Toimialue ja arvokkain kampanjahenkilökunta|
|Kuvaus|Varmista, että tärkeintä henkilökuntaa ja toimialuetta ei tekeytetä.|
|Käyttäjien lisääminen suojattavaksi|Valitse **+ Lisää ehto, Vastaanottaja on**. Kirjoita käyttäjänimet tai kirjoita ehdokkaan, kampanjapäällikön ja muiden tärkeiden henkilökunnan jäsenten sähköpostiosoitteet. Voit lisätä enintään 20 sisäistä ja ulkoista osoitetta, jotka haluat suojata tekeytymishenkilöltä.|
|Toimialueiden lisääminen suojattavaksi|Valitse **+ Lisää ehto, Vastaanottajan toimialue on**. Anna mukautettu toimialue, joka on liitetty Microsoft 365, jos määritit sellaisen. Voit kirjoittaa useamman kuin yhden toimialueen.|
|Toimintojen valinta|Jos sähköpostin lähettänyt tekeytynyt käyttäjä: Valitse **Ohjaa** viesti toiseen sähköpostiosoitteeseen ja kirjoita sitten suojauksenvalvojan sähköpostiosoite. esimerkiksi *Toni <span> <span> @contoso.com.* Jos sähköpostin lähettää tekeytynyt toimialue: Valitse **Karanteeniviesti**.|
|Postilaatikkotiedot|Postilaatikkotiedot valitaan oletusarvoisesti, kun luot uuden tietojenkalastelun torjuntakäytännön. Jätä tämä asetus **käytössä,** niin saat parhaan tuloksen.|
|Luotettujen lähettäjien ja toimialueiden lisääminen|Tässä voit lisätä oman toimialueesi tai minkä tahansa muun luotetun toimialueen.|
|Käytössä kohteeseen|Valitse **Vastaanottajan toimialue on**. Valitse **Mikä tahansa näistä** **-kohdassa Valitse**. Valitse **+ Lisää**. Valitse toimialueen nimen vieressä oleva valintaruutu, esimerkiksi *contoso. <span> <span> com* ja valitse sitten **Lisää**. Valitse **Valmis**.|

## <a name="protect-against-malicious-attachments-and-files-with-safe-attachments"></a>Turvallisten liitteiden suojaaminen haitallisilta liitteiltä ja tiedostoilta

Henkilöt lähettävät, vastaanottavat ja jakavat säännöllisesti liitteitä, kuten asiakirjoja, esityksiä, laskentataulukoita ja paljon muuta. Sähköpostiviestin avulla ei ole aina helppo tietää, onko liite turvallinen vai haitallinen. Microsoft Defender for Office 365 sisältää turvallisten liitteiden suojauksen, mutta tämä suojaus ei ole oletusarvoisesti käytössä. Suosittelemme, että luot uuden säännön suojauksen käytön aloittamista varten. Tämä suojaus kattaa myös SharePoint, OneDrive ja Microsoft Teams.

Voit luoda turvallisten liitteiden käytännön joko katsomalla [tämän lyhyen videon tai](../business-video/safe-attachments.md)toimimalla seuraavasti:

1. Siirry [https://protection.office.com](https://protection.office.com) -tunnukseen ja kirjaudu sisään järjestelmänvalvojan tililläsi.

2. Valitse Tietoturvakeskuksen &amp; vasemman siirtymisruudun Uhkien hallinta -kohdassa **Käytäntö**. 

3. Valitse Käytäntö-sivulla **Turvalliset liitteet**.

4. Käytä tätä suojausta laajalti Turvalliset liitteet -sivulla valitsemalla Ota **ATP käyttöön SharePoint-, OneDrive-** Microsoft Teams-valintaruutu.

5. Luo **+** uusi käytäntö valitsemalla .

6. Ota asetukset käyttöön seuraavassa taulukossa.

7. Kun olet tarkistanut asetukset, valitse **Luo tämä käytäntö** tai **Tallenna**.

|Asetus tai asetus|Suositeltu asetus|
|---|---|
|Nimi|Estä nykyiset ja tulevat sähköpostiviestit tunnistetuilla haittaohjelmilla.|
|Kuvaus|Estä nykyiset ja tulevat sähköpostiviestit ja liitteet havaittujen haittaohjelmien avulla.|
|Liitteiden tallentaminen tuntemattomasta haittaohjelmavastauksen sovelluksesta|Valitse **Estä – estä nykyiset ja tulevat sähköpostiviestit ja liitteet, joissa on havaittu haittaohjelma.**|
|Liitteen uudelleenohjaus tunnistukseen|Ota uudelleenohjaus käyttöön (valitse tämä ruutu) Kirjoita järjestelmänvalvojan tili tai postilaatikon määritys karanteeniin.          Käytä yllä olevaa valintaa, jos liitteiden tarkistus käy läpi haittaohjelmia tai tapahtuu virhe (valitse tämä ruutu).|
|Käytössä kohteeseen|Vastaanottajan toimialue on . . . valitse toimialueesi.|

Lisätietoja on kohdassa [Tietojenkalastelun torjuntakäytäntöjen määritys Microsoft Defender for Office 365.](../security/office-365-security/set-up-anti-phishing-policies.md)

## <a name="protect-against-phishing-attacks-with-safe-links"></a>Tietojenkalasteluhyökkäyksiltä suojautuminen turvallisten linkkien avulla

Hakkerit piilovat joskus vahingollisia sivustoja sähköpostissa tai muissa tiedostoissa olevista linkeistä. Turvalliset linkit, joka on osa Microsoft Defender for Office 365 -selainta, voivat auttaa suojaamaan organisaatiotasi antamalla sähköpostiviesteissä ja tiedostoissa olevien verkko-osoitteiden (URL-osoitteiden) napsautuksen Office tarkistamisen. Suojaus määritetään turvallisten linkkien käytännöistä.

Suosittelemme, että toimit seuraavasti:

- Voit parantaa suojausta muokkaamalla oletuskäytäntöä.

- Lisää uusi käytäntö, joka on kohdennettu toimialueesi kaikille vastaanottajille.

Voit määrittää turvalliset linkit katsomalla [tämän lyhyen koulutusvideon](../business-video/safe-links.md)tai noudattamalla seuraavia ohjeita:

1. Siirry [https://protection.office.com](https://protection.office.com) -tunnukseen ja kirjaudu sisään järjestelmänvalvojan tililläsi.

2. Valitse Tietoturvakeskuksen &amp; vasemman siirtymisruudun Uhkien hallinta -kohdassa **Käytäntö**. 

3. Valitse Käytäntö-sivulla **Turvalliset linkit**.

Oletuskäytännön muokkaaminen:

1. Valitse Turvalliset linkit -sivun **Koko organisaatiota koskevat** käytännöt -kohdassa **Oletuskäytäntö.**

2. Valitse **Asetukset, joka koskee** muuta sisältöä kuin sähköpostia , **-kohdassa Microsoft 365 -sovellukset suuryrityksille, Office iOS- ja Android-laitteille**.

3. Valitse **Tallenna**.

Voit luoda uuden käytännön, joka on kohdennettu toimialueesi kaikille vastaanottajille:

1. Luo uusi käytäntö valitsemalla Turvalliset **linkit**-sivun Koko organisaatiota koskevat **+** käytännöt -kohdassa .

2. Ota käyttöön seuraavassa taulukossa luetellut asetukset.

3. Valitse **Tallenna**.

|Asetus tai asetus|Suositeltu asetus|
|---|---|
|Nimi|Turvalliset linkit -käytäntö kaikille toimialueen vastaanottajille|
|Valitse viestien tuntemattomien mahdollisesti vahingollisen URL-osoitteiden toiminto|Valitse **Käytössä – URL-osoitteet kirjoitetaan** uudelleen ja tarkistetaan tunnettujen haitallisten linkkien luetteloon, kun käyttäjä napsauttaa linkkiä .|
|Ladattavien sisältöjen skannaaminen turvallisten liitteiden avulla|Valitse tämä ruutu.|
|Käytössä kohteeseen|Vastaanottajan toimialue on . . . valitse toimialueesi.|

Lisätietoja on kohdassa [Turvalliset linkit.](../security/office-365-security/safe-links.md)

## <a name="go-to-intune-admin-center"></a>Siirry Intune-hallintakeskukseen

1. Kirjaudu [Azure-portaaliin.](https://portal.azure.com/)

2. Valitse **Kaikki palvelut** ja kirjoita *Intune* **hakuruutuun**.

3. Kun tulokset ovat näkyvissä, valitse aloitus **Microsoft Intune,** jotta se on suosikki ja helppo löytää myöhemmin.

Hallintakeskuksen lisäksi voit Intunen avulla rekisteröidä ja hallita organisaatiosi laitteita. Lisätietoja on vaihtoehdoissa [Intunella hallittujen laitteiden Windows](/intune/enrollment/enrollment-method-capab) rekisteröintimenetelmän ominaisuudet ja [rekisteröintiasetukset.](/intune/enrollment-options)
