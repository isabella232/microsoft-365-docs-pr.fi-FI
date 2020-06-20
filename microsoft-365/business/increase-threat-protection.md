---
title: Microsoft 365 for Businessin uhkasuojauksen lisääminen
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
description: Määritä Office 365 Advanced Threat Protection ja suojaa arkaluonteisia tietoja tietojen kalastelulta, haittaohjelmilta ja muilta uhilta.
ms.openlocfilehash: d5510cdc082781fd9a1776e86b1bab1d8a2723d6
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/18/2020
ms.locfileid: "44786202"
---
# <a name="increase-threat-protection"></a>Lisää uhkien suojaa

Tämän artikkelin avulla voit parantaa Microsoft 365 -tilauksesi suojausta tietojenkalastelulta, haittaohjelmilta ja muilta uhilta suojautumiseksi. Nämä suositukset soveltuvat organisaatioille, joilla on lisääntynyt turvallisuustarve, kuten lakitoimistot ja terveydenhuollon klinikat.

Ennen kuin aloitat, tarkista Office 365:n suojatut pisteet. Office 365:n suojatut pisteet analysoivat organisaatiosi tietoturvan tavallisten toimintojen ja suojausasetusten perusteella ja määrittää pisteet. Aloita ottamalla huomioon nykyinen pisteet. Voit lisätä pisteitäsi suorittamalla tässä artikkelissa suositellut toimet. Tavoitteena ei ole saavuttaa maksimipisteet, vaan olla tietoinen mahdollisuuksista suojata ympäristöä, joka ei vaikuta kielteisesti käyttäjien tuottavuuteen. 

