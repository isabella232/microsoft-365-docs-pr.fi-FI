---
title: Microsoft 365 Businessin määrittäminen ohjatun määritystoiminnon avulla
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Opi neljä vaihetta täyttämällä 365 Microsoft Business määrittäminen.
ms.openlocfilehash: f57239b884bd2e186c0bc01973130a10fa4cfe84
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982193"
---
# <a name="set-up-microsoft-365-business-by-using-the-setup-wizard"></a>Microsoft 365 Businessin määrittäminen ohjatun määritystoiminnon avulla

Suorita vaiheet 1-4 alla.
  
### <a name="set-up-microsoft-365-business"></a>Microsoft 365 Businessin määrittäminen

Katso video siitä, miten määritetään Microsoft 365 liiketoiminnan, jos sinulla ei ole paikallisen Active Directory:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/0705c337-f3e8-4d28-bb6c-530cd28e99f2?autoplay=false]
  
Asetusten määrittämisen vaiheet ovat asetukset, jotka sisältävät paikallisen Active Directoryn tietoja. Jos haluat edelleen käyttää toimialueeseen liittymistä laitteita, lue seuraavista artikkeleista kahdella eri tavalla, käyttöönoton ja kaikki vaiheet on suoritettu, ennen kuin suoritat ohjatun asennuksen:
  
- [Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi](manage-windows-devices.md)
    
    -Tämä on suositeltava tapa.
    
- [Käyttää tiloissa Azure AD liitetty laite 365 Microsoft Business resurssit](access-resources.md)
    
### <a name="step-1-personalize-sign-in"></a>Vaihe 1: Kirjaudu sisään mukauttaminen

