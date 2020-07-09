---
title: Microsoft 365 Business Premiumin määrittäminen
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Tutustu Microsoft 365 Business Premiumin asennusvaiheisiin, kuten toimialueen ja käyttäjien lisäämiseen, suojauskäytäntöjen määrittämiseen ja muihin.
ms.openlocfilehash: efa7934ece0dfeac3c4b20daa37da6f1160901e7
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081844"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Microsoft 365 Business Premiumin määrittäminen ohjatussa asennustoiminnossa

Tämä video on kohdassa Microsoft 365 Business Premiumin asennuksen yleiskatsaus.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

## <a name="add-your-domain-users-and-set-up-policies"></a>Toimialueen, käyttäjien ja käytäntöjen määrittäminen

Kun ostat Microsoft 365 Business Premiumin, voit käyttää omistamaasi toimialuetta tai ostaa sellaisen [rekisteröitymisen](sign-up.md)aikana.

- Jos ostit uuden toimialueen rekisteröitymisen yhteydessä, toimialueesi on määritetty ja voit siirtyä [Lisää käyttäjiä -kohtaan ja määrittää käyttöoikeuksia](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Toimialueen lisääminen kirjautumisen mukauttamiseksi

1. Kirjaudu [Microsoft 365 -hallintakeskukseen](https://admin.microsoft.com) yleisten järjestelmänvalvojan tunnistetietojen avulla. 

2. Käynnistä ohjattu toiminto valitsemalla **Siirry asennukseen.**

    ![Valitse Siirry asennukseen.](../media/gotosetupinadmincenter.png)

3. Asenna **Office-sovellukset -sivulla** voit halutessasi asentaa sovellukset omaan tietokoneeseesi.
    
4. Kirjoita **Lisää toimialue** -vaiheeseen toimialuenimi, jota haluat käyttää (kuten contoso.com).

    > [!IMPORTANT]
    > Jos ostit toimialueen rekisteröitymisen aikana, et näe **lisää toimialuevaihetta** tässä. Siirry sen sijaan [Kohtaan Lisää käyttäjiä.](#add-users-and-assign-licenses)

    ![Näyttökuva Mukauta kirjautumissivuasi.](../media/adddomain.png)

    
4. [Luo DNS-tietueet missä tahansa Microsoft 365:n DNS-isännöintipalvelussa](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) ohjatun toiminnon ohjeiden mukaisesti, jotka tarkistavat toimialueen omistavan dns-isännöintipalvelun. Jos tunnet toimialueen isännän, katso myös [isäntäkohtaiset ohjeet](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Jos isännöintipalvelusi on GoDaddy tai toinen [isäntä,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)joka on käytössä toimialueen yhdistämisessä, prosessi on helppo ja sinua pyydetään automaattisesti kirjautumaan sisään ja antamaan Microsoftin todentaa puolestasi.

    ![Valitse GoDaddy Confirm Access (Vahvista käyttö) -sivulla Valtuuta.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Lisää käyttäjiä ja määritä käyttöoikeuksia

Voit lisätä käyttäjiä ohjattuun toimintoon, mutta voit [myös lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallintakeskuksessa. Jos sinulla on paikallinen toimialueen ohjauskone, voit lisätä käyttäjiä [Azure AD Connectin](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)avulla.

#### <a name="add-users-in-the-wizard"></a>Käyttäjien lisääminen ohjattuun toimintoon

Kaikille ohjatussa toiminnossa lisättäjille määritetään automaattisesti Microsoft 365 Business Premium -käyttöoikeus.

![Näyttökuva ohjatun toiminnon Lisää uusia käyttäjiä -sivusta](../media/addnewuserspage.png)

1. Jos Microsoft 365 Business Premium -tilauksessasi on olemassa olevia käyttäjiä (esimerkiksi jos käytit Azure AD Connectia), voit määrittää heille käyttöoikeuksia nyt. Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.

2. Kun olet lisännyt käyttäjät, voit myös jakaa tunnistetiedot lisäämiesi uusien käyttäjien kanssa. Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.

### <a name="connect-your-domain"></a>Toimialueen yhdistäminen

> [!NOTE]
> Jos valitsit .onmicrosoft-toimialueen käyttämisen tai käytät Azure AD Connectia käyttäjien määrittämiseen, et näe tätä vaihetta.
  
Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.
  
1. Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa. Jos näin ei ole, [Muuta nimipalvelimia, jos haluat määrittää Microsoft 365:n minkä tahansa toimialueen rekisteröintipalvelun kanssa.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar) 

    - Jos sinulla on aiemmin luotuja DNS-tietueita, esimerkiksi aiemmin luotu web-sivusto, mutta DNS-isäntäsi on käytössä [toimialueen yhdistämistä](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)varten, valitse **Lisää tietueita minulle**. Hyväksy **Valitse online-palvelut -sivulla** kaikki oletukset ja valitse **Seuraava**ja valitse DNS-isännän sivulla **Valtuuta.**
    - Jos sinulla on dns-tietueita muiden DNS-isäntien kanssa (ei käytössä toimialueen yhdistämistä varten), sinun kannattaa hallita omia DNS-tietueita varmistaaksesi, että nykyiset palvelut pysyvät yhteydessä toisiinsa. Lisätietoja [on toimialueen perustiedoissa.](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics)

        ![Aktivoi tietuesivu.](../media/activaterecords.png)

2. Noudata ohjatun toiminnon ohjeita, niin sinulle määritetään sähköposti ja muut palvelut.

### <a name="protect-your-organization"></a>Organisaation suojaaminen 

Ohjatussa toiminnossa määritettyjä käytäntöjä käytetään automaattisesti [suojausryhmässä,](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) jonka nimi on *Kaikki käyttäjät*. Voit myös luoda lisää ryhmiä, joihin käytännöt määritetään hallintakeskuksessa.

1. On **Lisää suojausta kehittyneiltä kyberuhkilta**-kohdassa on suositeltavaa hyväksyä oletusarvot, joiden mukaan [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) voi skannata Office-sovellusten tiedostoja ja linkkejä.

    ![Näyttökuva Lisää suojausta -sivusta.](../media/increasetreatprotection.png)


2. Hyväksy **Suojaa arkaluonteisten tietojen vuodot** -sivulla office 365:n tietojen menetyksen estämisen (DLP) oletusasetukset, jotta voit seurata arkaluonteisia tietoja Office-sovelluksissa ja estää niiden tahattoman jakamisen organisaation ulkopuolella.

3. Jätä Mobiilisovellusten hallinta **Officen tietojen suojaaminen -sivulla,** laajenna asetukset ja tarkista ne ja valitse sitten **Luo mobiilisovellusten hallintakäytäntö**.

    ![Näyttökuva Suojaa tiedot Office mobiililaitteille -sivulla.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Windows 10 -tietokoneiden suojaaminen

Valitse vasemmassa siirtymisruudussa **Asennus** ja valitse sitten **Kirjautumis- ja suojaus -kohdasta** **Suojaa Windows 10 -tietokoneet**. Aloita valitsemalla **Näytä.** Katso täydelliset ohjeet [Windows 10 -tietokoneiden suojaamisesta.](secure-win-10-pcs.md)

## <a name="deploy-office-365-client-apps"></a>Office 365 -asiakassovellusten käyttöönotto

Jos valitsit Office-sovellusten automaattisen asentamisen asennuksen aikana, sovellukset asennetaan Windows 10 -laitteisiin, kun käyttäjät ovat kirjautuneet Azure AD:hen Windows-laitteistaan työtunnistetietojensa avulla.

Lisätietoja Officen asentamisesta iOS- tai Android-mobiililaitteisiin on ohjeaiheessa [Mobiililaitteiden määrittäminen Microsoft 365 Business Premium -käyttäjille](set-up-mobile-devices.md).

Voit asentaa Officen myös yksitellen. Katso ohjeet [kohdasta Officen asentaminen PC- tai Mac-tietokoneeseen.](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658)

## <a name="see-also"></a>Tutustu myös seuraaviin ohjeaiheisiin

[Microsoft 365 yritysten koulutus videoita](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
