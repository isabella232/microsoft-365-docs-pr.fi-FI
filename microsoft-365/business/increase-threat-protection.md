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
ms.custom:
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Määritä Office 365 Advanced uhkien torjunta ja suojaa arkaluontoisia tietoja.
ms.openlocfilehash: 87a5c79636a2eefe394b4a30e72971eb851e3ecb
ms.sourcegitcommit: 38934a2115d5cdeb44c7484d57be07686c6f7720
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704071"
---
# <a name="increase-threat-protection"></a>Lisää uhkien torjunta

Tämän artikkelin avulla voit suojata Microsoft 365-tilauksesi suojausta tietojenkalastelulta, haitta ohjelmilta ja muista uhkilta suojautumiselta. Nämä suositukset soveltuvat organisaatioille, joilla on lisääntynyt turvallisuuden tarve, kuten laki toimistot ja terveyden huollon klinikat.

Varmista ennen aloittamista, että Office 365 on suojattu pisteytys. Office 365 Secure Score analysoi Office 365-organisaatiosi tieto turvan tavallisiin aktiviteetteihin ja suojaus asetuksiin Perustuen ja määrittää Pisteet. Aloita ottamalla huomioon nykyinen piste määrä. Voit kasvattaa pisteesi tekemällä tässä artikkelissa suositellut toimet. Tavoitteena ei ole saavuttaa maksimi pisteitä, vaan olla tietoinen mahdollisuuksista suojata ympäristöäsi, jotka eivät vaikuta kielteisesti käyttäjien tuottavuuteen. 

Lisä tietoja on [Microsoft Securen pisteytys](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score)-kohdassa.

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Nosta suojaus tasoa haitta ohjelmilta Mailissa

Office 365-tai Microsoft 365-ympäristö sisältää suoja uksen haitta ohjelmilta. Voit lisätä suojausta estämällä liite tiedostoja tiedosto tyypeillä, joita käytetään yleisesti haitta ohjelmien yhteydessä. Voit lisätä haitta ohjelmien suojausta sähköpostitse:
  