Lisätietoja on kohdassa [Microsoft Secure Score](https://docs.microsoft.com/microsoft-365/security/mtp/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Nosta suojaustasoa haittaohjelmilta postitse

Office 365- tai Microsoft 365 -ympäristö sisältää suojauksen haittaohjelmilta. Voit lisätä tätä suojausta estämällä liitetiedostot, joiden tiedostotyypit ovat yleisesti haittaohjelmia. Haittaohjelmien suojauksen lisääminen sähköpostissa:
  
1. Siirry [https://protection.office.com](https://protection.office.com) ja kirjaudu sisään järjestelmänvalvojan tilin tunnistetiedoilla. 
    
2. Valitse &amp; Tietoturvan yhteensopivuuskeskuksen vasemman siirtymisruudun **Uhkien hallinta -kohdasta** **Policy** \> **Anti-Malware**.
    
3. Muokkaa tätä yrityksen laajuista käytäntöä kaksoisnapsauttamalla oletuskäytäntöä.
    
4. Valitse **Asetukset**.
    
5. Valitse **Yleiset liitetyyppien suodatus**-kohdassa **Käytössä**. Estetyt tiedostotyypit näkyvät tämän ohjausobjektin alapuolella olevassa ikkunassa. Varmista, että lisäät seuraavat tiedostotyypit:
   - ade, adp, ani, ade, a bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif  <br/> 
   
   Voit tarvittaessa lisätä tai poistaa tiedostotyyppejä myöhemmin.
    
6. Valitse **Tallenna.**
    
Lisätietoja on ohjeaiheessa [Haittaohjelmien torjunta](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Suojaa kiristysohjelmilta

Kiristysohjelmat rajoittavat tietojen käyttöä salaamalla tiedostoja tai lukitsemalla tietokoneen näytöt. Sen jälkeen se yrittää kiristää rahaa uhreilta pyytämällä "lunnaita", yleensä bitcoinien kaltaisten kryptovaluuttojen muodossa vastineeksi tietojen saatavuudesta. 
  
Voit suojata kiristysohjelmia luomalla yhden tai useamman sähköpostivuon säännöt, jotka estävät kiristysohjelmassa yleisesti käytetyt tiedostotunnisteet. (Lisäsit nämä säännöt [nostaa suojan haittaohjelmia vastaan postin](#raise-the-level-of-protection-against-malware-in-mail) vaiheessa.) Voit myös varoittaa käyttäjiä, jotka saavat nämä liitteet sähköpostitse.

Edellisessä vaiheessa estettyjen tiedostojen lisäksi on hyvä luoda sääntö, joka varoittaa käyttäjiä ennen makroja sisältävän Office-liitetiedostojen avaamista. Ransomware voidaan piilottaa sisällä makroja, joten varoittaa käyttäjiä ei avata näitä tiedostoja ihmisiltä he eivät tiedä.

Postin siirtosäännön luominen:
  
1. Siirry hallintakeskukseen kohdassa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> - ja valitse **Exchangen hallintakeskukset** \> **Exchange**.
    
2. Valitse **postin kulkuluokasta** **säännöt**.
    
3. Valitse **+** ja valitse sitten Luo uusi **sääntö**.
    
4. Valitse valintaikkunan alaosasta **Lisää asetuksia,** niin näet kaikki asetukset. 
    
5. Ota säännön asetukset käyttöön seuraavassa taulukossa. Käytä muiden asetusten oletusarvoja, ellet halua muuttaa niitä.
    
6. Valitse **Tallenna**.
    
|**Asetus**|**Varoita käyttäjiä ennen Office-tiedostojen liitteiden avaamista**||
|:-----|:-----|:-----|
|Nimi  <br/> |Ransomware-estosääntö: varoita käyttäjiä  <br/>  |
|Käytä tätä sääntöä, jos . . .  <br/> |Kaikki liitteet. . . tiedostopääte vastaa . . .  <br/> |
|Sanojen tai lauseiden määrittäminen  <br/> |Lisää seuraavat tiedostotyypit:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Toimi seuraavasti. . .  <br/> |Ilmoita vastaanottajalle viestillä  <br/> |
|Viestin tekstin kirjoittaminen  <br/> |Älä avaa tällaisia tiedostoja ihmisiltä, joita et tunne, koska ne saattavat sisältää makroja, joissa on haitallista koodia.  <br/> |
   
Lisätietoja on seuraavissa artikkeleissa:
  
- [Miten käsitellä ransomware](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [OneDriven palauttaminen](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Sähköpostin automaattisen edelleenlähetyksen lopettaminen

Hakkerit, jotka pääsevät käyttäjän postilaatikkoon, voivat varastaa sähköpostia määrittämällä postilaatikon lähettämään sähköpostin automaattisesti edelleen. Tämä voi tapahtua myös ilman käyttäjän tietoisuutta. Voit estää tämän määrittämällä sähköpostin kulkusääntöä. 
  
Voit luoda sähköpostin siirtosäännön katsomalla [tämän lyhyen videon](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) tai noudattamalla seuraavia ohjeita:
  
1. Valitse Microsoft 365 -hallintakeskuksessa **Exchangen hallintakeskukset** \> **Exchange**.
    
2. Valitse **postin kulkuluokasta** **säännöt**.
    
3. Valitse **+** ja valitse sitten Luo uusi **sääntö**.
    
4. Jos haluat nähdä kaikki vaihtoehdot, valitse valintaikkunan alareunasta **Lisää asetuksia.** 
    
5. Ota asetukset käyttöön seuraavassa taulukossa. Käytä muiden asetusten oletusarvoja, ellet halua muuttaa niitä.
    
6. Valitse **Tallenna**.
    
|**Asetus**|**Varoita käyttäjiä ennen Office-tiedostojen liitteiden avaamista**|
|:-----|:-----|
|Nimi  <br/> |Sähköpostin automaattisen edelleenlähetyksen estäminen ulkoisille verkkotunnuksille  <br/> |
|Käytä tätä sääntöä, jos ...  <br/> |Lähettäjä. . . on ulkoinen/sisäinen. . . Organisaation sisällä  <br/> |
|Lisää ehto  <br/> |Viestin ominaisuudet . . . sisältää sanomatyypin . . . Automaattinen eteenpäin  <br/> |
|Tee seuraavat ...  <br/> |Estä viesti . . . hylätä viestin ja sisältää selityksen.  <br/> |
|Viestin tekstin kirjoittaminen  <br/> |Sähköpostin automaattinen edelleenlähetys tämän organisaation ulkopuolella estetään turvallisuussyistä.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Sähköpostin suojaaminen tietojenkalasteluhyökkäyksiltä

Jos olet määrittänyt yhden tai useamman mukautetun toimialueen Office 365- tai Microsoft 365 -ympäristölle, voit määrittää kohdennetun tietojenkalastelun torjunnan. ATP-tietojenkalastelun torjunta, joka on osa Office 365 Advanced Threat Protection -suojausta, voi auttaa suojaamaan organisaatiotasi haitallisilta tekeytymispohjaisilta tietojenkalasteluhyökkäyksiltä ja muilta tietojenkalasteluhyökkäyksiltä. Jos et ole määrittänyt mukautettua toimialuetta, sinun ei tarvitse tehdä tätä.
  
Suosittelemme, että aloitat tämän suojauksen luomalla käytännön, joka suojaa tärkeimpiä käyttäjiäsi ja mukautettua toimialuettasi. 

Voit luoda ATP-tietojenkalastelun torjuntakäytännön katsomalla [tämän lyhyen harjoitusvideon](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)tai suorittamalla seuraavat vaiheet:
  
1. Siirry osoitteeseen [https://protection.office.com](https://protection.office.com). 
    
2. Valitse &amp; Tietoturvan yhteensopivuuskeskuksen vasemmanpuoleisen siirtymisruudun **Uhkien hallinta -kohdasta** **Käytäntö**.
    
3. Valitse **Policy** **Käytäntö-sivulla ATP-tietojenkalastelun torjunta**.
    
4. Valitse **Tietojenkalastelun torjunta -sivulla** **+ Luo**. Ohjattu toiminto käynnistää toiminnon, joka määrittää tietojenkalastelun torjuntakäytännön.
    
5. Määritä käytännön nimi, kuvaus ja asetukset seuraavassa taulukossa suositellulla tavalla. Lisätietoja on [ohjeaiheessa Lisätietoja ATP:n tietojenkalastelun torjuntakäytännöistä](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options). 
    
6. Kun olet tarkistanut asetuksesi, valitse **Luo tämä käytäntö** tai **Tallenna**tarpeen mukaan.
    

|**Asetus tai asetus**<br/>|**Suositeltu asetus** <br/>|
|:-----|:-----|
|Nimi  <br/> |Verkkotunnus ja arvokkain kampanjahenkilöstö  <br/> |
|Kuvaus  <br/> |Varmista, että tärkeintä henkilökuntaamme ja verkkotunnustamme ei tekeytyä.  <br/> |
|Käyttäjien lisääminen suojattavaksi  <br/> |Valitse **+ Lisää ehto, Vastaanottaja on**. Kirjoita käyttäjänimet tai kirjoita hakijan, kampanjapäällikön ja muiden tärkeiden toimihenkilöiden sähköpostiosoite. Voit lisätä enintään 20 sisäistä ja ulkoista osoitetta, jotka haluat suojata tekeytymiltä.  <br/> |
|Suojaamien toimialueiden lisääminen  <br/> |Valitse **+ Lisää ehto, Vastaanottajatoimialue on**. Kirjoita Microsoft 365 -tilaukseesi liittyvä mukautettu toimialue, jos olet määrittänyt sellaisen. Voit kirjoittaa useita toimialueita.  <br/> |
|Valitse toiminnot  <br/> |Jos tekeytyneen käyttäjän lähettämä sähköposti lähettää sähköpostiviestin: Valitse **Uudelleenohjausviesti toiseen sähköpostiosoitteeseen**ja kirjoita sitten suojauksen järjestelmänvalvojan sähköpostiosoite. Esimerkiksi *Alice <span> <span> @contoso.com*. Jos sähköpostiviestin lähettää tekeytynyt toimialue: Valitse **Karanteeniviesti**.  <br/> |
|Postilaatikon tietojen  <br/> |Oletusarvon mukaan postilaatikon tietotiedot valitaan, kun luot uuden tietojenkalastelun vastaisen käytännön. Jätä tämä asetus **Käytössä,** jotta saat parhaat tulokset.  <br/> |
|Luotettujen lähettäjien ja toimialueiden lisääminen  <br/> |Tähän voit lisätä oman toimialueen tai muita luotettuja toimialueita.  <br/> |
|Sovelletaan  <br/> |Valitse **Vastaanottajatoimialue on**. Valitse **Jokin näistä**-kohdassa **Valitse**. Valitse **+ Lisää**. Valitse toimialueen nimen vieressä oleva valintaruutu, esimerkiksi *contoso. <span> <span> com*ja valitse sitten **Lisää**. Valitse **Valmis**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Suojaa haitallisilta liitteiltä ja tiedostoilta ATP Safe Attachments -ohjelmiston avulla

Käyttäjät lähettävät, vastaanottavat ja jakavat säännöllisesti liitteitä, kuten asiakirjoja, esityksiä, laskentataulukoita ja paljon muuta. Aina ei ole helppoa tietää, onko liite turvallinen vai haitallinen vain sähköpostiviestistä. Office 365 Advanced Threat Protection sisältää ATP Safe Attachment -suojauksen, mutta tämä suojaus ei ole oletusarvoisesti käytössä. Suosittelemme, että luot uuden säännön, jotta voit aloittaa tämän suojauksen käyttämisen. Tämä suojaus koskee SharePointin, OneDriven ja Microsoft Teamsin tiedostoja.
  
Voit luoda ATP-turvallisen liitekäytännön joko [katsomalla tämän lyhyen videon](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)tai suorittamalla seuraavat vaiheet:
  
1. Siirry -kohtaan [https://protection.office.com](https://protection.office.com) ja kirjaudu sisään järjestelmänvalvojan tililläsi. 
    
2. Valitse &amp; Tietoturvan yhteensopivuuskeskuksen vasemmanpuoleisen siirtymisruudun **Uhkien hallinta -kohdasta** **Käytäntö**.
    
3. Valitse Käytäntö-sivulla **ATP:n turvalliset liitteet**.
    
4. Käytä Turvalliset liitteet -sivulla tätä suojausta laajasti valitsemalla **Ota ATP käyttöön SharePointissa, OneDrivessa ja Microsoft Teamsissa** -valintaruutu. 
    
5. Valitse **+** tämä, jos haluat luoda uuden käytännön. 
    
6. Ota asetukset käyttöön seuraavassa taulukossa. 
    
7. Kun olet tarkistanut asetuksesi, valitse **Luo tämä käytäntö** tai **Tallenna**tarpeen mukaan.
    

|**Asetus tai asetus**|**Suositeltu asetus** <br/>|
|:-----|:-----|
|Nimi  <br/> |Estä nykyiset ja tulevat sähköpostit, joissa on havaittuja haittaohjelmia.  <br/> |
|Kuvaus  <br/> |Estä nykyiset ja tulevat sähköpostit ja liitteet havaituilla haittaohjelmilla.  <br/> |
|Tallenna liitetiedostoja tuntematon haittaohjelmien vastaus  <br/> |Valitse **Block - Estä nykyiset ja tulevat sähköpostit ja liitteet, joissa on havaitut haittaohjelmat**.  <br/> |
|Uudelleenohjaa liite tunnistuksen  <br/> |Ota uudelleenohjaus käyttöön (valitse tämä ruutu) Anna järjestelmänvalvojan tili tai postilaatikon karanteeniasetukset.          Käytä yllä olevaa valintaa, jos liitteiden haittaohjelmien tarkistus aika loppuu tai tapahtuu virhe (valitse tämä ruutu).  <br/> |
|Sovelletaan  <br/> |Vastaanottajan toimialue on . . . valitse toimialueesi.  <br/> |
   
Lisätietoja on [ohjeaiheessa Office 365 ATP:n tietojenkalastelun torjuntakäytäntöjen määrittäminen](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).
  
## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Suojaa tietojenkalasteluhyökkäyksiltä ATP Safe Links -yhteydellä

Hakkerit piilottavat joskus haitalliset sivustot sähköpostin tai muiden tiedostojen linkeissä. Office 365 ATP Safe Links (ATP Safe Links), joka on osa Office 365 Advanced Threat Protectionia, voi auttaa suojaamaan organisaatiotasi tarkistamalla verkko-osoitteet (URL-osoitteet) sähköpostiviesteissä ja Office-asiakirjoissa. Suojaus määritellään ATP Safe Links -käytäntöjen avulla.
  
Suosittelemme, että toimit seuraavasti:
  
- Paranna suojausta muokkaamalla oletuskäytäntöä.
    
- Lisää uusi käytäntö, joka on kohdistettu kaikille toimialueen vastaanottajille.
    
Voit määrittää ATP Safe Links -linkit katsomalla [tämän lyhyen harjoitusvideon](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)tai suorittamalla seuraavat vaiheet:
  
1. Siirry -kohtaan [https://protection.office.com](https://protection.office.com) ja kirjaudu sisään järjestelmänvalvojan tililläsi. 
    
2. Valitse &amp; Tietoturvan yhteensopivuuskeskuksen vasemmanpuoleisen siirtymisruudun **Uhkien hallinta -kohdasta** **Käytäntö**.
    
3. Valitse Käytäntö-sivulla **ATP Safe Links**.
    
Oletuskäytännön muokkaaminen:
  
1. Valitse Turvalliset linkit -sivun **Käytännöt, jotka koskevat koko organisaatiota**-kohdassa **Oletuskäytäntö.** 
    
2. Valitse **Asetukset, jotka koskevat sisältöä sähköpostin lisäksi**-kohdassa Microsoft **365 Apps for enterprise, Office for iOS ja Android**.
    
3. Valitse **Tallenna**. 
    
Voit luoda uuden käytännön, joka on kohdistettu kaikille toimialueen vastaanottajille:
  
1. Luo uusi käytäntö valitsemalla Turvalliset linkit -sivun **Käytännöt, jotka koskevat koko organisaatiota** **+** -kohdassa. 
    
2. Ota käyttöön seuraavassa taulukossa luetellut asetukset.
    
3. Valitse **Tallenna**. 

|**Asetus tai asetus**|**Suositeltu asetus** <br/>|
|:-----|:-----|
|Nimi  <br/> |Kaikkien toimialueen vastaanottajien turvallisten linkkien käytäntö  <br/> |
|Valitse viestien tuntemattomien mahdollisesti haitallisten URL-osoitteiden toiminto  <br/> |Valitse **Käytössä - URL-osoitteet kirjoitetaan uudelleen ja verrataan tunnettujen haitallisten linkkien luetteloon, kun käyttäjä napsauttaa linkkiä**.  <br/> |
|Ladattavan sisällön skannaaminen turvallisten liitteiden avulla  <br/> |Valitse tämä ruutu.  <br/> |
|Sovelletaan  <br/> |Vastaanottajan toimialue on . . . valitse toimialueesi.  <br/> |
   
Lisätietoja on kohdassa [Office 365 ATP -turvalinkit](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Siirry Intune-hallintakeskukseen

1. Kirjaudu [Azure-portaaliin](https://portal.azure.com/).

2. Valitse **Kaikki palvelut** ja kirjoita **hakuruutuun** *Intune* .

3. Kun tulokset tulevat näkyviin, valitse **Microsoft Intunen** vieressä oleva alku, jotta se olisi suosikki ja helppo löytää myöhemmin.

Hallintakeskuksen lisäksi voit rekisteröidä ja hallita organisaation laitteita Intunen avulla. Lisätietoja on ohjeissa [Windows-laitteiden rekisteröintimenetelmän](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) ominaisuudet ja [Intunen hallitsemien laitteiden rekisteröintiasetukset](https://docs.microsoft.com/intune/enrollment-options).