1. Kirjaudu sisään [Microsoft 365 Businessiin](https://portal.microsoft.com) käyttämällä yleisen järjestelmänvalvojan tunnistetietojasi. Siirry hallintakeskukseen valitsemalla **Järjestelmänvalvoja**-ruutu. 
    
2. Käynnistä ohjattu toiminto valitsemalla hallintakeskuksessa **Aloita määritys** (tilasi mukaan näkyvissä oleva vaihtoehto voi olla **Jatka määritystä**). 
    
3. Kirjoita toimialuenimi, jota haluat käyttää (kuten contoso.com).
    
    Periksi ja kirjoita toimialueesi vaikka olet varmistanut käytettäessä esimerkiksi Azure AD-muodosta. Seuraavat kaksi vaihetta ei sovelleta, jos olet käyttänyt AD Azure Yhdistä tarkistamaan toimialueesi.
    
4. Noudata ohjatun toiminnon [luoda DNS-tietueet on mahdollisesti DNS Office 365 videopalvelujen tarjoajan](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) , joka tarkistaa, että omistat toimialueen. 
    
    Voit tarkastella esimerkiksi video [Video: uusi Admin Centerissä asennusohjelma Office 365](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8). Huomaa, että tämä video ei sisällä 365 Microsoft Business data protection vaiheet.
    
    ![Screenshot of the Business Cloud Suite setup wizard.](media/3c4fd40c-2de1-4a87-8ee0-78d3928c7bb7.png)
  
### <a name="step-2-add-users-and-assign-licenses"></a>Vaihe 2: Lisää käyttäjiä ja määrittää käyttöoikeuksia

1. Voit lisätä käyttäjiä tässä, tai voit [lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallintakeskuksessa. 
    
    Lisättäville käyttäjille määritetään automaattisesti Microsoft 365 Business-käyttöoikeus.
    
2. Jos Microsoft 365 Business-tilauksessasi on aiemmin luotuja käyttäjiä (jos esimerkiksi olet käyttänyt Azure AD Connectia), näkyviin tulee vaihtoehto, jolla voit määrittää heille käyttöoikeudet. Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.
    
3. Näkyviin tulee myös vaihtoehto, jolla voit jakaa tunnistetiedot lisäämiesi uusien käyttäjien kanssa. Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.
    
4. Ohita sähköpostiviestien siirtäminen valitsemalla **Siirrä sähköpostiviestejä** -sivulla **Seuraava**. 
    
    Jos siirrät toisen sähköpostin tarjoajalta ja haluat kopioida tiedot myöhemmin, voit [Siirtyminen sähköpostin ja yhteystietojen Office 365: ssä](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).
    
    ![Screenshot of two new users added in the setup wizard](media/8f729967-5c65-4ceb-b737-18119db40564.png)
  
### <a name="step-3-connect-your-domain"></a>Vaihe 3: Yhdistä toimialueeseen

> [!NOTE]
> Jos haluat käyttää toimialueen .onmicrosoft tai käyttää AD-Yhdistä Azure, et näe tässä vaiheessa. 
  
Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.
  
1. Ohjattu asennustoiminto havaitsee että registrar yleensä ja antaa linkin haluat vaiheittaiset ohjeet päivitetään NS-tietueet registrar-Web-sivustosta. Jos näin ei ole, [Muuta nameservers määrittäminen Office 365: ssä registrar mahdollisesti toimialueen kanssa](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).
    
2. Sähköposti ja muut palvelut määritetään automaattisesti puolestasi
    
### <a name="step-4-manage-devices-and-work-files"></a>Vaihe 4: Hallitse laitteita ja käyttää tiedostoja

1. Sivun asettaa **Suojaa Työtiedostojen kannettavissa laitteissa** sekä **Suojaa Työtiedostojen kun laitteita katoaa tai varastetaan** ja **hallita sitä, miten käyttäjät voivat käyttää mobiililaitteiden Office-tiedostojen** asetukset **käyttöön**. Voit myös käyttää kunkin osa asetuksen napsauttamalla kunkin asetuksen vieressä olevan nuolen.
  
  Kaikki käyttöoikeudet käyttäjien työtä tiedostot on nyt suojattu iOS ja Android-laitteet, niin pian kuin he [asentaa Office apps](set-up-mobile-devices.md) (ja todentaa käyttöoikeutensa Microsoft 365 Business kanssa). 
  
  ![Screenshot of protect work files on your mobile devices page](media/3139a9aa-6228-4e74-8166-c6a886d7319f.PNG)
  
2. **Laitteen kokoonpanotietoja määrittämällä Windows 10** -sivulla Määritä **Suojatun Windows 10-laitteiden** **käytössä**.
  
   Voit myös käyttää kunkin osa asetusta napsauttamalla sen vieressä olevaa merkkiä.
  
3. Määritä **Windows 10 laitteet asentaa Office** **Kyllä** jos kaikilla käyttäjillä on Windows (10) tietokonetta, ja joko ei ole olemassa Office asentaa tai pika-asennus Office asennetaan. Jos näin ei ole, Määritä tämän asetuksen arvoksi **ei**. Voit [asentaa automaattisesti Office](auto-install-or-uninstall-office.md) -hallintakeskukseen, kun olet valmistellut käyttäjien tietokoneissa. Lisätietoja on kohdassa [Office-asiakasohjelman asennuksen valmisteleminen](prepare-for-office-client-deployment.md).
  
    Työtiedostojen lisensoidut käyttäjät Windows 10-laitteiden suunniteltu niin pian kuin ne [liittyä Windows 10-laitteisiinsa](set-up-windows-devices.md) Microsoft 365 Business Azure AD-toimialueen tai [asentaa Windowsin uuteen tietokoneeseen 10](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) , kun samanaikaisesti liittyä Microsoft-365 Business Azure AD-toimialueesta. 
  
4. Valitse **Seuraava** ja olet valmis asennuksen kanssa. 
  
    Jätä meille palautetta voit auttaa meitä parantamaan kokemusta tässä vaiheessa.
  
    ![Screenshot of Prepare Windows 10 devices page](media/bff701c1-48a3-44f4-aa95-9d959d57c85b.PNG)
  
## <a name="additional-security-settings"></a>Muita tietoturva-asetuksia

Suojaus ja yhteensopivuus-asetus ohjatun asennuksen lisäksi voit määrittää myös seuraavia lisäasetuksia:
  
- Määritä liitteiden vastaan. **Advanced Threat Protection** (ATP) tunnistaa haitallista sisältöä, ja estää epäluotettavien liitetiedostojen toimittamisen suojaaminen tietojen kalastelussa ja ransomware tartuntoja vastaan. Liitetiedostojen suojaus aktivoimaan Katso [määrittäminen Office 365: n ATP Turvalliset liitetiedostot käytäntöjä](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).
    
- Suojaa ympäristön, kun käyttäjät napsauttavat haitallisia linkkejä. ATP tarkistaa linkkejä sähköpostitse, kun käyttäjä napsauttaa niitä. Jos linkkiä ei ole turvallinen, käyttäjä saa varoituksen ei päästä sivustoon tai ilmoittanut, että sivusto on estetty. Tämä auttaa suojautumaan tietojen kalastelussa. [Määrittäminen Office 365: n ATP turvallinen linkit käytännöt](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) tai [määrittäminen Office 365: n ATP turvallinen linkit käytäntöjä](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).
    
- Voit säilyttää kaikki postilaatikon sisältö, mukaan lukien poistetut sijoittamalla käyttäjän koko Postilaatikko- **Pidä oikeudenkäyntiä**. Lisätietoja on kohdassa 
- [Määritä sähköposti pidätyksen kanssa Exchange Online arkistoida](security-features.md#set-up-email-retention-with-exchange-online-archiving).
    
- Määritä mukautetut **säilytyskäytännöt**, esimerkiksi tietyn ajanjakson aikana säilyttää tai poistaa sisällön pysyvästi säilytysajan päätyttyä. Voit ottaa käyttöön mukautetut säilytyskäytännöt arvopapereihin ja compliance Centeriin, siirry **Data hallinnon** \> **pidätys**ja noudata sitten ohjatun toiminnon ohjeita. Lisätietoja on kohdassa [Yleiskatsaus säilytyskäytäntöjä](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).
    
## <a name="next-steps"></a>Seuraavat vaiheet

Käyttöoikeudet omaavilla käyttäjillä seuraava vaihe on laitteiden määrittäminen.<br/> Tutustu [Windows-laitteiden määrittäminen Microsoft 365 Business -käyttäjille](set-up-windows-devices.md) ja [Mobiililaitteiden määrittäminen Microsoft 365 Business -käyttäjille](set-up-mobile-devices.md). <br/>Kohdassa [Microsoft 365 Businessin hallinta](manage.md) on linkit aiheisiin, joissa on ohjeet laitteiden ja sovellusten suojauskäytäntöjen määrittämiseen ja tietojen poistamiseen käyttäjien laitteista. 
  


