---
title: Microsoft 365 Businessin määrittäminen
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
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Opi määrittämään Microsoft 365 Business.
ms.openlocfilehash: e635b828609fc47cd8b92bb179a25bcc43cb0a1a
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660765"
---
# <a name="set-up-microsoft-365-business"></a>Microsoft 365 Businessin määrittäminen

Ennen kuin aloitat, lisätietoja [Saat Microsoft 365 Business](get-microsoft-365-business.md) ilmoittautuminen.

Katso [lyhyt video siitä, miten määritetään Microsoft 365 liiketoiminnan](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) määrittäminen ohjatun ja kun ei ole paikallisen Active Directoryn avulla
  

## <a name="overview"></a>Yleistä

Ohjattu asennus voidaan tehdä suurimman osan vaiheiden määrittäminen, mutta luetellaan myös muita vaihtoehtoja.

1. [Toimialueen lisääminen](#add-your-domain-to-personalize-sign-in) (Jos olet ostanut toimialueen aikana [rekisteröityä](sign-up.md), tässä vaiheessa on jo tehty.)
2. Voit lisätä käyttäjiä. Voit tehdä tämän jossakin seuraavista kolmesta tavasta:
    - [Ohjattu asennus](#add-users-in-the-wizard).
    - Käyttää hakemiston synkronointi [Azure AD-yhteyden avulla käyttäjät](#add-users-by-using-azure-ad-connect) lisätään paikalliseen Active Directoryyn.
    - Voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) admin Centerissä.
3. Käytännöt ja laitteiden määrittäminen. Voit tehdä tämän jossakin seuraavista kolmesta tavasta:
    - [Ohjattu asennus](#set-up-policies-in-the-wizard).  
    - [Hallintakeskukseen](#modify-or-add-policies-in-the-admin-center).
    - [Intune hallintakeskukseen](https://docs.microsoft.com/intune/what-is-device-management).
4. Määritä ja Hallitse Windows 10-laitteita.

    Kun liität laitteen WIndows 10 Azure AD, kaikki käytännöt tulla otetuiksi siihen.
    - Määritä [ohjatun asennuksen](#set-up-policies-in-the-wizard)Windows 10 laitteiden määrityksiä.
    - Liittää [Windows 10 uuden laitteen](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) Azure AD.
    - [Olemassa Windows 10-laitteen](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) liittäminen Azure AD.
1. Asenna Office 365: n liiketoiminnan.
    - Voit asentaa Officen Windows-laitteet automaattisesti [ohjatun asennustoiminnon](#set-up-policies-in-the-wizard)avulla.
    - Automaattisesti [asentaa Officen](auto-install-or-uninstall-office.md) hallintakeskukseen.
    - Antaa käyttäjien [asentaa Office-sovellukset](https://docs.microsoft.com/office365/admin/setup/install-applications) ja laitteet.
     
1. Lisätietoja suojauksen määrittäminen.
    - Ohjattu asennus Lisää politiikan suojaa laitteita, mutta voit myös hyödyntää [suojausta](#additional-security-settings) ominaisuuksia voi auttaa turvallinen tietojen ja tilien ja sähköpostit. 

## <a name="add-your-domain-users-and-set-up-policies"></a>Lisää toimialueen, käyttäjiä ja määrittämällä käytännöt

![Nauha, joka osoittaa https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Kun ostat Microsoft 365 Business, voit halutessasi toimialue omistat tai ostaa yksi aikana [ilmoittautuminen](sign-up.md).

- Jos olet ostanut uuden toimialueen Kun rekisteröidyit, toimialueesi on kaikki ylös ja voit siirtää [Lisää käyttäjät](#add-users-and-assign-licenses)ja määrittää käyttöoikeudet.

### <a name="add-your-domain-to-personalize-sign-in"></a>Voit mukauttaa sisään toimialueen lisääminen

1. Kirjautuminen [hallintakeskukseen Microsoft 365](https://admin.microsoft.com) yleisen järjestelmänvalvojan tunnuksilla. 

2. Valitse Käynnistä ohjattu **Lisää toimialueeseen** .

    ![Valitse Lisää toimialueeseen.](media/addadomainadmincenter.png)
    
3. Ohjatun toiminnon Kirjoita toimialuenimi, jota haluat käyttää (esimerkiksi contoso.com).


    ![Kuva Mukauta sivusi sisään.](media/personalizesignin.png)

    
4. Noudata ohjatun toiminnon [luoda DNS-tietueet on mahdollisesti DNS Office 365 videopalvelujen tarjoajan](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , joka tarkistaa, että omistat toimialueen. Jos tiedät toimialueen isäntä, katso myös [tarkemmat ohjeet isäntä](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Jos videopalvelujen tarjoajan on GoDaddy, on helppo prosessi ja sinua pyydetään automaattisesti kirjautua sisään ja anna Microsoft todentaa käyttäjän puolesta:

    ![GoDaddy Vahvista sivun Valitse Hyväksy.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Lisää käyttäjiä ja määritä käyttöoikeuksia

Ohjatussa toiminnossa voit lisätä käyttäjiä, mutta voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) admin Centerissä. Lisäksi jos paikalliseen toimialueen ohjauskoneeseen, voit lisätä käyttäjät, joilla on [Azure AD-muodosta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Ohjatun käyttäjien lisääminen

Lisättävien käyttäjien ohjatun toiminnon Hae automaattisesti määritetty Microsoft 365 Business käyttöoikeuden.
Jos paikallisen toimialueen ohjauskonetta ja Active Directoryn avulla on kohdassa [ddd Azure AD-yhteyden avulla käyttäjät](#add-users-by-using-azure-ad-connect).

![Lisää uusia käyttäjiä-sivun ohjatun toiminnon kuva](media/addnewuserspage.png)

1. Jos Microsoft 365 Business-tilauksessasi on aiemmin luotuja käyttäjiä (jos esimerkiksi olet käyttänyt Azure AD Connectia), näkyviin tulee vaihtoehto, jolla voit määrittää heille käyttöoikeudet. Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.

3. Kun käyttäjät on lisätty, näyttöön tulee vaihtoehto jakaminen on lisätty uusien käyttäjien tunnistetiedot. Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.

4. Ohita sähköpostiviestien siirtäminen valitsemalla **Siirrä sähköpostiviestejä** -sivulla **Seuraava**. 

    Jos siirrät toisen sähköpostin tarjoajalta ja haluat kopioida tiedot myöhemmin, voit [Siirtyminen sähköpostin ja yhteystietojen Office 365: ssä](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).

#### <a name="add-users-by-using-azure-ad-connect"></a>Lisää käyttäjät Azure AD-yhteyden avulla

 Jos paikallisen toimialueohjaimen Active Directory-hakemistopalvelun kanssa, voit synkronoida käyttäjien kanssa Microsoft 365 Business [Azure AD-yhteyden](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)avulla. Suorita tämä loppuun, ennen kuin käynnistät ohjatun asennuksen. Voit ladata sen admin Centerissä:

- Siirry **käyttäjät** \> **aktiivisia käyttäjiä**kolmea pistettä sivun yläosassa ja valitse sitten Lataa AD Azure Yhdistä **hakemiston synkronointi** .

    ![Aktiiviset käyttäjät-sivulla Valitse kolme pistettä > hakemiston snchronization.](media/setupdirsync.png)

    > [!IMPORTANT]
    > Jos luot käyttäjiä tällä tavalla, joudut silti liittää käyttöoikeudet niihin admin Centerissä.

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a>Jatkossakin käyttää toimialueeseen liittymistä apps ja laitteita

Jos haluat edelleen käyttää toimialueeseen liittymistä apps ja laitteita, lue seuraavista artikkeleista käyttöönoton, kahdella eri tavalla:
  
- [Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi](manage-windows-devices.md)
    - Tämä on suositeltava tapa.

- [Käyttää tiloissa Azure AD liitetty laite 365 Microsoft Business resurssit](access-resources.md)

### <a name="connect-your-domain"></a>Toimialueen yhdistäminen

> [!NOTE]
> Jos haluat käyttää toimialueen .onmicrosoft tai määrittää käyttäjille Azure AD-yhteyden avulla, et näe tässä vaiheessa.
  
Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.
  
1. Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa. Jos näin ei ole, [Muuta nameservers määrittäminen Office 365: ssä registrar mahdollisesti toimialueen kanssa](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Olemassa olevan DNS-tietueet, esimerkiksi web-sivuston, jos haluat hallita oman DNS-tietueet, varmista, että voit pysyä olemassa oleviin palveluihin. Katso lisätietoja [toimialueen perusteet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .

        ![Yhteyttä toimialueen-sivu, jossa voin hallita omaa DNS-tietueet.](media/connectyourdomainpage.png)

2. Noudata ohjatun toiminnon ohjeita ja sähköpostin ja muita palveluita määritetään puolestasi.

### <a name="set-up-security-policies-and-device-configurations"></a>Käytännöt ja laitteiston määritysten määrittäminen 

Näitä käytäntöjä sovelletaan käyttäjien annat käyttöoikeuden, tai käyttäjäryhmä, jos päätät määrittää eri käytäntöjä joukolle käyttäjiä.

#### <a name="set-up-policies-in-the-wizard"></a>Määritä ohjatun toiminnon käytännöt

Ohjattu toiminto määrittää käytäntöjä käytetään automaattisesti *Kaikki*käyttäjät [suojausryhmään](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) .

1. **Mobiililaitteiden työn tiedostojen suojaaminen** vaihtoehto **Suojaa Työtiedostojen kun laitteita katoaa tai varastetaan** on oletusarvon mukaan valittuna. Voit valita, **miten käyttäjät voivat käyttää mobiililaitteiden Office-tiedostojen hallinta**käyttöön ja tämä on suositeltavaa.

    ![Kuva on suojata Työtiedostojen matkaviestimet-sivulla.](media/protectworkfilesondevices.png)

     - Jos laajennat **Suojaa Työtiedostojen kun laitteita katoaa tai varastetaan**, [oletusarvot](protect-work-files-on-lost-or-stolen-device.md) ovat ennalta valitut:

        ![Kuva laitteet menettää tiedostojen suojaaminen oletusarvot.](media/protectworkfilesondevicesdefault.png)

    - Valitse, **miten käyttäjät voivat käyttää mobiililaitteiden Office-tiedostojen hallinta** ja laajentaa sitä, jos [oletusarvot](manage-user-access-on-mobile-devices.md) näkyvät. On suositeltavaa hyväksyä oletusarvot asennuksen aikana kaikkia käyttäjiä koskevien sovelluskäytäntöjen luomiseksi Androidille, iOS:lle ja Windows 10:lle. Voit luoda lisää käytäntöjä asennuksen päätyttyä.

        ![Kuva-mobile Office-tiedostojen asetukset.](media/useraccessonmobile.png)

2. Viimeinen vaihe Valitse suojaa tiedot ja laitteet mahdollistaa käytäntöjen määrittäminen Windows 10-laitteiden suojaamiseen. Näitä asetuksia käytetään automaattisesti käyttäjän Windows-10 muodostaa yhteyden organisaatiossasi. Voit laajentaa **suojattua Windows-10 laitteet** ja muokkaa [oletusarvoja](secure-windows-10-devices.md).
3. Voit myös [asentaa automaattisesti Officen](install-office-on-windows-10-during-setup.md) Windows 10-laitteissa.

    ![Kuva Aseta laitteen Windows 10-määrityssivulla.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a>Muokkaa tai Lisää käytännöt-hallintakeskukseen

Katso [Microsoft 365 liiketoiminnan hallinnassa](manage.md) on linkkejä ohjeaiheisiin siitä, kuinka voit tarkastella ja muokata laitteiden ja sovellusten suojaus-käytäntöjä, ja tietojen poistamisesta tai Palauta käyttäjän laitteita.

## <a name="deploy-and-manage-windows-10"></a>Käyttöönotto ja hallinta Windows-10
Lisätietoja Azure AD, joko uusia tietokoneita tai vaihtamalla kirjautuminen profiilin käytössä asennuksen aikana muodostettava [määrittäminen Microsoft 365 yrityskäyttäjille Windows-laitteet](set-up-windows-devices.md) . 

### <a name="use-autopilot-to-set-up-new-devices"></a>Automaattiohjauksen avulla voit määrittää uusia laitteita

[Windows automaattiohjauksen](add-autopilot-devices-and-profile.md) avulla voit määrittää käyttäjän **Uusi** Windows 10-laitteet automaattisesti ennalta, mutta voi olla helpompi saada [kumppani](https://www.microsoft.com/solution-providers/search) , jolla voit tehdä tämän sinulle. Voit myös siirtyä [Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) ja pyytää asiantuntija pilvi tekniikka määrittää, ostaa uusia laitteita.

### <a name="access-on-premises-resources"></a>Käyttää tiloissa resursseja

Jos organisaatiossa käytetään Windows Server Active Directory tiloissa, voit määrittää Microsoft 365 liiketoiminnan suojaamaan Windows 10-laitteet, säilyttäen kuitenkin edellyttää paikallista todennusta tiloissa resurssien käytön. Voit määrittää [toimialueeseen liittymistä Windows 10 laitteita voi hallita Microsoft 365 Business käyttöön](manage-windows-devices.md) noudattamalla. Tämä on ensisijainen menetelmä, ja tässä tilassa laitteita kutsutaan hybridi Azure AD liitetyt laitteet.

Jos yrityksesi on paikallista Active Directory, joka sisältää joitakin tiloissa (kuten jaettujen tiedostoresurssien ja tulostinten), voit antaa Azure AD liittynyt laitteiden käyttöä noudattamalla tässä nämä resurssit: [käyttö paikalliset resurssit Microsoft 365 Business AD liitetty laite Azure](access-resources.md).

## <a name="deploy-office-365-client-apps"></a>Ottaa käyttöön Office 365-asiakassovellukset

Jos päätit asentaa Office-sovellukset automaattisesti joukon aikana ylös, apps asennetaan Windows 10-laitteet, kun käyttäjiä on kirjautuneena Azure AD laitteiden kanssa työtä tunnistetietonsa Windows.
Jos haluat asentaa Office mobile iOS tai Android-laitteet, kohdassa [Mobiililaitteiden käyttäjille Microsoft 365 Business määrittäminen](set-up-mobile-devices.md).

Voit asentaa Officen myös erikseen. Katso ohjeet [asentaa PC-tai Mac Office](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) .

## <a name="additional-security-settings"></a>Muita tietoturva-asetuksia

Suojaus ja yhteensopivuus-asetus ohjatun asennuksen lisäksi voit määrittää myös seuraavia lisäasetuksia:
  
- **Sähköposti Suojaus haittaohjelmilta**
- **Kehittyneen uhkien suojaa (ATP) Turvalliset liitetiedostot**
- **ATP-Safe-linkit**
- **PIHARAKENNUS anti-phishing**
- **Exchange Online Archiving**
- **Tietojen menetyksen estäminen (DLP)**
- **Azure-tietojen suojaaminen** (1 aio)
- **Portaalin käytettävyyttä Intune**

Aloita ks- [käytäntöjen suojauksen lisäasetusten määrittäminen](set-up-advanced-security.md).

Katso myös suojauksen parhaiden käytäntöjen opas [top 10 tapoja suojata yrityksen Microsoft 365](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) .