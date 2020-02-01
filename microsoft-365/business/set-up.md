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
description: Lue lisä tietoja Microsoft 365 Businessin määrittämisestä.
ms.openlocfilehash: c370a5b3fd735e704eea56ac1079bb2e5dad4c4b
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594265"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Microsoft 365-liike toiminnan määrittäminen ohjatussa asennus toiminnossa

Katso tästä videosta yleiskatsaus Microsoft 365-liike toiminnan asennukseen.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

## <a name="add-your-domain-users-and-set-up-policies"></a>Lisää toimi alue, käyttäjät ja määritä käytännöt

[![Selite, jossa ilmoitetaan, että hallintakeskus muuttuu. Lisätietoja löytyy osoitteesta aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Kun ostat Microsoft 365 Businessin, sinulla on mahdollisuus käyttää omistamaani verkko tunnusta tai ostaa se [rekisteröityessäsi](sign-up.md).

- Jos olet hankkinut uuden verkko tunnuksen, kun olet rekisteröitynyt, toimi alueesi on määritetty ja voit siirtyä lisäämään [käyttäjiä ja määrittämään lisenssejä](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Lisää verkko tunnuksesi mukauttamaan sisäänkirjautumista

1. Kirjaudu sisään [Microsoft 365-hallinta keskukseen](https://admin.microsoft.com) käyttämällä yleisiä järjestelmänvalvojan tunniste tietoja. 

2. Käynnistä ohjattu toiminto valitsemalla **Siirry asennukseen** .

    ![Valitse Siirry asennukseen.](media/gotosetupinadmincenter.png)

3. Voit vaihtoehtoisesti asentaa sovellukset omaan tieto koneeseesi **Asenna Office-sovellukset** -sivulla.
    
4. Kirjoita **Lisää toimi alue** -vaiheeseen toimi alue nimi, jota haluat käyttää (kuten contoso.com).

    > [!IMPORTANT]
    > Jos ostit verkko tunnuksen rekisteröitymistä varten, et näe **Lisää toimi** alue-vaihetta tässä. Siirry sen sijaan kohtaan [Lisää käyttäjiä](#add-users-and-assign-licenses) .

    ![Kuva kaappaus Mukauta kirjautumissivua.](media/adddomain.png)

    
4. Noudata ohjatun toiminnon ohjeita [luodaksesi DNS-tietueet missä tahansa DNS-isännöinti palvelun tarjoajana (Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) ), joka varmistaa, että omistat toimi alueen. Jos tiedät verkko tunnuksesi isäntäsi, Katso myös [isännän erityiset ohjeet](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Jos hosting-palveluntarjoajasi on GoDaddy tai toinen isäntä, joka on otettu käyttöön [Domain Connectin](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)kanssa, prosessi on helppoa ja sinua pyydetään automaattisesti Kirjautu maan sisään ja anna Microsoftin todentaa se puolestasi.

    ![Valitse GoDaddy Confirm Access-sivulla Valtuuta.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Lisää käyttäjiä ja määritä käyttöoikeuksia

Voit lisätä käyttäjiä ohjatussa toiminnossa, mutta voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallinta keskukseen. Lisäksi jos sinulla on paikallinen toimi alueen ohjaus kone, voit lisätä käyttäjiä [Azure AD Connectin](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)avulla.

#### <a name="add-users-in-the-wizard"></a>Lisää käyttäjiä ohjatussa toiminnossa

Kaikki käyttäjät, jotka lisäät ohjatussa toiminnossa, saavat automaattisesti Microsoft 365-yritys käyttö oikeuden.

![Ohjatun toiminnon lisää uusia käyttäjiä-sivun kuva kaappaus](media/addnewuserspage.png)

1. Jos Microsoft 365-liiketoiminta tilauksessasi on aiemmin luotuja käyttäjiä (Jos esimerkiksi käytit Azure AD Connectia), saat mahdollisuuden määrittää heille käyttö oikeudet nyt. Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.

2. Kun olet lisännyt käyttäjät, saat myös mahdollisuuden jakaa tunniste tiedot lisättyjen uusien käyttäjien kanssa. Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.

### <a name="connect-your-domain"></a>Toimialueen yhdistäminen

> [!NOTE]
> Jos valitsit. onmicrosoft-toimi alueen tai käytät Azure AD Connectia käyttäjien määrittämisestä, et näe tätä vaihetta.
  
Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.
  
1. Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa. Jos näin ei ole, [Vaihda nimi palvelimet, jotta voit määrittää Office 365-palvelimen minkä tahansa toimi alueen rekisterin pitäjän kanssa](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Jos sinulla on aiemmin luotuja DNS-tietueita, esimerkiksi olemassa oleva Web-sivusto, mutta DNS-isäntä on otettu käyttöön [toimi alueen yhdistämä](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), valitse **Lisää tietueita minulle**. Hyväksy **Valitse online-palvelut** -sivulla kaikki oletus arvot, valitse **Seuraava** **ja valitse sitten Hyväksy DNS** -isännän sivulla.
    - Jos sinulla on DNS-tietueita muiden DNS-Isän tien kanssa (ei käytössä toimi alueen yhteydessä), sinun kannattaa hallita omia DNS-tietueita ja varmistaa, että olemassa olevat palvelut ovat yhteydessä toisiinsa. Lisä tietoja on kohdassa [toimi alueen perusteet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .

        ![Aktivoi tietueet-sivu.](media/activaterecords.png)

2. Noudata ohjatun toiminnon ohjeita, ja Sähkö posti ja muut palvelut määritetään puolestasi.

### <a name="protect-your-organization"></a>Organisaation suojaaminen 

Ohjatussa toiminnossa käyttöön luomat käytännöt kohdistetaan automaattisesti [Suojaus ryhmään](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) nimeltä *Kaikki käyttäjät*. Voit myös luoda lisä ryhmiä määrittämään käytäntöjä hallinta keskuksessa.

1. **Lisä suojaa kehittyneiltä kyberuhkilta**suositellaan, että hyväksyt oletus asetukset, jotta [Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) -tieto turva tarkistus tiedostot ja linkit Office-sovelluksissa hyväksytään.

    ![Kuva kaappaus lisää suojausta-sivulta.](media/increasetreatprotection.png)


2. Hyväksy **arkaluontoisten tietojen vuodot** -sivun oletus asetukset, jos haluat ottaa Office 365-tietojen menetyksen eston (DLP) käyttöön, jotta voit seurata luottamuksellisia tietoja Office-sovelluksissa ja estää niiden tahattoman jakamisen organisaatiosi ulkopuolella.

3. Jätä Mobile-sovelluksen hallinta päälle, Laajenna asetukset ja tarkista ne ja valitse sitten **Luo mobiilisovelluksen hallinta käytäntö**, jos **haluat suojata Officen mobiiliverdauksen tiedot** -sivulla.

    ![Kuva kaappaus Office for Mobile-sivun tietojen suojaamisesta.](media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Secure Windows 10-tieto koneet

Valitse vasemmasta siirtymis kohdasta **Asetukset** ja valitse sitten **Sing-in ja Security**-kohdasta **suojaa Windows 10-tieto koneesi**. Pääset alkuun valitsemalla **Näytä** . Katso täydelliset ohjeet kohdasta [Windows 10-tieto koneiden suojaaminen](secure-win-10-pcs.md) .

## <a name="deploy-office-365-client-apps"></a>Office 365-asiakas sovellusten käyttöönotto

Jos valitsit, että Office-sovellukset asennetaan asennuksen aikana automaattisesti, sovellukset asennetaan Windows 10-laitteisiin sen jälkeen, kun käyttäjät ovat kirjauduneet sisään Azure ADIIN Windows-laitteistaan käyttämällä työn tunniste tietoja.

Jos haluat asentaa Officen mobiililaitteisiin iOS-tai Android-laitteisiin, katso [Microsoft 365-yritys käyttäjien mobiililaitteiden määrittäminen](set-up-mobile-devices.md).

Voit myös asentaa Officen yksitellen. Katso ohjeet [Officen asentamisesta PC:hen tai Maciin](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .

## <a name="see-also"></a>Tutustu myös seuraaviin ohjeaiheisiin

[Microsoft 365 Business -koulutusvideot](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
