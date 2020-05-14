---
title: Lisää Microsoft 365 for Businessin uhkasuojausta
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
description: Määritä Office 365 Advanced Threat Protection ja suojaa arkaluonteiset tiedot tietojenkalastelulta, haittaohjelmilta ja muilta uhilta.
ms.openlocfilehash: 748868b07ac8759a66bac3c6b4165509270426a6
ms.sourcegitcommit: 6007dbe2cf758c683de399f94023122c678bcada
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/14/2020
ms.locfileid: "44224467"
---
# <a name="increase-threat-protection"></a>Uhkien torjunnan lisääminen

Tämän artikkelin avulla voit parantaa Microsoft 365 -tilauksesi suojausta tietojenkalastelulta, haittaohjelmilta ja muilta uhilta. Nämä suositukset soveltuvat organisaatioille, joilla on lisääntynyt turvallisuustarve, kuten lakitoimistot ja terveydenhuollon klinikat.

Tarkista Office 365:n suojatut pisteet ennen aloittamista. Office 365:n suojatut pisteet analysoi organisaation suojauksen tavallisten aktiviteettien ja suojausasetusten perusteella ja määrittää pisteet. Aloita ottamalla huomioon nykyinen pisteet. Voit lisätä pisteitä suorittamalla tässä artikkelissa suositellut toimet. Tavoitteena ei ole saavuttaa maksimipistemäärää, vaan olla tietoinen mahdollisuuksista suojata ympäristöäsi, joka ei vaikuta käyttäjien tuottavuuteen kielteisesti. 

