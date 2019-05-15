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
ms.openlocfilehash: f3a9ad62f5ec8779296e800b9ecc8d6181d7aff7
ms.sourcegitcommit: f420a5cdedf3ec2babc6d8ad7e7c79da0b08e115
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/13/2019
ms.locfileid: "33966974"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Määritä ohjatussa asennustoiminnossa 365 Microsoft Business

## <a name="add-your-domain-users-and-set-up-policies"></a>Lisää toimialueen käyttäjille ja käytäntöjen määrittäminen

![Nauha, joka osoittaa https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Kun ostat Microsoft 365 Business, voit halutessasi toimialue omistat tai ostaa yksi aikana [ilmoittautuminen](sign-up.md).

- Jos olet ostanut uuden toimialueen Kun rekisteröidyit, toimialueesi on kaikki ylös ja voit siirtää [Lisää käyttäjät](#add-users-and-assign-licenses)ja määrittää käyttöoikeudet.

### <a name="add-your-domain-to-personalize-sign-in"></a>Voit mukauttaa sisään toimialueen lisääminen

1. Kirjautuminen [hallintakeskukseen Microsoft 365](https://admin.microsoft.com) yleisen järjestelmänvalvojan tunnuksilla. 

2. Valitse **Lisää toimialueeseen** **Lisää käyttäjiä** tai Käynnistä ohjattu toiminto.
    > [!IMPORTANT]
    > Jos olet ostanut toimialueen rekisteröitymisen yhteydessä, se ei katso **Lisää toimialue** vaiheen tähän. Siirry [Lisää käyttäjiä](#add-users-and-assign-licenses) sen sijaan.

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

![Lisää uusia käyttäjiä-sivun ohjatun toiminnon kuva](media/addnewuserspage.png)

1. Jos Microsoft 365 Business-tilauksesi on olemassa käyttäjiä (esimerkiksi jos olet käyttänyt AD-Yhdistä Azure), voit määrittää käyttöoikeudet niihin nyt saat. Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.

3. Kun käyttäjät on lisätty, näyttöön tulee vaihtoehto jakaminen on lisätty uusien käyttäjien tunnistetiedot. Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.

4. Ohita sähköpostiviestien siirtäminen valitsemalla **Siirrä sähköpostiviestejä** -sivulla **Seuraava**. 

    Jos siirrät toisen sähköpostin tarjoajalta ja haluat kopioida tiedot myöhemmin, voit [Siirtyminen sähköpostin ja yhteystietojen Office 365: ssä](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).


### <a name="connect-your-domain"></a>Toimialueen yhdistäminen

> [!NOTE]
> Jos haluat käyttää toimialueen .onmicrosoft tai määrittää käyttäjille Azure AD-yhteyden avulla, et näe tässä vaiheessa.
  
Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.
  
1. Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa. Jos näin ei ole, [Muuta nameservers määrittäminen Office 365: ssä registrar mahdollisesti toimialueen kanssa](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Olemassa olevan DNS-tietueet, esimerkiksi web-sivuston, jos haluat hallita oman DNS-tietueet, varmista, että voit pysyä olemassa oleviin palveluihin. Katso lisätietoja [toimialueen perusteet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .

        ![Yhteyttä toimialueen-sivu, jossa voin hallita omaa DNS-tietueet.](media/connectyourdomainpage.png)

2. Noudata ohjatun toiminnon ohjeita ja sähköpostin ja muita palveluita määritetään puolestasi.

### <a name="set-up-security-policies-and-device-configurations"></a>Käytännöt ja laitteiston määritysten määrittäminen 

Ohjattu toiminto määrittää käytäntöjä käytetään automaattisesti *Kaikki*käyttäjät [suojausryhmään](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) . Voit myös luoda uusia ryhmiä määrittelemään hallintakeskukseen käytäntöjä.

1. **Mobiililaitteiden työn tiedostojen suojaaminen** vaihtoehto **Suojaa Työtiedostojen kun laitteita katoaa tai varastetaan** on oletusarvon mukaan valittuna. Voit valita, **miten käyttäjät voivat käyttää mobiililaitteiden Office-tiedostojen hallinta**käyttöön ja tämä on suositeltavaa.

    ![Kuva on suojata Työtiedostojen matkaviestimet-sivulla.](media/protectworkfilesondevices.png)

     - Laajenna **Suojaa Työtiedostojen kun laitteita katoaa tai varastetaan** [oletusarvot](protect-work-files-on-lost-or-stolen-device.md):

        ![Kuva laitteet menettää tiedostojen suojaaminen oletusarvot.](media/protectworkfilesondevicesdefault.png)

    - **Miten käyttäjät voivat käyttää mobiililaitteiden Office-tiedostojen hallinta** Valitse ja laajenna se näyttää [oletusarvot](manage-user-access-on-mobile-devices.md). Suosittelemme, että hyväksyt Sovelluskäytännöt Luo Android, iOS ja Windows 10-asennuksen aikana oletusarvot, jotka koskevat kaikkia käyttäjiä. Voit luoda lisää käytäntöjä asennuksen päätyttyä.

        ![Kuva-mobile Office-tiedostojen asetukset.](media/useraccessonmobile.png)

2. Viimeinen vaihe Valitse suojaa tiedot ja laitteet mahdollistaa käytäntöjen määrittäminen Windows 10-laitteiden suojaamiseen. Näitä asetuksia käytetään automaattisesti käyttäjän Windows-10 muodostaa yhteyden organisaatiossasi. Voit laajentaa **suojattua Windows-10 laitteet** ja muokkaa [oletusarvoja](secure-windows-10-devices.md).
3. Voit myös [asentaa automaattisesti Officen](install-office-on-windows-10-during-setup.md) Windows 10-laitteissa.

    ![Kuva Aseta laitteen Windows 10-määrityssivulla.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a>Ottaa käyttöön Office 365-asiakassovellukset

Jos päätit asentaa Office-sovellukset automaattisesti joukon aikana ylös, apps asennetaan Windows 10-laitteet, kun käyttäjiä on kirjautuneena Azure AD laitteiden kanssa työtä tunnistetietonsa Windows.
Jos haluat asentaa Office mobile iOS tai Android-laitteet, kohdassa [Mobiililaitteiden käyttäjille Microsoft 365 Business määrittäminen](set-up-mobile-devices.md).

Voit asentaa Officen myös erikseen. Katso ohjeet [asentaa PC-tai Mac Office](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) .
