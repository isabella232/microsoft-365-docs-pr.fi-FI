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
ms.openlocfilehash: b6e9941eee9de4f295b0f8056c1c91b7076e530c
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086315"
---
# <a name="increase-threat-protection"></a>Suurenna threat protection

Tämä artikkeli auttaa sinua lisäämään suojaus-Microsoft 365-tilauksesi phishing, haittaohjelmia ja muita uhkia vastaan. Nämä suositukset soveltuvat organisaatioiden kanssa tietoturva laki- ja terveydenhuollon klinikat kuten lisääntynyt tarve.

Ennen kuin aloitat, Tarkista Office 365: n Secure pisteet. Office 365: n Secure pisteet analysoi Office 365-organisaatiosi suojaus perustuu toiminnan säännöllinen ja suojausasetukset ja määrittää pistemäärän. Aloita panee merkille nykyisen pistemäärää. Pistemäärä kasvaa suositella tämän artikkelin toimilla. Tavoite ei ole saavuttaa Maksimi pisteet, vaan olla tietoinen mahdollisuuksia ympäristön suojelemiseksi, jotka eivät vaikuta kielteisesti käyttäjien tuottavuutta. 

Lisätietoja [Microsoft Secure pisteet](https://docs.microsoft.com/en-us/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Nosta suojan haittaohjelmilta, sähköposti

Office 365: ssä tai Microsoft 365-ympäristösi sisältää haittaohjelmia vastaan, mutta voi parantaa suojaus liitetiedostojen eston tiedostotyypit, joita yleisesti käytetään haittaohjelmien kanssa. Kasvattaminen haittaohjelmilta sähköpostitse:
  
1. Siirry [https://protection.office.com](https://protection.office.com) ja kirjaudu admin tilin tunnistetiedoilla. 
    
2. Office 365-suojauksen &amp; Compliance Centeriin valitsemalla vasemmanpuoleisessa siirtymisruudussa **Threat management** **käytännön** \> **Anti-Malware**.
    
3. Kaksoisnapsauta oletuskäytäntö muokattava käytäntö koko yrityksen.
    
4. Valitse **asetukset**.
    
5. ** **Yleinen liitetiedostojen tyypit suodatin**Valitse.** Tämän ohjausobjektin alapuolelle ikkunan luetellaan tiedostotyypit, jotka on estetty.  Varmista, että lisäät nämä filetypes:
   - ADE, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, työ, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, YTA, shs, URL-osoite, vb, vbe, vbs, wsc, wsf, wsh, exe, pif  <br/> Voit lisätä tai poistaa tiedostotyyppejä myöhemmin tarvittaessa.
    
6. Valitse **Tallenna.**
    
Lisätietoja [haittaohjelmien suojelua](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Ransomware vastaan

Ransomware rajoittaa tietojen käyttö tiedostojen salausta tai lukita tietokoneen näytöllä. Sitten yrittää extort uhreja kuin rahaa pyytämällä ”ransom”, yleensä ovat cryptocurrencies Bitcoin, kuten tietojen vastaan. 
  
Voit suojautua ransomware luomalla yhden tai useamman sähköpostin työnkulkusäännöt estämään tiedostotunnisteet, joita yleisesti käytetään ransomware (nämä on lisätty vaiheessa [nostaa suojan haittaohjelmilta, sähköposti](#raise-the-level-of-protection-against-malware-in-mail) ) tai Varoita, käyttäjä vastaanottaa näitä sähköpostin liitteet.

Jotka edellisessä vaiheessa estänyt tiedostojen lisäksi on myös hyvä varoittaa käyttäjiä ennen kuin avaat Office liitetiedostot, jotka sisältävät makroja säännön luominen. Ransomware voi piilottaa sisällä makroja, joten olemme varoittaa käyttäjiä ei avaa näitä tiedostoja ihmisiltä he eivät tiedä.

Postin kuljetus säännön luominen:
  
1. Siirry hallintakeskukseen <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> ja valitse **Admin keskittää** \> **Exchange**.
    
2. **Postin kulku** -luokan Valitse **säännöt**.
    
3. Valitse **+**, ja valitse sitten **Luo uusi sääntö**.
    
4. Valitse **Lisäasetukset** -valintaikkunan alaosassa Nähdäksesi täydellisen luettelon vaihtoehdoista. 
    
5. Seuraavassa taulukossa on säännön asetukset koskevat. Jättää loput asetukset oletusarvo, ellet halua muuttaa asetuksia.
    
6. Valitse **Tallenna**.
    
|**Asetus**|**Varoita käyttäjiä, ennen kuin avaat liitetiedostoja Office-tiedostojen**||
|:-----|:-----|:-----|
|Nimi  <br/> |Anti-ransomware sääntö: Varoita käyttäjiä  <br/>  |
|Käytä tätä sääntöä, jos. . .  <br/> |Liitettä. . . tunniste vastaa. . .  <br/> |
|Määritä sanoja tai lauseita  <br/> |Lisää tiedostotyyppejä:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Tee seuraavat toimet. . .  <br/> |Sanoman vastaanottaja ilmoittaa  <br/> |
|Anna teksti  <br/> |Älä avaa nämä tiedostot tyypin ihmisiä et tiedä koska ne saattavat sisältää makrot ja haitallista koodia.  <br/> |
   
Lisätietoja on seuraavissa artikkeleissa:
  
- [Miten käsitellä ransomware](https://go.microsoft.com/fwlink/?linkid=2016501&amp;clcid=0x409)
    
- [Palauta yhteys OneDrive](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)
    


## <a name="stop-auto-forwarding-for-email"></a>Lopeta automaattinen edelleenlähetystä lähetettäväksi sähköpostitse

Luvattomilta käyttäjiltä, jotka muodostavat yhteyden käyttäjän postilaatikon voi varastaa postin asettamalla voit välittää automaattisesti sähköposti postilaatikko. Näin voi tapahtua myös ilman käyttäjän tietoisuutta. Voit estää tämän määrittämällä virtauksen sähköpostisääntö. 
  
Postin kuljetus säännön luominen, katsoa [Tämä lyhyt video](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) tai seuraavasti:
  
1. Valitse Microsoft 365-hallintakeskukseen **Admin keskittää** \> **Exchange**.
    
2. **Postin kulku** -luokan Valitse **säännöt**.
    
3. Valitse **+**, ja valitse sitten **Luo uusi sääntö**.
    
4. Valitse **Lisäasetukset** -valintaikkunan alaosassa Nähdäksesi täydellisen luettelon vaihtoehdoista. 
    
5. Käytä asetuksia seuraavassa taulukossa. Jättää loput asetukset oletusarvo, ellet halua muuttaa asetuksia.
    
6. Valitse **Tallenna**.
    
|**Asetus**|**Varoita käyttäjiä, ennen kuin avaat liitetiedostoja Office-tiedostojen**|
|:-----|:-----|
|Nimi  <br/> |Estää ulkoisten toimialueiden sähköpostin automaattinen edelleenlähetys  <br/> |
|Käytä tätä sääntöä, jos...  <br/> |Lähettäjä. . . on ulkoinen tai sisäinen. . . Organisaation sisällä  <br/> |
|Lisää ehto  <br/> |Viestin ominaisuudet. . . sisältää viestityyppi. . . Välitä automaattisesti  <br/> |
|Toimi seuraavasti...  <br/> |Estä viesti. . . Hylkää viesti ja Sisällytä selitys.  <br/> |
|Anna teksti  <br/> |Automaattisen edelleenlähetyksen sähköpostia organisaation ulkopuolelle on estetty suojaussyistä.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Sähköpostin suojaaminen tietojen kalastelu-viesteiltä

Jos olet määrittänyt yhden tai usean mukautetun toimialueen Office 365: ssä tai Microsoft 365-ympäristössä, voit määrittää kohdennettuja anti-phishing-suojaus. ATP anti-phishing-suojaus, Office 365: n Advanced Threat Protection-osa auttaa suojaamaan organisaatiosi haittaohjelmien impersonation-pohjainen phishing hyökkäyksiä ja muut phishing-hyökkäykset. Jos et ole määrittänyt mukautetun toimialueen, sinun ei tarvitse tehdä.
  
Suosittelemme, että aloitat tällä käyttöoikeudella luomalla suojata tärkeimmät käyttäjät ja mukautetun toimialueen käytäntöä. 

  
ATP-anti-phishing-käytännön luominen, katsella [tämän lyhyen videon koulutuksen](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)tai toimimalla seuraavasti:
  
1. Siirry osoitteeseen [https://protection.office.com](https://protection.office.com). 
    
2. Office 365-suojauksen &amp; Compliance Centeriin valitsemalla vasemmanpuoleisessa siirtymisruudussa **Threat management** **käytännön**.
    
3. Valitse **käytäntö** -sivulla **ATP anti-phishing**.
    
4. **Anti-phishing** -sivulla Valitse **+ Luo**. Ohjattu toiminto käynnistyy, joka opastaa sinut läpi anti-phishing-käytännön määrittäminen.
    
5. Määritä nimi, kuvaus ja asetukset kuten alla olevassa kaaviossa suositellaan käytännön. Saat tarkempia [Lisätietoja tietokalastelun ATP-käytäntöasetukset](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409) . 
    
6. Kun olet tarkistanut asetukset, valitse **Luo tämä käytäntö** tai **tallentaa**, tarpeen mukaan.
    

|**Asetus tai valinta**<br/>|**Suositeltavat asetukset** <br/>|
|:-----|:-----|
|Nimi  <br/> |Toimialue ja eniten hyötyä kampanjan henkilöstö  <br/> |
|Kuvaus  <br/> |Varmista tärkein henkilöstön ja omalta toimialueelta ei Persoonaton.  <br/> |
|Lisää suojaa käyttäjiä  <br/> |Valitse **+ Lisää edellyttäen, että vastaanottaja on**. Kirjoita käyttäjänimi tai sähköpostiosoite ehdokkaan kampanjan hallinta ja muita tärkeitä henkilökunnan jäsenet. Voit lisätä enintään 20 sisäiset ja ulkoiset osoitteet, jotka haluat suojata tekeytymistä.  <br/> |
|Lisää suojaa toimialueet  <br/> |Valitse **+ Lisää ehto vastaanottajan toimialueella**. Kirjoita mukautetun toimialueen Microsoft 365-tilaukseen liittyvää, jos jokin määritetty. Voit syöttää useampaan kuin yhteen toimialueeseen.  <br/> |
|Valitse Toiminnot  <br/> |Jos sähköposti lähetetään tekeytyneen käyttäjän: valita **toisen sähköpostiosoitteen viestin uudelleenohjaaminen**ja kirjoita sitten sähköpostiosoite security Administrator; esimerkiksi *Anneli<span><span>@contoso.com*.          Jos sähköposti lähetetään tekeytynyt toimialueen mukaan: Valitse **viestin karanteeniin**.  <br/> |
|Postilaatikon intelligence  <br/> |Postilaatikon intelligence on valittu oletusarvoisesti, kun luot uuden anti-phishing-käytännön. Jätä **Tämä asetus parhaan tuloksen** .  <br/> |
|Luotettujen lähettäjien ja toimialueiden lisääminen  <br/> |Voit lisätä oman toimialueen tai muista luotetuista toimialueista.  <br/> |
|Käytetty  <br/> |Valitse **vastaanottajan toimialue on**. **Valitse kohdassa **mainituista**.** Valitse **+ Lisää**. Esimerkiksi *contoso-toimialueen nimen vieressä oleva valintaruutu.<span> <span>com*, -luettelosta ja valitse sitten **Lisää**. Valitse **Valmis**.  <br/> |
   
Lisätietoja [Office 365: n ATP tietokalastelun käytäntöjä määritetty](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Suojaudu haittaohjelmien liitteet ja tiedostot, joiden ATP Turvalliset liitetiedostot

Ihmiset lähettää säännöllisesti, saada ja jakaa liitteitä, esimerkiksi asiakirjoja, esityksiä, laskentataulukoita ja paljon. Aina ei ole helppoa tietää, onko liite on turvallista tahallaan tai vain katsomalla sähköpostiviestin. Office 365: n Advanced Threat Protection sisältää ATP Liitetiedostojen turvallinen suojaus, mutta suojaus ei ole käytössä oletusarvoisesti. Suosittelemme, että luot uuden säännön alkavan avulla Suojaus. Tämä suoja ulottuu tiedostot SharePoint ja Microsoft Teams OneDrive.
  
Voit luoda käytännön ATP Turvalliset liitetiedostot, katsoa [Tämä lyhyt video](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)tai toimimalla seuraavasti:
  
1. Siirry [https://protection.office.com](https://protection.office.com) ja kirjaudu sisään admin tili. 
    
2. Office 365-suojauksen &amp; Compliance Centeriin valitsemalla vasemmanpuoleisessa siirtymisruudussa **Threat management** **käytännön**.
    
3. Valitse käytäntö-sivulla **ATP Turvalliset liitetiedostot**.
    
4. Turvalliset liitetiedostot-sivun käyttää laajalti **käyttöön SharePoint, OneDrive, ja Microsoftin työryhmät ATP** -valintaruutu. 
    
5. Valitse **+** voit luoda uuden käytännön. 
    
6. Käytä asetuksia seuraavassa taulukossa. 
    
7. Kun olet tarkistanut asetukset, valitse **Luo tämä käytäntö** tai **tallentaa**, tarpeen mukaan.
    

|**Asetus tai valinta**|**Suositeltavat asetukset** <br/>|
|:-----|:-----|
|Nimi  <br/> |Nykyiset ja tulevat sähköpostit havaitut haittaohjelmat ja estää.  <br/> |
|Kuvaus  <br/> |Estää nykyiset ja tulevat sähköpostiviestit ja liitteet, joiden havaitut haittaohjelmat.  <br/> |
|Tallenna liitteet Tuntematon malware response  <br/> |Valitse **Estä - Estä nykyiset ja tulevat sähköpostiviestit ja liitteet, joiden havaitut haittaohjelmat**.  <br/> |
|Ohjata liite tunnistus  <br/> |Ottaa uudelleenohjauksen käyttöön (Valitse tämä valintaruutu), kirjoita karanteenin valvoja-tili tai postilaatikon asetukset.          Käytä yllä olevaa valintaa malware skannaus liitteitä varten aikakatkaistaan tai virhe tapahtuu, jos (kun tämä on valittuna).  <br/> |
|Käytetty  <br/> |Vastaanottajan ryhmä on. . . Valitse toimialueesi.  <br/> |
   
Lisätietoja [Office 365: n ATP tietokalastelun käytäntöjä määritetty](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>ATP-turvallinen linkkejä phishing hyökkäyksiä vastaan

Hakkerit Piilota joskus pahantahtoinen Web-sivustoja linkit sähköposti tai muita tiedostoja. Office 365: n ATP turvallinen linkit (ATP turvallinen linkit), osana Office 365: n Advanced Threat Protection, suojata organisaation tarjoamalla web URL-osoitteita valitsemalla aika tarkastaminen Office-asiakirjoja ja sähköpostiviestejä. Suojaus määritetään ATP turvallinen linkit politiikkojen kautta.
  
Microsoft suosittelee, että toimit seuraavasti:
  
- Muokkaa oletuskäytäntö suojelun lisäämiseksi.
    
- Lisää uuden toimialueen kaikille vastaanottajille kohdistettu käytännön.
    
Määrittää Turvalliset ATP-linkkejä, katsella [tämän lyhyen videon koulutuksen](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)tai toimimalla seuraavasti:
  
1. Siirry [https://protection.office.com](https://protection.office.com) ja kirjaudu sisään admin tili. 
    
2. Office 365-suojauksen &amp; Compliance Centeriin valitsemalla vasemmanpuoleisessa siirtymisruudussa **Threat management** **käytännön**.
    
3. Käytäntö-sivulla voit valita **Turvallinen ATP-linkkejä**.
    
Voit muokata oletuskäytäntö seuraavasti:
  
1. Valitse **oletuskäytäntö** turvallinen linkit-sivun **käytännöt, jotka koskevat koko organisaatiota**. 
    
2. Valitse **asetukset, jotka koskevat paitsi sähköpostin sisältöä** **Office 365 ProPlus, iOS ja Android**.
    
3. Valitse **Tallenna**. 
    
Voit luoda uuden käytännön toimialueen kaikille vastaanottajille kohdistettu:
  
1. Valitse Turvalliset linkit-sivulla **käytännöt, jotka koskevat koko organisaatiota**, **+** voit luoda uuden käytännön. 
    
2. Käytä seuraavassa taulukossa lueteltuja asetuksia.
    
3. Valitse **Tallenna**. 

|**Asetus tai valinta**|**Suositeltavat asetukset** <br/>|
|:-----|:-----|
|Nimi  <br/> |Toimialueen kaikille vastaanottajille käytännön turvallinen linkit  <br/> |
|Valitse Tuntematon mahdollisesti haitallisen URL-osoitteet viestejä  <br/> |Valitse **-URL-osoitteet on kirjoitettava uudelleen ja verrataan tunnettujen haittaohjelmien linkkiluettelon käyttäjän napsauttaessa linkkiä**.  <br/> |
|Turvalliset liitetiedostot avulla voit tarkistaa ladattavan sisällön  <br/> |Valitse tämä valintaruutu.  <br/> |
|Käytetty  <br/> |Vastaanottajan ryhmä on. . . Valitse toimialueesi.  <br/> |
   
Lisätietoja [Office 365: n ATP turvallinen linkkejä](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Siirry hallintakeskukseen Intune

1. Kirjaudu [Azure](https://portal.azure.com/)portaaliin.

2. Valitse **kaikki palvelut** ja kirjoita **Hakuruutuun** *Intune* .

3. Kun näkyviin, napsauta Käynnistä-painiketta, seuraava **Microsoft Intune** , tehdä siitä suosikin ja helppo löytää myöhemmin.

Hallintakeskukseen Intune avulla voit rekisteröidä ja hallita organisaation laitteita. Lisätietoja [rekisteröinti-menetelmän avulla Windows-laitteiden ominaisuudet](https://docs.microsoft.com/intune/enrollment-method-capabs) ja [rekisteröinnin asetukset Intune hallituilla laitteilla](https://docs.microsoft.com/intune/enrollment-options).
