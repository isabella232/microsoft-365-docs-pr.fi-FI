---
title: Paranna Microsoft 365 for Businessin uhkien suojausta
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
description: Määritä Microsoft Defender for Office 365 ja suojaa luottamukselliset tiedot tietojen kalastelulta, haitta ohjelmilta ja muilta uhilta.
ms.openlocfilehash: 2f1a26b5a2c5678871502d441b6ba64c9b011e1c
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842252"
---
# <a name="increase-threat-protection"></a>Uhkien suojaamisen lisääminen

Tämän artikkelin avulla voit parantaa Microsoft 365-tila uksen suojausta tietojen kalastelua, haitta ohjelmia ja muita uhkia vastaan. Nämä suositukset soveltuvat organisaatioille, joilla on lisääntynyt turvallisuus, kuten asianajo toimistot ja terveyden huolto klinikat.

Ennen kuin aloitat, tarkista Office 365-suojaus Pisteet. Office 365 Secure-Pisteet analysoi organisaatiosi tieto turvaa tavallisten toimintojen ja suojaus asetusten perusteella ja määrittää Pisteet. Aloita ottamalla huomioon nykyinen Pisteet. Jos haluat lisätä piste määrän, suorita tässä artikkelissa Suositellut toiminnot. Tavoitteena ei ole saavuttaa maksimi piste määrää, vaan olla tietoinen ympäristösi suoja uksen mahdollisuuksista, jotka eivät vaikuta kielteisesti käyttäjien tuottavuuteen.

