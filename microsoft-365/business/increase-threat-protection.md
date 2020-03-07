---
title: Lisää Microsoft 365 Businessin uhkien suojausta
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
ms.openlocfilehash: 17425de3f6e0022945899a559cf88575b6315a56
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561606"
---
# <a name="increase-threat-protection"></a>Uhkien torjunnan lisääminen

Tämän artikkelin avulla voit parantaa Microsoft 365 -tilauksesi suojausta tietojenkalastelulta, haittaohjelmilta ja muilta uhilta suojautumiseksi. Nämä suositukset soveltuvat organisaatioille, joilla on lisääntynyt turvallisuustarve, kuten lakitoimistot ja terveydenhuoltokeskukset.

Tarkista Office 365:n suojatut pisteet ennen aloittamista. Office 365:n suojatut pisteet analysoiOffice 365 -organisaatiosi suojauksen säännöllisten toimintojen ja suojausasetusten perusteella ja määrittää tuloksen. Aloita merkitsemällä huomioitavaa nykyiset pisteet. Voit lisätä pisteitä suorittamalla tässä artikkelissa suositellut toimet. Tavoitteena ei ole saavuttaa maksimipistemäärää, vaan olla tietoinen mahdollisuuksista suojata ympäristöäsi, jotka eivät vaikuta kielteisesti käyttäjien tuottavuuteen. 