1. Siirry [https://protection.office.com](https://protection.office.com) ja Kirjaudu sisään järjestelmänvalvojan tilin tunniste tiedoilla. 
    
2. Valitse Office 365-tieto &amp; turvan yhteensopivuus keskuksessa vasemmanpuoleisessa siirtymis ruudussa **uhkien hallinta**-kohdasta **käytännön** \> **haitta ohjelmien torjunta**.
    
3. Kaksoisnapsauta oletus käytäntöä, jos haluat muokata koko yrityksen käytäntöä.
    
4. Valitse **Asetukset**.
    
5. Valitse **yhteiset liite tyypit-suodattimessa** **käytössä**. Estetyt tiedosto tyypit näkyvät ikkunassa suoraan tämän ohjaus objektin alapuolella. Varmista, että lisäät nämä tiedosto tyypit:
   - ADE, ADP, Ani, BAS, bat, chm, cmd, com, cpl, CRT, hlp, HT, HTA, inf, ins, ISP, Job, js, JSE, LNK, MDA, MDB, MDE, MDZ, MSC, MSI, msp, MST, PCD, reg, SCR, SCT, SHS, URL, VB, VBE, VBS, WSC, WSF, WSH, exe, PIF  <br/> 
   
   Tarvittaessa voit lisätä tai poistaa tiedosto tyyppejä myöhemmin.
    
6. Valitse **Tallenna.**
    
Lisä tietoja on artikkelissa [haitta ohjelmien torjunta](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Suojaa kiristys ohjelmilta

Ransomware rajoittaa pääsyä tietoihin salaamalla tiedostoja tai lukitsemalla tieto koneen näytöt. Sitten se yrittää kiristystä rahaa uhreilta pyytämällä "lunnaita", yleensä kryptovaluuttojen muodossa, kuten Bitcoin, vastineeksi pääsystä tietoihin. 
  
Suojautu maan kiristys ohjelmilta, luo yksi tai useampi sähkö postin virta sääntöjä estää tiedosto laajennuksia, joita käytetään yleisesti ransomware. (Lisäsit nämä säännöt [nostamalla suojaus tasoa haitta ohjelmilta Mail](#raise-the-level-of-protection-against-malware-in-mail) -vaiheessa.) Voit myös varoittaa käyttäjiä, jotka vastaanottavat nämä liitteet sähköpostitse.

Edellisessä vaiheessa estettyjen tiedostojen lisäksi on hyvä käytäntö luoda sääntö, joka varoittaa käyttäjiä, ennen kuin avaat makroja sisältävät Office-liite tiedostot. Ransomware voidaan piilottaa sisällä makroja, joten varoittaa käyttäjiä ei avata näitä tiedostoja ihmiseltä he eivät tiedä.

Sähkö postin siirto säännön luominen:
  
1. Siirry hallinta keskukseen <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>ja valitse **hallinta keskusten** \> **vaihto**.
    
2. Valitse **Mail Flow** -luokassa **säännöt**.
    
3. Valitse **+** ja valitse sitten **Luo uusi sääntö**.
    
4. Valitsemalla **Lisää vaihto ehtoja** valinta ikkunan alareunasta näet kaikki vaihto ehdot. 
    
5. Käytä säännön seuraavassa taulukossa asetuksia. Käytä muiden asetusten oletus arvoja, ellet halua muuttaa niitä.
    
6. Valitse **Tallenna**.
    
|**Asetus**|**Varoita käyttäjiä ennen Office-tiedostojen liitteiden avaamista**||
|:-----|:-----|:-----|
|Nimi  <br/> |Anti-ransomware sääntö: varoittaa käyttäjiä  <br/>  |
|Käytä tätä sääntöä, jos. . .  <br/> |Mitään liitettä. . . tiedosto pääte vastaa. . .  <br/> |
|Sanojen tai lauseiden määrittäminen  <br/> |Lisää nämä tiedosto tyypit:  <br/> DOTM, DOCM, xlsm, sltm, XLA, XLAM, XLL, pptm, potm, PPAM, ppsm, sldm  <br/>|
|Toimi seuraavasti. . .  <br/> |Ilmoita vastaanottajalle viestillä  <br/> |
|Sanoman tekstin tarjoaminen  <br/> |Älä avaa tällaisia tiedostoja ihmisistä et tiedä, koska ne saattavat sisältää makroja, joilla on haitallinen koodi.  <br/> |
   
Lisätietoja on seuraavissa artikkeleissa:
  
- [Miten käsitellä ransomware](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [Palauta OneDrive-](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Pysäytä sähkö postin automaattinen edelleenlähetys

Hakkerit, jotka pääsevät käsiksi käyttäjän posti laatikkoon, voivat varastaa postia asettamalla posti laatikon automaattisesti välittämään sähkö postia. Tämä voi tapahtua myös ilman käyttäjän tietoisuutta. Jos haluat estää tämän tapahtumasta, määritä Sähkö posti työn kulku sääntö. 
  
Voit luoda sähkö postin siirto säännön joko katsomalla [tämän lyhyen videon](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) tai toimimalla seuraavasti:
  
1. Valitse Microsoft 365-hallinta keskuksessa **hallinta keskusten** \> **vaihto**.
    
2. Valitse **Mail Flow** -luokassa **säännöt**.
    
3. Valitse **+** ja valitse sitten **Luo uusi sääntö**.
    
4. Jos haluat nähdä kaikki vaihto ehdot, valitse **Lisää vaihto ehtoja** valinta ikkunan alareunasta. 
    
5. Käytä seuraavan taulukon asetuksia. Käytä muiden asetusten oletus arvoja, ellet halua muuttaa niitä.
    
6. Valitse **Tallenna**.
    
|**Asetus**|**Varoita käyttäjiä ennen Office-tiedostojen liitteiden avaamista**|
|:-----|:-----|
|Nimi  <br/> |Estä sähkö postin automaattinen edelleenlähetys ulkoisiin verkko tunnuksiin  <br/> |
|Käytä tätä sääntöä, jos...  <br/> |Lähettäjälle. . . on ulkoinen/sisäinen. . . Organisaation sisällä  <br/> |
|Lisää ehto  <br/> |Sanoman ominaisuudet. . . Sisällytä viesti tyyppi. . . Automaattinen eteenpäin  <br/> |
|Tee seuraavat toimet...  <br/> |Estä viesti. . . hylkää viesti ja sisällytä selitys.  <br/> |
|Sanoman tekstin tarjoaminen  <br/> |Sähkö postin automaattinen edelleenlähetys tämän organisaation ulkopuolella estetään turvallisuussyistä.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Suojaa sähkö postisi tietojenkalasteluhyökkäyksiltä

Jos olet määrittänyt yhden tai useita mukautettuja toimi alueita Office 365-tai Microsoft 365-ympäristöön, voit määrittää kohdennetun tietojenkalastelun esto suojauksen. ATP-tietojenkalastelusuojaus, osa Office 365 Advanced Threat Protectionista, voi auttaa suojaamaan organisaatiotasi haitalli silta tekeytymis hyökkäyksiltä ja muista tietojenkalasteluhyökkäyksistä. Jos et ole määrittänyt mukautettua toimi aluetta, tätä ei tarvitse tehdä.
  
Suosittelemme, että aloitat tämän suoja uksen luomalla käytännön, joka suojaa tärkeimpiä käyttäjiä ja mukautettua toimi aluetta. 

Jos haluat luoda ATP-kalastelun torjunta käytännön, katso [Lyhyt harjoitus video](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)tai tee seuraavat toimet:
  
1. Siirry osoitteeseen [https://protection.office.com](https://protection.office.com). 
    
2. Valitse Office 365 Security &amp; Compliance Centerissä vasemmanpuoleisessa siirtymis ruudussa **uhkien hallinta**-kohdassa **käytäntö**.
    
3. Valitse **käytäntö** -sivulla **ATP anti-phishing**.
    
4. Valitse **anti-phishing-** sivulla **+ Luo**. Ohjattu toiminto käynnistyy, joka opastaa sinua tieto kalastelun torjunta käytännön määrittämisessä.
    
5. Määritä käytännön nimi, kuvaus ja asetukset seuraavan taulukon suositusten mukaan. Lisä tietoja on kohdassa lisä tietoja [ATP-tietojenkalastelun esto käytännöstä](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options). 
    
6. Kun olet tarkistanut asetuksesi, valitse **Luo tämä käytäntö** tai **Tallenna**tarvittaessa.
    

|**Asetus tai optio**<br/>|**Suositeltu asetus** <br/>|
|:-----|:-----|
|Nimi  <br/> |Verkko tunnus ja arvokkain kampanjan henkilö kunta  <br/> |
|Kuvaus  <br/> |Varmista, että tärkein henkilö kunta ja verkko tunnuksesi eivät ole tekeytymistä.  <br/> |
|Käyttäjien lisääminen suojatakseen  <br/> |Valitse **+ Lisää ehto, vastaanottaja on**. Kirjoita käyttäjä tunnukset tai kirjoita hakijan, Campaign Managerin ja muiden tärkeiden henkilö kunnan jäsenten Sähkö posti osoite. Voit lisätä enintään 20 sisäistä ja ulkoista osoitetta, jotka haluat suojata tekeytymistä.  <br/> |
|Toimi alueiden lisääminen suojatakseen  <br/> |Valitse **+ Lisää ehto, vastaanottajan toimi alue on**. Kirjoita Microsoft 365-tila ukseen liitetty mukautettu toimi alue, jos olet määrittänyt sen. Voit kirjoittaa useamman kuin yhden toimi alueen.  <br/> |
|Valitse toiminnot  <br/> |Jos sähkö postia lähettää tekeytyvät käyttäjät: Valitse **Ohjaa viesti toiseen Sähkö posti osoitteeseen**ja kirjoita sitten suojausvalvojan Sähkö posti osoite. esimerkiksi *Alice<span><span>@contoso. com*. Jos sähkö postia lähetetään tekeytyvät toimi alue: Valitse **karanteeni viesti**.  <br/> |
|Posti laatikon älykkyys  <br/> |Posti laatikon älykkyys on oletusarvoisesti valittuna, kun luot uuden tietojenkalastelun esto käytännön. Jätä tämä asetus **päälle** parhaan tuloksen.  <br/> |
|Luotettujen lähettäjien ja toimi alueiden lisääminen  <br/> |Tässä voit lisätä oman toimi alueesi tai muita luotettuja verkko tunnuksia.  <br/> |
|Soveltaa  <br/> |Valitse **vastaanottajan toimi alue**. Valitse **jokin näistä**-kohdasta **Valitse**. Valitse **+ Lisää**. Valitse toimi alueen nimen vieressä oleva valinta ruutu, esimerkiksi *contoso.<span> com <span>*-luettelosta ja valitse sitten **Lisää**. Valitse **valmis**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Suojaa haitalli silta liitteiltä ja tiedostoja ATP turvallisia liitteitä

Ihmiset lähettävät, vastaanottavat ja jakavat säännöllisesti liitteitä, kuten asia kirjoja, esityksiä ja laskenta taulukoita. Ei ole aina helppoa kertoa, onko liite tiedosto turvallinen vai haitallinen vain katsomalla Sähkö posti viestiä. Office 365 Advanced uhkien torjunta sisältää ATP-turva kiinnityksen suoja uksen, mutta tämä suojaus ei ole oletusarvoisesti käytössä. Tämän suoja uksen käyttämisen aloittavan uuden säännön luominen on suositeltavaa. Tämä suojaus ulottuu SharePoint-, OneDrive-ja Microsoft teams-tiedostoihin.
  
Voit luoda ATP-turva kiinnitys käytännön joko katsomalla [tämän lyhyen videon](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)tai tekemällä seuraavat toimet:
  
1. [https://protection.office.com](https://protection.office.com)Siirry ja Kirjaudu sisään järjestelmänvalvojan tilillä. 
    
2. Valitse Office 365 Security &amp; Compliance Centerissä vasemmanpuoleisessa siirtymis ruudussa **uhkien hallinta**-kohdassa **käytäntö**.
    
3. Valitse käytäntö-sivulla **ATP turvalliset liitteet**.
    
4. Käytä turvalliset liitteet-sivulla tätä suojausta laajasti valitsemalla **Ota ATP käyttöön SharePointissa, OneDrivessa ja Microsoft Teamsissa** -valinta ruutu. 
    
5. Valitse **+** tämä, jos haluat luoda uuden käytännön. 
    
6. Käytä seuraavan taulukon asetuksia. 
    
7. Kun olet tarkistanut asetuksesi, valitse **Luo tämä käytäntö** tai **Tallenna**tarvittaessa.
    

|**Asetus tai optio**|**Suositeltu asetus** <br/>|
|:-----|:-----|
|Nimi  <br/> |Estä nykyiset ja tulevat sähkö postit havaittujen haitta ohjelmien kanssa.  <br/> |
|Kuvaus  <br/> |Estä nykyiset ja tulevat sähkö postit ja liitteet havaittujen haitta ohjelmien avulla.  <br/> |
|Tallenna liitteet tuntematon haitta ohjelma vastaus  <br/> |Valitse **Block-estä nykyiset ja tulevat sähkö postit ja liitteet havaittujen haitta ohjelmien kanssa**.  <br/> |
|Uudelleenohjauksen liitteen tunnistus  <br/> |Ota uudelleenohjaus käyttöön (Valitse tämä ruutu) Anna järjestelmänvalvojan tili tai posti laatikon asetukset karanteeniin.          Käytä yllä olevaa valintaa, jos haitta ohjelmat skannataan liitteille kertaa tai virhe tapahtuu (Valitse tämä ruutu).  <br/> |
|Soveltaa  <br/> |Vastaanottajan toimi alue on. . . Valitse verkko tunnuksesi.  <br/> |
   
Lisä tietoja on kohdassa [Aseta Office 365 ATP-tietojenkalastelukäytännöt](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Suojaus tietojenkalasteluhyökkäyksiltä ATP Safe Links-linkeissä

Hakkerit joskus piilottaa haitallisia sivustoja linkkejä sähkö postin tai muiden tiedostojen. Office 365 ATP turvalliset linkit (ATP Safe Links), osa Office 365 Advanced uhkien torjunta, voi auttaa suojaamaan organisaatiotasi tarjoamalla aika-of-click todentaminen Web-osoitteet (URL) sähkö posti viesteissä ja Office-asia kirjoissa. Suojaus määritetään ATP Safe Links-käytäntöjen avulla.
  
Suosittelemme, että teet seuraavat toimet:
  
- Muokkaa oletus käytäntöä suoja uksen lisäämiseksi.
    
- Lisää uusi käytäntö, joka kohdistetaan kaikille toimi alueesi vastaanottajille.
    
Jos haluat määrittää ATP-turvalliset linkit, katso [Lyhyt harjoitus video](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)tai tee seuraavat toimet:
  
1. [https://protection.office.com](https://protection.office.com)Siirry ja Kirjaudu sisään järjestelmänvalvojan tilillä. 
    
2. Valitse Office 365 Security &amp; Compliance Centerissä vasemmanpuoleisessa siirtymis ruudussa **uhkien hallinta**-kohdassa **käytäntö**.
    
3. Valitse käytäntö-sivulla **ATP Safe Links**.
    
Oletus käytännön muokkaaminen:
  
1. Valitse **oletus** käytäntö turvalliset linkit-sivun **käytännöt, jotka koskevat koko organisaatiota**. 
    
2. Valitse **Asetukset, jotka koskevat sisältöä, paitsi sähkö postia**, **Office 365 ProPlus, Office iOS:lle ja Androidille**.
    
3. Valitse **Tallenna**. 
    
Voit luoda uuden käytännön kohdistettua kaikille toimi alueesi vastaanottajille:
  
1. Luo uusi käytäntö valitsemalla **+** turvalliset linkit-sivun käytännöt, **jotka koskevat koko organisaatiota**. 
    
2. Käytä seuraavassa taulukossa lueteltuja asetuksia.
    
3. Valitse **Tallenna**. 

|**Asetus tai optio**|**Suositeltu asetus** <br/>|
|:-----|:-----|
|Nimi  <br/> |Kaikkien toimi alueen vastaanottajien turvalliset linkit-käytäntö  <br/> |
|Valitse tuntemattomien mahdollisten haitallisten URL-osoitteiden toiminto viesteissä  <br/> |Valitse **URL-osoitteet kirjoitetaan uudelleen ja tarkistetaan tunnettujen haitallisten linkkien luetteloa vastaan, kun käyttäjä napsauttaa linkkiä**.  <br/> |
|Ladattavan sisällön skannaaminen turvallisten liitteiden avulla  <br/> |Valitse tämä ruutu.  <br/> |
|Soveltaa  <br/> |Vastaanottajan toimi alue on. . . Valitse verkko tunnuksesi.  <br/> |
   
Lisä tietoja on artikkelissa [Office 365 ATP Safe Links](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Siirry Intune-hallinta keskukseen

1. Kirjaudu sisään [Azure-portaaliin](https://portal.azure.com/).

2. Valitse **Kaikki palvelut** ja kirjoita *Intune* **haku kenttään**.

3. Kun tulokset tulevat näkyviin, valitse Aloita **Microsoft Intunen** vierestä, jotta se on suosikki ja helppo löytää myöhemmin.

Hallinta keskuksen lisäksi voit rekisteröidä ja hallinnoida organisaatiosi laitteita Intune-ohjelman avulla. Lisä tietoja on kohdassa [Windows-laitteiden rekisteröinti menetelmän ominaisuudet](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) ja [Intune-menetelmällä hallinnoitujen laitteiden rekisteröinti asetukset](https://docs.microsoft.com/intune/enrollment-options).