Lisä tietoja on kohdassa [Microsoftin suojattu piste](https://docs.microsoft.com/microsoft-365/security/mtp/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Sähkö postissa olevan haitta ohjelman suojaus tason nostaminen

Office 365-tai Microsoft 365-ympäristössäsi on suojaus haitta ohjelmia vastaan. Voit parantaa suojausta estämällä liite tiedostot, joiden tiedosto tyyppi on yleisesti käytetty haitta ohjelmien varalta. Voit lisätä haitta ohjelmien suojausta sähköpostitse seuraavasti:

1. Siirry [https://protection.office.com](https://protection.office.com) järjestelmänvalvojan tilin tunniste tiedoilla ja Kirjaudu sisään.

2. Valitse tieto turva &amp; -yhteensopivuus keskuksen vasemmassa siirtymis ruudussa **uhkien hallinta** -kohdassa **käytännön** \> **Anti-Malware**.

3. Kaksoisnapsauta oletus käytäntöä, jos haluat muokata tätä yrityksen laajuista käytäntöä.

4. Valitse **Asetukset**.

5. Valitse **Yleiset liitteiden tyypit-suodattimessa** **käytössä**. Suljetut tiedosto tyypit luetellaan suoraan tämän ohjaus objektin alapuolella olevassa ikkunassa. Varmista, että lisäät seuraavat tiedosto tyypit:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   Tarvittaessa voit lisätä tai poistaa tiedosto tyyppejä myöhemmin.

6. Valitse **Tallenna.**

Lisä tietoja on Ohje aiheessa [Anti-Malware Protection in EDIS:ssä](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-malware-protection).

## <a name="protect-against-ransomware"></a>Suojaa kiristys-ja

Kiristys ohjelmat rajoittavat tietojen käyttöä salaamalla tiedostoja tai lukitsemasta tieto koneen näyttöjä. Sen jälkeen se yrittää kiristää rahaa uhreilta pyytämällä "lunnaita", joka on yleensä muodossa cryptocurrencies, kuten Bitcoin, vaihdossa tietojen käyttöön.

Jos haluat suoja utua kiristys ohjelmien varalta, luo yksi tai useampi sähkö postin kulku sääntö, jonka avulla estetään yleisesti käytettävien kiristys ohjelmien tiedosto Tunnisteet. (Lisäsit nämä säännöt, kun [nostat suojausta haitta ohjelmilta Sähkö posti](#raise-the-level-of-protection-against-malware-in-mail) vaiheessa.) Voit myös varoittaa käyttäjiä, jotka saavat nämä liitteet sähköpostitse.

Edellisessä vaiheessa pysäytettävien tiedostojen lisäksi on hyvä käytäntö luoda sääntö, joka varoittaa käyttäjiä ennen makroja sisältävien Office-liite tiedostojen avaamista. Kiristys ohjelmat voidaan piilottaa makrojen sisällä, joten käyttäjät eivät voi avata näitä tiedostoja ihmisiltä, joita he eivät tiedä.

Sähkö postin siirto säännön luominen:

1. Siirry hallinta keskukseen osoitteessa <https://admin.microsoft.com> ja valitse **hallinta keskusten** \> **Exchange**.

2. Valitse **postin kulku** -luokassa **säännöt**.

3. Valitse **+** ja valitse sitten **Luo uusi sääntö**.

4. Saat näkyviin kaikki asetukset valitsemalla valinta ikkunan alareunasta **Lisää asetuksia** .

5. Käytä säännön seuraavassa taulukossa olevia asetuksia. Käytä oletus arvoja muihin asetuksiin, ellet halua muuttaa niitä.

6. Valitse **Tallenna**.

|Asetus|Varoita käyttäjiä ennen Office-tiedostojen liitteiden avaamista||
|---|---|---|
|Nimi|Anti-ranthware-sääntö: Varoita käyttäjiä|
|Käytä tätä sääntöä, jos. . .|Mikä tahansa liitteet. . . tiedosto tunniste vastaa toisiaan. . .|
|Sanojen tai lauseiden määrittäminen|Lisää seuraavat tiedosto tyypit:  <br/> DOTM, DOCM, xlsm, sltm, XLA, XLAM, XLL, pptm, potm, PPAM, ppsm, sldm|
|Toimi seuraavasti. . .|Ilmoituksen lähettäminen vastaanottajille|
|Viestin tekstin tarjoaminen|Älä avaa tämäntyyppisiä tiedostoja ihmisiltä, jotka eivät tiedä, koska ne saattavat sisältää makroja, joissa on haitallista koodia.|

Lisätietoja on seuraavissa artikkeleissa:

- [Kiristys ohjelmat: riskin pienentäminen](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [OneDriven palauttaminen](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Sähkö postin automaattisen lähettämisen lopettaminen

Käyttäjät, jotka pääsevät käsiksi käyttäjän posti laatikkoon, voivat varastaa Sähkö posti viestejä määrittämällä posti laatikon välittämään Sähkö posti viestit automaattisesti. Tämä voi tapahtua jopa ilman käyttäjän tietoisuutta. Jos haluat estää tämän, määritä sähkö postin kulku sääntö.

Jos haluat luoda sähkö postin siirto säännön, katso [Tämä lyhyt video](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) tai noudata seuraavia ohjeita:

1. Valitse Microsoft 365-hallinta keskuksessa **hallinta keskusten** \> **Exchange**.

2. Valitse **postin kulku** -luokassa **säännöt**.

3. Valitse **+** ja valitse sitten **Luo uusi sääntö**.

4. Jos haluat nähdä kaikki asetukset, valitse **Lisää asetuksia** valinta ikkunan alareunasta.

5. Ota asetukset käyttöön seuraavassa taulukossa. Käytä oletus arvoja muihin asetuksiin, ellet halua muuttaa niitä.

6. Valitse **Tallenna**.

|Asetus|Varoita käyttäjiä ennen Office-tiedostojen liitteiden avaamista|
|---|---|
|Nimi|Sähkö postin automaattisen lähettämisen estäminen ulkoisille toimi alueille|
|Käytä tätä sääntöä, jos...|Lähettäjä. . . on ulkoinen/sisäinen. . . Organisaation sisällä|
|Ehdon lisääminen|Viestin ominaisuudet. . . Sisällytä viesti tyyppi. . . Automaattinen kelaus eteenpäin|
|Toimi seuraavasti...|Estä viesti. . . hylkää viesti ja sisällytä selitys.|
|Viestin tekstin tarjoaminen|Automaattinen sähkö postin lähettäminen tämän organisaation ulkopuolelle estetään turvallisuussyistä.|


## <a name="protect-your-email-from-phishing-attacks"></a>Sähkö postin suojaaminen tietojenkalasteluhyökkäyksiltä

Jos olet määrittänyt yhden tai useamman mukautetun toimi alueen Office 365-tai Microsoft 365-ympäristöön, voit määrittää kohdennetun tietojenkalastelusuojauksen. Tietojenkalastelusuoja, joka on osa Microsoft Defender for Office 365-suojausta, voi auttaa suojaamaan organisaatiotasi haitalli silta tekeytymistä tieto kalastelu hyökkäyksiltä ja muilta tietojenkalasteluhyökkäyksiltä. Jos et ole määrittänyt mukautettua toimi aluetta, sinun ei tarvitse tehdä tätä.

Suosittelemme, että aloitat tämän suoja uksen käytön luomalla käytännössä tärkeimmät käyttäjät ja mukautetun toimi alueen suoja uksen.

Jos haluat luoda tietojenkalastelukäytännöt Microsoft Defender for Office 365-ohjelmassa, katso  [Tämä lyhyt koulutus video](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)tai Suorita seuraavat vaiheet:

1. Siirry osoitteeseen [https://protection.office.com](https://protection.office.com).

2. Valitse tieto turva- &amp; yhteensopivuus keskuksen vasemmassa siirtymis ruudussa **uhkien hallinta** -kohdassa **käytännöt**.

3. Valitse **käytännöt** **-sivulla anti-phishing**.

4. Valitse **tietojenkalastelusivulla** **+ Luo**. Ohjattu toiminto käynnistyy ja opastaa määrittämään tietojenkalastelukäytäntöä.

5. Määritä käytännölle nimi, kuvaus ja asetukset seuraavan taulukon suositusten mukaisesti. Lisä tietoja on artikkelissa [lisä tietoja tietojenkalastelukäytännöstä Microsoft Defender for Office 365-asetuksissa](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).

6. Kun olet tarkistanut asetukset, valitse **Luo tämä menettely** tai **Tallenna** tarvittaessa.

|Asetus tai asetus|Suositeltu asetus|
|---|---|
|Nimi|Toimi alue ja arvokkain kampanjan henkilö kunta|
|Kuvaus|Varmista, että tärkein henkilö kunta ja toimi alue eivät ole tekemillä.|
|Käyttäjien lisääminen suojausta varten|Valitse **+ Lisää ehto, vastaanottajaon**. Kirjoita käyttäjä nimet tai kirjoita ehdokkaan, kampanjan valvojan ja muiden tärkeiden henkilö kunnan jäsenten Sähkö posti osoitteet. Voit lisätä enintään 20 sisäistä ja ulkoista osoitetta, jotka haluat suojata tekeytymästä.|
|Toimi alueiden lisääminen suojausta varten|Valitse **+ Lisää ehto, vastaanottajatoimi alue on**. Kirjoita Microsoft 365-tila ukseen liitetty mukautettu toimi alue, jos olet määrittänyt sellaisen. Voit lisätä useamman kuin yhden toimi alueen.|
|Valitse toiminnot|Jos tekeytetty käyttäjä lähettää sähkö postia: Valitse **Ohjaa viesti toiseen Sähkö posti osoitteeseen** ja kirjoita sitten tieto turva-järjestelmänvalvojan Sähkö posti osoite. esimerkiksi *Alice <span> <span> @contoso. com*. Jos tekeytetty toimi alue lähettää sähkö postia: Valitse **karanteeni viesti**.|
|Posti laatikon tiedot|Posti laatikon tiedot valitaan oletusarvoisesti, kun luot uuden tietojenkalastelukäytäntöä. Jätä tämä asetus **päälle** parhaiden tulosten saamiseksi.|
|Luotettujen lähettäjien ja toimi alueiden lisääminen|Tässä voit lisätä oman toimi alueesi tai muita luotettuja toimi alueita.|
|Käytetään|Valitse **vastaanottajatoimi alue**. Valitse **jokin näistä** -kohdassa **Valitse**. Valitse **+ Lisää**. Valitse toimi alueen nimen vieressä oleva valinta ruutu, esimerkiksi *contoso. <span> <span> com* , luettelosta ja valitse sitten **Lisää**. Valitse **valmis**.|

## <a name="protect-against-malicious-attachments-and-files-with-safe-attachments"></a>Suojaudu haitalli silta liitteiltä ja tiedostoista, joilla on turvalliset liitteet

Ihmiset lähettävät ja jakavat säännöllisesti liitteitä, kuten asia kirjoja, esityksiä ja laskenta taulukoita. Sähkö posti viestistä ei aina käy helposti selville, onko se turvallinen vai vahingollinen. Microsoft Defender for Office 365 sisältää turvallisen liitteiden suojaamisen, mutta tätä suojausta ei oletusarvoisesti ole otettu käyttöön. On suositeltavaa luoda uusi sääntö, jonka avulla voit aloittaa tämän suojan käytön. Tämä suojaus ulottuu tiedostoihin SharePointissa, OneDrivessa ja Microsoft Teamsissa.

Jos haluat luoda turvallisen liitteiden käytännöt, katso [Tämä lyhyt video](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)tai Suorita seuraavat vaiheet:

1. Siirry [https://protection.office.com](https://protection.office.com) -kohtaan ja Kirjaudu sisään järjestelmänvalvojan tilillä.

2. Valitse tieto turva- &amp; yhteensopivuus keskuksen vasemmassa siirtymis ruudussa **uhkien hallinta** -kohdassa **käytännöt**.

3. Valitse käytännöt-sivulla **turvalliset liitteet**.

4. Ota tämä suojaus käyttöön yleisesti turvalliset liitteet-sivulla valitsemalla **Ota käyttöön ATP SharePoint-, OneDrive-ja Microsoft teams** -valinta ruutu.

5. **+** Luo uusi käytännöt valitsemalla.

6. Ota asetukset käyttöön seuraavassa taulukossa.

7. Kun olet tarkistanut asetukset, valitse **Luo tämä menettely** tai **Tallenna** tarvittaessa.

|Asetus tai asetus|Suositeltu asetus|
|---|---|
|Nimi|Estä nykyiset ja tulevat sähkö postit havaitusta haitta ohjelman avulla.|
|Kuvaus|Estä nykyiset ja tulevat sähkö postit ja liitteet havaittujen haitta ohjelmien avulla.|
|Liitteiden tallentaminen tuntematon haitta ohjelma vastaus|Valitse **Estä-estä nykyiset ja tulevat sähkö postit ja liitteet havaittujen haitta ohjelmien avulla**.|
|Uudelleenohjauksen uudelleenohjaus tunnistamisen aikana|Ota uudelleenohjaus käyttöön (Valitse tämä valinta ruutu) Anna järjestelmänvalvojan tili tai Määritä karanteenin posti laatikon asetukset.          Käytä edellä mainittua valintaa, jos liitteiden virus tarkistus aikakatkaistaan tai tapahtuu virhe (Valitse tämä valinta ruutu).|
|Käytetään|Vastaanottajatoimi alue on. . . Valitse toimi alueesi.|

Lisä tietoja on Ohje aiheessa [tietojenkalastelukäytäntöjen määrittäminen Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies)-sovelluksessa.

## <a name="protect-against-phishing-attacks-with-safe-links"></a>Suojaudu tieto kalastelu hyökkäyksiltä, joissa on turvalliset linkit

Hakkerit piilottavat toisinaan vihamielisiä sivustoja sähkö postin tai muiden tiedostojen linkeissä. Turvalliset linkit, jotka ovat osa Microsoft Defender for Office 365-palvelua, voivat auttaa suojaamaan organisaatiotasi antamalla Sähkö posti viesteissä ja Office-asia kirjoissa olevien verkko-osoitteiden (URL) tarkistus ajan kohdan. Suojaus määritetään turvallisten linkkien käytäntöjen kautta.

Suosittelemme, että teet seuraavat toimet:

- Paranna suojausta muokkaamalla oletus käytäntöä.

- Lisää uusi toiminta tapa, joka kohdistetaan kaikille toimi alueesi edunsaajille.

Voit määrittää turvallisia linkkejä katsomalla [tämän lyhyen koulutus videon](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)tai suorittamalla seuraavat vaiheet:

1. Siirry [https://protection.office.com](https://protection.office.com) -kohtaan ja Kirjaudu sisään järjestelmänvalvojan tilillä.

2. Valitse tieto turva- &amp; yhteensopivuus keskuksen vasemmassa siirtymis ruudussa **uhkien hallinta** -kohdassa **käytännöt**.

3. Valitse käytännöt-sivulla **Turvalliset linkit**.

Oletus käytäntöjen muokkaaminen:

1. Valitse Turvalliset linkit-sivun **koko organisaatiota koskevat käytännöt** -kohdassa **oletus** käytäntö.

2. Valitse **Asetukset, jotka koskevat sisältöä paitsi Sähkö posti** -kohdassa **Microsoft 365-sovellukset Enterprise-, Office for iOS-ja Android-sovelluksissa**.

3. Valitse **Tallenna**.

Uuden käytäntöjen luominen kaikille toimi alueen kaikille edunsaajille:

1. Valitse Turvalliset linkit-sivun **koko organisaatiota koskevat käytännöt** -kohdassa, **+** Jos haluat luoda uuden käytännön.

2. Käytä seuraavassa taulukossa lueteltuja asetuksia.

3. Valitse **Tallenna**.

|Asetus tai asetus|Suositeltu asetus|
|---|---|
|Nimi|Turvallisten linkkien käytännöt kaikille toimi alueen edunsaajille|
|Tuntemattomien mahdollisesti haitallisten URL-osoitteiden toiminnon valitseminen viesteissä|Valitse **URL-osoitteet kirjoitetaan uudelleen ja tarkistetaan tunnettujen haitallisten linkkien luettelosta, kun käyttäjä napsauttaa linkkiä**.|
|Ladattavien sisältöjen skannaaminen turvallisten liitteiden avulla|Valitse tämä valinta ruutu.|
|Käytetään|Vastaanottajatoimi alue on. . . Valitse toimi alueesi.|

Lisä tietoja on kohdassa [Turvalliset linkit](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links).

## <a name="go-to-intune-admin-center"></a>Siirry Intune-hallinta keskukseen

1. Kirjaudu sisään [Azure Portaliin](https://portal.azure.com/).

2. Valitse **Kaikki palvelut** ja kirjoita **haku ruutuun** *Intune* .

3. Kun tulokset tulevat näkyviin, valitse Aloita **Microsoft Intune** -kohdan vierestä, jotta se on suosikki ja helppo löytää myöhemmin.

Hallinta keskuksen lisäksi voit käyttää Intunea organisaation laitteiden rekisteröimiseen ja hallintaan. Lisä tietoja on kohdassa [ominaisuudet Windows-laitteiden rekisteröinti menetelmällä](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) ja [Intune-laitteiden rekisteröinti vaihtoehdot](https://docs.microsoft.com/intune/enrollment-options).
