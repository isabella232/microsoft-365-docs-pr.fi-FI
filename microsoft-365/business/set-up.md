---
title: Microsoft 365 Businessin määrittäminen
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Lue tietoja Microsoft 365 Businessin määrittämisestä.
ms.openlocfilehash: a41d03c4f9e250cf3b16d11bf23897e31adaf866
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2020
ms.locfileid: "42090844"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Microsoft 365 Businessin määrittäminen ohjatussa asennustoiminnossa

Tämä video on yleiskuvaus Microsoft 365 Businessin asennuksesta.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

## <a name="add-your-domain-users-and-set-up-policies"></a>Toimialueen, käyttäjien ja käytäntöjen määrittäminen

[![Selite, jossa ilmoitetaan, että hallintakeskus muuttuu. Lisätietoja löytyy osoitteesta aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Kun ostat Microsoft 365 Businessin, voit käyttää omistamaasi toimialuetta tai ostaa sen [rekisteröitymisen](sign-up.md)aikana.

- Jos ostit uuden toimialueen rekisteröityessäsi, toimialueesi on määritetty ja voit siirtyä [Lisää käyttäjiä -kohtaan ja määrittää käyttöoikeuksia](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Toimialueen lisääminen kirjautumisen mukauttamiseksi

1. Kirjaudu [Microsoft 365 -hallintakeskukseen](https://admin.microsoft.com) käyttämällä yleisiä järjestelmänvalvojan tunnistetietoja. 

2. Käynnistä ohjattu toiminto valitsemalla **Siirry asennukseen.**

    ![Valitse Siirry asennukseen.](../media/gotosetupinadmincenter.png)

3. Asenna **Office-sovellukset -sivulla** voit halutessasi asentaa sovellukset omaan tietokoneeseesi.
    
4. Kirjoita **Lisää toimialue** -vaiheeseen haluamasi toimialueen nimi (kuten contoso.com).

    > [!IMPORTANT]
    > Jos ostit toimialueen rekisteröitymisen aikana, lisää **toimialuevaihe** ei näy tässä. Siirry sen sijaan [kohtaan Käyttäjien lisääminen.](#add-users-and-assign-licenses)

    ![Näyttökuva Mukauta kirjautumista -sivusta.](../media/adddomain.png)

    
4. Luo [DNS-tietueita missä tahansa Office 365:n DNS-isännöintipalvelussa](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) ohjatun toiminnon ohjeiden mukaisesti, mikä tarkistaa toimialueen omistavan. Jos tunnet verkkotunnuksen isännän, katso myös [isäntäkohtaiset ohjeet](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Jos isännöintipalvelusi on GoDaddy tai toinen isäntä, joka on otettu käyttöön [toimialueen yhteyden muodostamisen](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)yhteydessä , prosessi on helppo ja sinua pyydetään kirjautumaan sisään ja antamaan Microsoftin todentaa henkilöllisyytesi puolestasi.

    ![Valitse GoDaddyConfirm Access (Vahvista käyttöoikeus) -sivulla Valtuuta.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Lisää käyttäjiä ja määritä käyttöoikeuksia

Voit lisätä käyttäjiä ohjattuun toimintoon, mutta voit [myös lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallintakeskukseen. Lisäksi jos sinulla on paikallinen toimialueen ohjauskone, voit lisätä käyttäjiä [Azure AD Connectin](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)avulla.

#### <a name="add-users-in-the-wizard"></a>Käyttäjien lisääminen ohjattuun toimintoon

Kaikki ohjatussa toiminnossa lisäämäsi käyttäjät saavat automaattisesti Microsoft 365 Business -käyttöoikeuden.

![Näyttökuva ohjatun toiminnon Lisää uusia käyttäjiä -sivusta](../media/addnewuserspage.png)

1. Jos Microsoft 365 Business -tilauksessasi on olemassa olevia käyttäjiä (esimerkiksi jos käytit Azure AD Connectia), voit määrittää heille käyttöoikeudet nyt. Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.

2. Kun olet lisännyt käyttäjät, voit myös jakaa tunnistetiedot lisäämäsi uusien käyttäjien kanssa. Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.

### <a name="connect-your-domain"></a>Toimialueen yhdistäminen

> [!NOTE]
> Jos valitsit .onmicrosoft-toimialueen käyttämisen tai käytät Azure AD Connectia käyttäjien määrittämiseen, et näe tätä vaihetta.
  
Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.
  
1. Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa. Jos näin ei ole, [Muuta nimipalvelimia niin, että Office 365 määritetään minkä tahansa toimialueen rekisteröintipalvelun kanssa.](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2) 

    - Jos sinulla on aiemmin luotuja DNS-tietueita, esimerkiksi aiemmin luotu web-sivusto, mutta DNS-isäntä on käytössä [toimialueen yhdistämisessä](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), valitse **Lisää tietueita minulle**. Hyväksy **Valitse verkkopalvelut** -sivulla kaikki oletusarvot ja valitse **Seuraava**ja valitse DNS-isännän sivulla **Valtuuta.**
    - Jos sinulla on aiemmin luotuja DNS-tietueita muiden DNS-isäntien kanssa (ei otettu käyttöön toimialueen yhdistämisessä), sinun kannattaa hallita omia DNS-tietueitasi ja varmistaa, että olemassa olevat palvelut pysyvät yhteydessä toisiinsa. Lisätietoja on [verkkotunnuksen perustiedoissa.](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics)

        ![Aktivoi tietuesivu.](../media/activaterecords.png)

2. Noudata ohjatun toiminnon ohjeita, ja sähköposti ja muut palvelut määritetään puolestasi.

### <a name="protect-your-organization"></a>Suojaa organisaatiosi 

Ohjatussa toiminnossa määritetyt käytännöt otetaan automaattisesti käyttöön *Kaikki käyttäjät* [-suojausryhmässä.](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) Voit myös luoda muita ryhmiä, joihin käytännöt määritetään hallintakeskuksessa.

1. **Lisäsuojaa kehittyneiltä kyberuhkilta**-kohdassa on suositeltavaa hyväksyä oletusarvot, joiden avulla [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) voi skannata tiedostoja ja linkkejä Office-sovelluksissa.

    ![Näyttökuva Lisää suojaus -sivusta.](../media/increasetreatprotection.png)


2. Hyväksy **Estä arkaluonteisten tietojen vuodot** -sivulla oletukset, joiden mukaan Office 365 Data Loss Prevention (DLP) ottaa käyttöön arkaluonteisten tietojen seuraamiseksi Office-sovelluksissa ja estääksesi niiden tahattoman jakamisen organisaation ulkopuolella.

3. Jätä **Suojaa tiedot Office mobiililaitteille -sivulla** mobiilisovellusten hallinta päälle, laajenna asetukset ja tarkista ne ja valitse sitten **Luo mobiilisovellusten hallintakäytäntö**.

    ![Näyttökuva Suojaa tiedot Office mobiililaitteille -sivulla.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Suojaa Windows 10 -tietokoneet

Valitse vasemmassa siirtymisruudussa **Asetukset** ja valitse sitten **Sing-in ja security (Suojaa** **Windows 10 -tietokoneet)**-kohdasta. Aloita valitsemalla **Näytä.** Katso täydelliset ohjeet [noudattamalla Windows 10 -tietokoneiden suojaaminen.](secure-win-10-pcs.md)

## <a name="deploy-office-365-client-apps"></a>Office 365 -asiakassovellusten käyttöönotto

Jos valitsit Office-sovellusten automaattisen asennuksen asennuksen aikana, sovellukset asennetaan Windows 10 -laitteisiin, kun käyttäjät ovat kirjautuneet Azure AD:hen Windows-laitteistaan käyttämällä työtunnistetietojaan.

Lisätietoja Officen asentamisesta mobiili-iOS- tai Android-laitteisiin on ohjeaiheessa [Mobiililaitteiden määrittäminen Microsoft 365 Business -käyttäjille](set-up-mobile-devices.md).

Voit asentaa Officen myös yksitellen. Katso ohjeet [artikkelista Officen asentaminen PC- tai Mac-tietokoneeseen.](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658)

## <a name="see-also"></a>Tutustu myös seuraaviin ohjeaiheisiin

[Microsoft 365 Business -koulutusvideot](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