Lisätietoja on [ohjeaiheessa MicrosoftSecure Score](https://docs.microsoft.com/microsoft-365/security/mtp/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Parantaa suojausta haittaohjelmilta postitse

Office 365- tai Microsoft 365 -ympäristö sisältää suojauksen haittaohjelmilta. Voit parantaa tätä suojausta estämällä liitetiedostoja, joiden tiedostotyyppejä käytetään yleisesti haittaohjelmissa. Haittaohjelmien suojauksen lisääminen sähköpostissa:
  
1. Siirry [https://protection.office.com](https://protection.office.com) sisään ja kirjaudu sisään järjestelmänvalvojan tilisi tunnistetiedoilla. 
    
2. Valitse Suojauksen &amp; yhteensopivuuskeskuksen vasemmanpuoleisen siirtymisruudun **Uhkien hallinta**-kohdasta **Policy** \> **Anti-Malware**.
    
3. Muokkaa tätä yrityksen laajuista käytäntöä kaksoisnapsauttamalla oletuskäytäntöä.
    
4. Valitse **Asetukset**.
    
5. Valitse **Yleiset liitetyyppien suodatus -kohdassa** **Käytössä**. Estetyt tiedostotyypit näkyvät tämän ohjausobjektin alapuolella olevassa ikkunassa. Varmista, että lisäät seuraavat tiedostotyypit:
   - ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif, pif, pif, pif, pif, psh, p  <br/> 
   
   Voit tarvittaessa lisätä tai poistaa tiedostotyyppejä myöhemmin.
    
6. Valitse **Tallenna.**
    
Lisätietoja on ohjeaiheessa [Haittaohjelmien torjunta](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Suojaa kiristysohjelmilta

Kiristysohjelmat rajoittavat tietojen käyttöä salaamalla tiedostoja tai lukitsemalla tietokoneen näyttöjä. Sen jälkeen se yrittää kiristää rahaa uhreilta pyytämällä "lunnaita", yleensä Bitcoinin kaltaisten kryptovaluuttojen muodossa tietojen saantia vastaan. 
  
Jos haluat suojautua kiristysohjelmilta, luo vähintään yksi postin kulkusääntö, joka estää kiristysohjelmille yleisesti käytetyt tiedostotunnisteet. (Lisäsit nämä säännöt [nostaa suojan haittaohjelmilta postin](#raise-the-level-of-protection-against-malware-in-mail) vaiheessa.) Voit myös varoittaa käyttäjiä, jotka vastaanottavat nämä liitteet sähköpostitse.

Edellisessä vaiheessa estämiesi tiedostojen lisäksi on hyvä luoda sääntö, joka varoittaa käyttäjiä ennen makroja sisältävän Office-liitetiedoston avaamisen aloittamista. Ransomware voidaan piilottaa makrojen sisällä, joten varoita käyttäjiä olemaan avaamatta näitä tiedostoja ihmisiltä, joita he eivät tunne.

Voit luoda postin siirtosäännön:
  
1. Siirry -järjestelmänhallintakeskukseen <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> ja valitse **Hallintakeskukset** \> **Exchange**.
    
2. Valitse **postin kulku** -luokassa **säännöt**.
    
3. Valitse **+** ja valitse sitten Luo uusi **sääntö**.
    
4. Valitse valintaikkunan alaosasta **Lisää asetuksia,** niin näet kaikki asetukset. 
    
5. Ota säännön asetukset käyttöön seuraavassa taulukossa. Käytä muiden asetusten oletusarvoja, ellet halua muuttaa niitä.
    
6. Valitse **Tallenna**.
    
|**Asetus**|**Varoita käyttäjiä ennen Office-tiedostojen liitteiden avaamista**||
|:-----|:-----|:-----|
|Nimi  <br/> |Anti-ransomware sääntö: varoittaa käyttäjiä  <br/>  |
|Käytä tätä sääntöä, jos . . .  <br/> |Kaikki liitteet . . . tiedostopääte vastaa . . .  <br/> |
|Sanojen tai lauseiden määrittäminen  <br/> |Lisää seuraavat tiedostotyypit:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Toimi seuraavasti. . .  <br/> |Ilmoita vastaanottajalle viestillä  <br/> |
|Viestin tekstin antaja  <br/> |Älä avaa tämäntyyppisiä tiedostoja ihmisiltä, joita et tunne, koska ne saattavat sisältää makroja, joilla on haitallista koodia.  <br/> |
   
Lisätietoja on seuraavissa artikkeleissa:
  
- [Miten käsitellä ransomware](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [OneDriven palauttaminen](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Sähköpostin automaattisen edelleenlähetyksen lopettaminen

Hakkerit, jotka voivat käyttää käyttäjän postilaatikkoa, voivat varastaa postia asettamalla postilaatikon välittämään sähköpostiviestit automaattisesti. Tämä voi tapahtua myös ilman käyttäjän tietoisuutta. Voit estää tämän määrittämällä postin kulkusäännön. 
  
Voit luoda postin siirtosäännön joko katsomalla [tämän lyhyen videon](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) tai toimimalla seuraavasti:
  
1. Valitse Microsoft 365 -hallintakeskuksessa **Hallintakeskukset** \> **Exchange**.
    
2. Valitse **postin kulku** -luokassa **säännöt**.
    
3. Valitse **+** ja valitse sitten Luo uusi **sääntö**.
    
4. Jos haluat nähdä kaikki asetukset, valitse valintaikkunan alaosasta **Lisää vaihtoehtoja.** 
    
5. Ota asetukset käyttöön seuraavassa taulukossa. Käytä muiden asetusten oletusarvoja, ellet halua muuttaa niitä.
    
6. Valitse **Tallenna**.
    
|**Asetus**|**Varoita käyttäjiä ennen Office-tiedostojen liitteiden avaamista**|
|:-----|:-----|
|Nimi  <br/> |Sähköpostin automaattisen edelleenlähetyksen estäminen ulkoisille verkkotunnuksille  <br/> |
|Käytä tätä sääntöä, jos ...  <br/> |Lähettäjä. . . on ulkoinen/sisäinen . . . Organisaation sisällä  <br/> |
|Lisää ehto  <br/> |Viestin ominaisuudet . . . viestityyppi . . . Automaattinen eteenpäin  <br/> |
|Tee seuraavat ...  <br/> |Estä viesti . . . hylkää viesti ja liitä mukaan selitys.  <br/> |
|Viestin tekstin antaja  <br/> |Tämän organisaation ulkopuolella lähettämisen automaattinen edelleenlähetys estetään turvallisuussyistä.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Sähköpostin suojaaminen tietojenkalasteluhyökkäyksiltä

Jos olet määrittänyt yhden tai useamman mukautetun toimialueen Office 365- tai Microsoft 365 -ympäristöä varten, voit määrittää kohdistetun tietojenkalastelusuojauksen. ATP:n tietojenkalastelun torjunta, joka on osa Office 365 Advanced Threat Protectionia, voi auttaa suojaamaan organisaatiotasi haitallisilta tekeytymispohjaisilta tietojenkalasteluhyökkäyksiltä ja muilta tietojenkalasteluhyökkäyksiltä. Jos et ole määrittänyt mukautettua toimialuetta, sinun ei tarvitse tehdä tätä.
  
Suosittelemme, että aloitat tämän suojauksen luomalla käytännön, joka suojaa tärkeimpiä käyttäjiä ja mukautettua toimialuetta. 

Voit luoda ATP:n tietojenkalastelun vastaisen käytännön katsomalla [tämän lyhyen harjoitusvideon](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)tai suorittamalla seuraavat vaiheet:
  
1. Siirry osoitteeseen [https://protection.office.com](https://protection.office.com). 
    
2. Valitse &amp; Tietoturvan yhteensopivuuskeskuksen vasemmanpuoleisen siirtymisruudun **Uhkien hallinta**-kohdasta **Käytäntö**.
    
3. Valitse **Policy** **Käytäntö-sivulla ATP anti-phishing**.
    
4. Valitse **Tietojenkalastelun torjunta -sivulla** **+ Luo**. Ohjattu toiminto käynnistää toiminnon, jossa voit määrittää tietojenkalastelun vastaisen käytännön.
    
5. Määritä käytännön nimi, kuvaus ja asetukset seuraavassa taulukossa suositellulla tavalla. Lisätietoja on ohjeaiheessa [Lisätietoja ATP:n tietojenkalastelun vastaisista käytäntöasetuksista](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options). 
    
6. Kun olet tarkistanut asetukset, valitse **Luo tämä käytäntö** tai **Tallenna**tarpeen mukaan.
    

|**Asettaminen tai asetus**<br/>|**Suositeltava asetus** <br/>|
|:-----|:-----|
|Nimi  <br/> |Verkkotunnus ja arvokkain kampanjahenkilöstö  <br/> |
|Kuvaus  <br/> |Varmista, että tärkeintä henkilökuntaa ja verkkotunnustamme ei tekeytyisi.  <br/> |
|Käyttäjien lisääminen suojattavaksi  <br/> |Valitse **+ Lisää ehto, Vastaanottaja on**. Kirjoita käyttäjänimet tai kirjoita hakijan, kampanjan hallinnan ja muiden tärkeiden henkilöstön jäsenten sähköpostiosoite. Voit lisätä enintään 20 sisäistä ja ulkoista osoitetta, jotka haluat suojata tekeytymisiltä.  <br/> |
|Suojaamattomien toimialueiden lisääminen  <br/> |Valitse **+ Lisää ehto, Vastaanottajan toimialue on**. Kirjoita Microsoft 365 -tilaukseesi liittyvä mukautettu toimialue, jos olet määrittänyt sellaisen. Voit kirjoittaa useita toimialueita.  <br/> |
|Valitse toiminnot  <br/> |Jos tekeytynyt käyttäjä lähettää sähköpostiviestin: Valitse **Uudelleenohjausviesti toiseen sähköpostiosoitteeseen**ja kirjoita sitten suojauksen valvojan sähköpostiosoite. esimerkiksi *Alice <span> <span> @contoso.com*. Jos sähköpostin lähettää tekeytynyt toimialue: Valitse **Karanteeniviesti**.  <br/> |
|Postilaatikon älykkyys  <br/> |Oletusarvon mukaan postilaatikon älykkyys valitaan, kun luot uuden tietojenkalastelun vastaisen käytännön. Jätä tämä asetus **päälle** parhaan tuloksen saamiseksi.  <br/> |
|Luotettujen lähettäjien ja toimialueiden lisääminen  <br/> |Tähän voit lisätä oman toimialueen tai muita luotettuja verkkotunnuksia.  <br/> |
|Kohdistettu kohteeseen  <br/> |Valitse **Vastaanottajan toimialue on**. Valitse **Jokin näistä**-kohdasta **Valitse**. Valitse **+ Lisää**. Valitse toimialueen nimen vieressä oleva valintaruutu, esimerkiksi *contoso. <span> <span> com*, luettelosta ja valitse sitten **Lisää**. Valitse **Valmis**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Suojaa haitallisilta liitteiltä ja tiedostoilta ATP Safe -liitteiden avulla

Ihmiset lähettävät, vastaanottavat ja jakavat säännöllisesti esimerkiksi asiakirjoja, esityksiä ja laskentataulukoita. Ei ole aina helppoa tietää, onko liite turvallinen vai haitallinen vain tarkastelemalla sähköpostiviestiä. Office 365 Advanced Threat Protection sisältää ATP Safe Attachment -suojauksen, mutta tämä suojaus ei ole oletusarvoisesti käytössä. Suosittelemme, että luot uuden säännön, jotta voit aloittaa tämän suojauksen käyttämisen. Tämä suojaus koskee SharePointin, OneDriven ja Microsoft Teamsin tiedostoja.
  
Voit luoda ATP:n turvallisen liitekäytännön joko katsomalla [tämän lyhyen videon](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)tai suorittamalla seuraavat vaiheet:
  
1. Siirry [https://protection.office.com](https://protection.office.com) kohtaan ja kirjaudu sisään järjestelmänvalvojan tililläsi. 
    
2. Valitse &amp; Tietoturvan yhteensopivuuskeskuksen vasemmanpuoleisen siirtymisruudun **Uhkien hallinta**-kohdasta **Käytäntö**.
    
3. Valitse Käytäntö-sivulla **ATP-turvalliset liitteet**.
    
4. Ota tämä suojaus käyttöön Turvalliset liitteet -sivulla laajasti valitsemalla **Ota ATP sharePointille, OneDrivelle ja Microsoft Teamsille käyttöön** -valintaruutu. 
    
5. Valitse **+** tämä, jos haluat luoda uuden käytännön. 
    
6. Ota asetukset käyttöön seuraavassa taulukossa. 
    
7. Kun olet tarkistanut asetukset, valitse **Luo tämä käytäntö** tai **Tallenna**tarpeen mukaan.
    

|**Asettaminen tai asetus**|**Suositeltava asetus** <br/>|
|:-----|:-----|
|Nimi  <br/> |Estä nykyiset ja tulevat sähköpostit havaituilla haittaohjelmilla.  <br/> |
|Kuvaus  <br/> |Estä nykyiset ja tulevat sähköpostit ja liitteet havaituilla haittaohjelmilla.  <br/> |
|Tallenna liitteet tuntematon haittaohjelmien vastaus  <br/> |Valitse **Estä - Estä nykyiset ja tulevat sähköpostit ja liitteet havaituilla haittaohjelmilla**.  <br/> |
|Uudelleenohjauksen liite tunnistusta varten  <br/> |Ota uudelleenohjaus käyttöön (valitse tämä ruutu) Anna järjestelmänvalvojan tili tai postilaatikon asetukset karanteenia varten.          Käytä yllä olevaa valintaa, jos liitteiden haittaohjelmien tarkistus aikakatkaistaan tai virhe ilmenee (valitse tämä ruutu).  <br/> |
|Kohdistettu kohteeseen  <br/> |Vastaanottajan toimialue on . . . valitse toimialueesi.  <br/> |
   
Lisätietoja on ohjeaiheessa [Office 365 ATP:n tietojenkalastelun torjuntakäytäntöjen määrittäminen](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).
  
## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Suojaa tietojenkalasteluhyökkäyksiltä ATP Safe Linksin avulla

Hakkerit piilottavat joskus haitallisia sivustoja sähköpostin tai muiden tiedostojen linkeissä. Office 365 ATP Safe Links (ATP Safe Links), joka on osa Office 365 Advanced Threat Protectionia, voi auttaa suojaamaan organisaatiotasi tarjoamalla sähköpostiviestien ja Office-asiakirjojen URL-osoitteiden todennuksen. Suojaus määritetään ATP Safe Links -käytäntöjen avulla.
  
Suosittelemme, että teet seuraavat toimet:
  
- Muokkaa oletuskäytäntöä suojauksen parantamiseksi.
    
- Lisää uusi käytäntö, joka on kohdistettu kaikille toimialueen vastaanottajille.
    
Voit määrittää ATP Safe Links -linkit katsomalla [tämän lyhyen harjoitusvideon](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)tai suorittamalla seuraavat vaiheet:
  
1. Siirry [https://protection.office.com](https://protection.office.com) kohtaan ja kirjaudu sisään järjestelmänvalvojan tililläsi. 
    
2. Valitse &amp; Tietoturvan yhteensopivuuskeskuksen vasemmanpuoleisen siirtymisruudun **Uhkien hallinta**-kohdasta **Käytäntö**.
    
3. Valitse Käytäntö-sivulla **ATP Safe Links**.
    
Oletuskäytännön muokkaaminen:
  
1. Valitse Turvalliset linkit -sivun **Käytännöt, jotka koskevat koko organisaatiota**-kohdassa **Oletuskäytäntö.** 
    
2. Valitse **Asetukset, jotka koskevat sisältöä paitsi sähköpostia**-kohdassa Microsoft **365 Apps for enterprise, Office for iOS ja Android**.
    
3. Valitse **Tallenna**. 
    
Voit luoda uuden käytännön, joka on kohdistettu kaikille toimialueen vastaanottajille:
  
1. Luo uusi käytäntö Valitsemalla Turvalliset linkit -sivun **Käytännöt, jotka koskevat koko organisaatiota**koskevat **+** käytännöt -kohdassa. 
    
2. Ota käyttöön seuraavassa taulukossa luetellut asetukset.
    
3. Valitse **Tallenna**. 

|**Asettaminen tai asetus**|**Suositeltava asetus** <br/>|
|:-----|:-----|
|Nimi  <br/> |Kaikkien toimialueen vastaanottajien turvallisten linkkien käytäntö  <br/> |
|Valitse tuntemattomien mahdollisesti haitallisten URL-osoitteiden toiminto viesteissä  <br/> |Valitse **Käytössä - URL-osoitteet kirjoitetaan uudelleen ja verrataan tunnettujen haitallisten linkkien luetteloon, kun käyttäjä napsauttaa linkkiä**.  <br/> |
|Ladattavan sisällön skannaaminen turvallisten liitteiden avulla  <br/> |Valitse tämä ruutu.  <br/> |
|Kohdistettu kohteeseen  <br/> |Vastaanottajan toimialue on . . . valitse toimialueesi.  <br/> |
   
Lisätietoja on kohdassa [Office 365 ATP safe links](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Siirry Intune-hallintakeskukseen

1. Kirjaudu [Azure-portaaliin](https://portal.azure.com/).

2. Valitse **Kaikki palvelut** ja kirjoita **Haku-ruutuun** *Intune* .

3. Kun tulokset tulevat näkyviin, valitse **Microsoft Intunen** vieressä oleva aloitus, jotta se on suosikki ja helppo löytää myöhemmin.

Hallintakeskuksen lisäksi voit käyttää Intusta organisaation laitteiden rekisteröintiin ja hallintaan. Lisätietoja on ohjeessa [Windows-laitteiden rekisteröintimenetelmän](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) ominaisuudet ja [Intunen hallitsemien laitteiden rekisteröintiasetukset](https://docs.microsoft.com/intune/enrollment-options).