Lisätietoja on ohjeaiheessa [Microsoftin suojatut pisteet](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Nosta suojausta haittaohjelmilta sähköpostissa

Office 365- tai Microsoft 365 -ympäristö sisältää suojauksen haittaohjelmilta. Voit parantaa tätä suojausta estämällä liitetiedostot tiedostotyypeillä, joita käytetään yleisesti haittaohjelmissa. Haittaohjelmien suojauksen lisääminen sähköpostissa:
  
1. Siirry [https://protection.office.com](https://protection.office.com) järjestelmänvalvojan tilisi tunnistetietoihin ja kirjaudu sisään. 
    
2. Valitse Office 365 &amp; Security Compliance Centerin vasemmanpuoleisen siirtymisruudun **Uhkajenhallinta**-kohdasta **Käytäntö** \> **haittaohjelmien torjunta**.
    
3. Muokkaa tätä yrityksen laajuista käytäntöä kaksoisnapsauttamalla oletuskäytäntöä.
    
4. Valitse **Asetukset**.
    
5. Valitse **Yleiset liitetyypit -suodattimessa** **Käytössä**. Estetyt tiedostotyypit näkyvät tämän ohjausobjektin alapuolella olevassa ikkunassa. Varmista, että lisäät seuraavat tiedostotyypit:
   - Ade, ADP, Ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, inf, ins, isp, työ, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif, pif,  <br/> 
   
   Voit tarvittaessa lisätä tai poistaa tiedostotyyppejä myöhemmin.
    
6. Valitse **Tallenna.**
    
Lisätietoja on ohjeaiheessa [Haittaohjelmien torjunta](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Suojaa kiristysohjelmilta

Ransomware rajoittaa tietojen käyttöä salaamalla tiedostoja tai lukitsemalla tietokoneen näyttöjä. Sen jälkeen se yrittää kiristää rahaa uhreilta pyytämällä "lunnaita", yleensä bitcoinien kaltaisten kryptovaluuttojen muodossa vastineeksi tietojen saatavuudesta. 
  
Voit suojautua kiristysohjelmilta luomalla yhden tai useamman postin kulkusääntöjä estääksesi kiristysohjelmien tiedostotunnisteet. (Olet lisännyt nämä säännöt [nostaa suojelun tasoa haittaohjelmia postin](#raise-the-level-of-protection-against-malware-in-mail) vaiheessa.) Voit myös varoittaa käyttäjiä, jotka saavat nämä liitteet sähköpostitse.

Edellisessä vaiheessa estämiesi tiedostojen lisäksi on hyvä luoda sääntö, joka varoittaa käyttäjiä ennen makroja sisältävän Office-liitetiedoston avaamista. Ransomware voidaan piilottaa makrojen sisällä, joten varoita käyttäjiä olemaan avaamatta näitä tiedostoja ihmisiltä, joita he eivät tunne.

Postin siirtosäännön luominen:
  
1. Siirry <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>hallintakeskukseen -kohdasta ja valitse **Hallintakeskukset** \> **Exchange**.
    
2. Valitse **postin työnkulkuluokasta** **säännöt**.
    
3. Valitse **+** ja valitse sitten **Luo uusi sääntö**.
    
4. Valitse valintaikkunan alaosasta **Lisää asetuksia,** niin näet kaikki asetukset. 
    
5. Ota säännön asetukset käyttöön seuraavassa taulukossa. Käytä muiden asetusten oletusarvoja, ellet halua muuttaa niitä.
    
6. Valitse **Tallenna**.
    
|**Asetus**|**Käyttäjien varoittaminen ennen Office-tiedostojen liitteiden avaamista**||
|:-----|:-----|:-----|
|Nimi  <br/> |Anti-ransomware sääntö: varoittaa käyttäjiä  <br/>  |
|Käytä tätä sääntöä, jos . . .  <br/> |Mikä tahansa kiinnitys . . . tiedostotunniste vastaa . . .  <br/> |
|Sanojen tai lauseiden määrittäminen  <br/> |Lisää seuraavat tiedostotyypit:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Toimi seuraavasti. . .  <br/> |Ilmoita vastaanottajalle viestillä  <br/> |
|Viestin tekstin anto  <br/> |Älä avaa tämäntyyppisiä tiedostoja ihmisiltä, joita et tunne, koska ne saattavat sisältää makroja, joissa on haitallista koodia.  <br/> |
   
Lisätietoja on seuraavissa artikkeleissa:
  
- [Miten käsitellä ransomware](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [OneDriven palauttaminen](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Sähköpostin automaattisen edelleenlähetyksen lopettaminen

Hakkerit, jotka pääsevät käyttäjän postilaatikkoon, voivat varastaa sähköpostia asettamalla postilaatikon välittämään sähköpostin automaattisesti. Tämä voi tapahtua myös ilman käyttäjän tietoisuutta. Voit estää tämän määrittämällä postin kulkusäännön. 
  
Voit luoda postin siirtosäännön joko katsomalla [tämän lyhyen videon](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) tai toimimalla seuraavasti:
  
1. Valitse Microsoft 365 -hallintakeskuksessa **Hallintakeskukset** \> **Exchange**.
    
2. Valitse **postin työnkulkuluokasta** **säännöt**.
    
3. Valitse **+** ja valitse sitten **Luo uusi sääntö**.
    
4. Jos haluat nähdä kaikki vaihtoehdot, valitse valintaikkunan alaosasta **Lisää asetuksia.** 
    
5. Ota seuraavan taulukon asetukset käyttöön. Käytä muiden asetusten oletusarvoja, ellet halua muuttaa niitä.
    
6. Valitse **Tallenna**.
    
|**Asetus**|**Käyttäjien varoittaminen ennen Office-tiedostojen liitteiden avaamista**|
|:-----|:-----|
|Nimi  <br/> |Sähköpostin automaattisen edelleenlähetyksen estäminen ulkoisille toimialueille  <br/> |
|Käytä tätä sääntöä, jos ...  <br/> |Lähettäjä. . . on ulkoinen/sisäinen. . . Organisaation sisällä  <br/> |
|Lisää ehto  <br/> |Sanoman ominaisuudet . . . viestin tyyppi . . . Automaattinen eteenpäin  <br/> |
|Tee seuraavat ...  <br/> |Estä viesti . . . hylkää viesti ja liitä mukaan selitys.  <br/> |
|Viestin tekstin anto  <br/> |Sähköpostin automaattinen edelleenlähetys tämän organisaation ulkopuolella estetään turvallisuussyistä.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Sähköpostin suojaaminen tietojenkalasteluhyökkäyksiltä

Jos olet määrittänyt office 365- tai Microsoft 365 -ympäristölle yhden mukautetun toimialueen, voit määrittää kohdennetun tietojenkalastelun torjunnan. ATP-tietojenkalastelun torjunta, joka on osa Office 365 Advanced Threat Protectionia, voi auttaa suojaamaan organisaatiotasi haitallisilta tekeytymispohjaisilta tietojenkalasteluhyökkäyksiltä ja muilta tietojenkalasteluhyökkäyksiltä. Jos et ole määrittänyt mukautettua toimialuetta, sinun ei tarvitse tehdä tätä.
  
Suosittelemme, että aloitat tämän suojauksen luomalla käytännön, joka suojaa tärkeimpiä käyttäjiäja mukautettua toimialuetta. 

Voit luoda ATP-tietojenkalastelun vastaisen käytännön katsomalla [tämän lyhyen harjoitusvideon](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)tai suorittamalla seuraavat toimet:
  
1. Siirry osoitteeseen [https://protection.office.com](https://protection.office.com). 
    
2. Valitse Office 365 &amp; Security Compliance Centerin vasemmanpuoleisen siirtymisruudun **Uhkahallinta-kohdassa** **Käytäntö**.
    
3. Valitse **Käytäntö-sivulla** **ATP-tietojenkalastelun torjunta**.
    
4. Valitse **Tietojenkalastelun torjunta** -sivulla **+ Luo**. Ohjattu toiminto käynnistyy, joka opastaa tietojenkalastelun torjuntakäytännön määrittämisessä.
    
5. Määritä käytännön nimi, kuvaus ja asetukset seuraavassa taulukossa suositellulla tavalla. Lisätietoja on ohjeaiheessa [Lisätietoja ATP:n tietojenkalastelun vastaisista käytäntövaihtoehdoista](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options). 
    
6. Kun olet tarkistanut asetuksesi, valitse **Luo tämä käytäntö** tai **Tallenna**tarpeen mukaan.
    

|**Asettaminen tai asetus**<br/>|**Suositeltava asetus** <br/>|
|:-----|:-----|
|Nimi  <br/> |Verkkotunnus ja arvokkain kampanjahenkilöstö  <br/> |
|Kuvaus  <br/> |Varmista, että tärkeintä henkilökuntaa mme ja verkkotunnustamme ei tekeyty.  <br/> |
|Käyttäjien lisääminen suojattavaksi  <br/> |Valitse **+ Lisää ehto, Vastaanottaja on**. Kirjoita käyttäjänimi tai kirjoita ehdokkaan, kampanjan hallinnan ja muiden tärkeiden henkilökunnan jäsenten sähköpostiosoite. Voit lisätä enintään 20 sisäistä ja ulkoista osoitetta, jotka haluat suojata tekeytymisiltä.  <br/> |
|Suojaata vanlleta toimialueiden lisääminen  <br/> |Valitse **+ Lisää ehto, Vastaanottajan toimialue on**. Kirjoita Microsoft 365 -tilaukseesi liittyvä mukautettu toimialue, jos olet määrittänyt sellaisen. Voit kirjoittaa useita toimialueita.  <br/> |
|Valitse toiminnot  <br/> |Jos tekeytynyt käyttäjä lähettää sähköpostiviestin: Valitse **Uudelleenohjausviesti toiseen sähköpostiosoitteeseen**ja kirjoita sitten suojauksen valvojan sähköpostiosoite. Esimerkiksi *Alice<span><span>@contoso.com*. Jos sähköpostin lähettää tekeytynyt toimialue: Valitse **Karanteeniviesti**.  <br/> |
|Postilaatikon tietojen määrittäminen  <br/> |Oletusarvon mukaan postilaatikon tietotiedot valitaan, kun luot uuden tietojenkalastelun vastaisen käytännön. Jätä tämä asetus **päälle** parhaan tuloksen saamiseksi.  <br/> |
|Luotettavien lähettäjien ja toimialueiden lisääminen  <br/> |Tähän voit lisätä oman toimialueen tai muita luotettuja toimialueita.  <br/> |
|Kohdistetaan  <br/> |Valitse **Vastaanottajatoimialue on**. Valitse **Jokin näistä**-kohdasta **Valitse**. Valitse **+ Lisää**. Valitse toimialueen nimen vieressä oleva valintaruutu, esimerkiksi *contoso.<span> com <span>*, luettelosta ja valitse sitten **Lisää**. Valitse **Valmis**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Suojaa haitallisilta liitteiltä ja tiedostoilta ATP Safe Attachmentsin avulla

Käyttäjät lähettävät, vastaanottavat ja jakavat säännöllisesti liitteitä, kuten asiakirjoja, esityksiä, laskentataulukoita ja paljon muuta. Aina ei ole helppo sanoa, onko liite turvallinen vai haitallinen vain katsomalla sähköpostiviestiä. Office 365 Advanced Threat Protection sisältää ATP Safe Attachment -suojauksen, mutta tämä suojaus ei ole oletusarvoisesti käytössä. Suosittelemme, että luot uuden säännön tämän suojauksen käytön aloittamiseksi. Tämä suojaus koskee SharePointin, OneDriven ja Microsoft Teamsin tiedostoja.
  
Voit luoda ATP:n turvallisen liitekäytännön joko katsomalla [tämän lyhyen videon](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)tai suorittamalla seuraavat vaiheet:
  
1. Siirry [https://protection.office.com](https://protection.office.com)-kohtaan ja kirjaudu sisään järjestelmänvalvojan tililläsi. 
    
2. Valitse Office 365 &amp; Security Compliance Centerin vasemmanpuoleisen siirtymisruudun **Uhkahallinta-kohdassa** **Käytäntö**.
    
3. Valitse Käytäntö-sivulla **ATP-turvalliset liitteet**.
    
4. Käytä Tätä suojausta Turvalliset liitteet -sivulla laajasti valitsemalla **Ota ATP käyttöön SharePointille, OneDrivelle ja Microsoft Teamsille** -valintaruutu. 
    
5. Valitse **+** tämä, jos haluat luoda uuden käytännön. 
    
6. Ota seuraavan taulukon asetukset käyttöön. 
    
7. Kun olet tarkistanut asetuksesi, valitse **Luo tämä käytäntö** tai **Tallenna**tarpeen mukaan.
    

|**Asettaminen tai asetus**|**Suositeltava asetus** <br/>|
|:-----|:-----|
|Nimi  <br/> |Estä nykyiset ja tulevat sähköpostit havaituilla haittaohjelmilla.  <br/> |
|Kuvaus  <br/> |Estä nykyiset ja tulevat sähköpostit ja liitteet havaituilla haittaohjelmilla.  <br/> |
|Tallenna liitetiedostoja tuntematon haittaohjelmien vastaus  <br/> |Valitse **Estä - Estä nykyiset ja tulevat sähköpostit ja liitteet havaituilla haittaohjelmilla**.  <br/> |
|Uudelleenohjausliite tunnistuksessa  <br/> |Ota uudelleenohjaus käyttöön (valitse tämä ruutu) Anna järjestelmänvalvojan tili tai postilaatikon asetukset karanteenia varten.          Käytä yllä olevaa valintaa, jos liitetiedostojen haittaohjelmien tarkistus aikakatkaistaan tai tapahtuu virhe (valitse tämä ruutu).  <br/> |
|Kohdistetaan  <br/> |Vastaanottajan toimialue on . . . valitse toimialueesi.  <br/> |
   
Lisätietoja on ohjeaiheessa [Office 365 ATP:n tietojenkalastelun torjuntakäytäntöjen määrittäminen](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Suojaa tietojenkalasteluhyökkäyksiltä ATP Safe Linksin avulla

Hakkerit piilottavat joskus haitalliset sivustot sähköpostin tai muiden tiedostojen linkeissä. Office 365 ATP Safe Links (ATP Safe Links), joka on osa Office 365 Advanced Threat Protectionia, voi auttaa suojaamaan organisaatiotasi antamalla sähköpostiviesteissä ja Office-asiakirjoissa www-osoitteiden (URL-osoitteiden) reaaliaikaisen tarkistamisen. Suojaus määritetään ATP Safe Links -käytäntöjen avulla.
  
Suosittelemme, että toimit seuraavasti:
  
- Lisää suojausta muokkaamalla oletuskäytäntöä.
    
- Lisää uusi käytäntö, joka on kohdistettu kaikille toimialueen vastaanottajille.
    
Voit määrittää ATP Safe Links -linkit katsomalla [tämän lyhyen harjoitusvideon](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)tai suorittamalla seuraavat vaiheet:
  
1. Siirry [https://protection.office.com](https://protection.office.com)-kohtaan ja kirjaudu sisään järjestelmänvalvojan tililläsi. 
    
2. Valitse Office 365 &amp; Security Compliance Centerin vasemmanpuoleisen siirtymisruudun **Uhkahallinta-kohdassa** **Käytäntö**.
    
3. Valitse Käytäntö-sivulla **ATP Safe Links**.
    
Oletuskäytännön muokkaaminen:
  
1. Valitse Turvalliset linkit -sivun **Koko organisaatiota koskevat käytännöt**-kohdassa **Oletuskäytäntö.** 
    
2. Valitse **Asetukset, jotka koskevat sisältöä sähköpostia lukuun ottamatta**-kohdassa **Office 365 ProPlus, Office for iOS ja Android**.
    
3. Valitse **Tallenna**. 
    
Voit luoda uuden käytännön, joka on kohdistettu kaikille toimialueen vastaanottajille:
  
1. Luo uusi käytäntö Valitsemalla Turvalliset linkit -sivun **Koko organisaatiota koskevat käytännöt**-kohdassa **+** uusi käytäntö. 
    
2. Ota käyttöön seuraavassa taulukossa luetellut asetukset.
    
3. Valitse **Tallenna**. 

|**Asettaminen tai asetus**|**Suositeltava asetus** <br/>|
|:-----|:-----|
|Nimi  <br/> |Turvalinkkikäytäntö kaikille toimialueen vastaanottajille  <br/> |
|Valitse viestien tuntemattomien mahdollisesti haitallisten URL-osoitteiden toiminto  <br/> |Valitse **Käytössä - URL-osoitteet kirjoitetaan uudelleen ja verrataan tunnettujen haitallisten linkkien luetteloon, kun käyttäjä napsauttaa linkkiä**.  <br/> |
|Ladattavan sisällön skannaaminen turvallisten liitteiden avulla  <br/> |Valitse tämä ruutu.  <br/> |
|Kohdistetaan  <br/> |Vastaanottajan toimialue on . . . valitse toimialueesi.  <br/> |
   
Lisätietoja on ohjeaiheessa [Office 365 ATP:n turvalliset linkit](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Siirry Intune-hallintakeskukseen

1. Kirjaudu [Azure-portaaliin](https://portal.azure.com/).

2. Valitse **Kaikki palvelut** ja kirjoita **Hakuruutu -kenttään** *Intune.*

3. Kun tulokset tulevat näkyviin, valitse **Microsoft Intune** -kohdan vieressä oleva aloitus, jotta se olisi suosikki ja helppo löytää myöhemmin.

Hallintakeskuksen lisäksi voit käyttää Intunen avulla organisaation laitteiden rekisteröintiä ja hallintaa. Lisätietoja on ohjeen apterisessa kohdassa [Windows-laitteiden ominaisuudet rekisteröintimenetelmän mukaan](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) ja [Intunen hallitsemien laitteiden rekisteröintiasetukset](https://docs.microsoft.com/intune/enrollment-options).
