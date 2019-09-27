---
title: Microsoft 365 Businessin määrittäminen
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Lue lisä tietoja Microsoft 365 Businessin määrittämisestä.
ms.openlocfilehash: d33839693001f36fbb56541775015f739300b043
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288491"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Microsoft 365-liike toiminnan määrittäminen ohjatussa asennus toiminnossa

## <a name="add-your-domain-users-and-set-up-policies"></a>Lisää toimi alue, käyttäjät ja määritä käytännöt

[![Etiketti, jonka avulla voit tietää, että hallinta keskus on muuttumassa ja löydät lisä tietoja osoitteessa aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Kun ostat Microsoft 365 Businessin, sinulla on mahdollisuus käyttää omistamaani verkko tunnusta tai ostaa se [rekisteröityessäsi](sign-up.md).

- Jos olet hankkinut uuden verkko tunnuksen, kun olet rekisteröitynyt, toimi alueesi on määritetty ja voit siirtyä lisäämään [käyttäjiä ja määrittämään lisenssejä](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Lisää verkko tunnuksesi mukauttamaan sisäänkirjautumista

1. Kirjaudu sisään [Microsoft 365-hallinta keskukseen](https://admin.microsoft.com) käyttämällä yleisiä järjestelmänvalvojan tunniste tietoja. 

2. Käynnistä ohjattu toiminto valitsemalla **Lisää toimi alue** tai **Lisää käyttäjiä** .
    > [!IMPORTANT]
    > Jos ostit verkko tunnuksen rekisteröitymistä varten, et näe **Lisää toimi** alue-vaihetta tässä. Siirry sen sijaan kohtaan [Lisää käyttäjiä](#add-users-and-assign-licenses) .

    ![Valitse Lisää toimi alue.](media/addadomainadmincenter.png)
    
3. Kirjoita ohjatussa toiminnossa haluamasi toimi alueen nimi (kuten contoso.com).


    ![Kuva kaappaus Mukauta kirjautumissivua.](media/personalizesignin.png)

    
4. Noudata ohjatun toiminnon ohjeita [luodaksesi DNS-tietueet missä tahansa DNS-isännöinti palvelun tarjoajana (Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) ), joka varmistaa, että omistat toimi alueen. Jos tiedät verkko tunnuksesi isäntäsi, Katso myös [isännän erityiset ohjeet](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Jos palveluntarjoajasi on GoDaddy tai toinen isäntä, joka on otettu käyttöön [Domain Connectin](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)kanssa, prosessi on helppoa ja sinua pyydetään automaattisesti Kirjautu maan sisään ja anna Microsoftin todentaa se puolestasi:

    ![Valitse GoDaddy Confirm Access-sivulla Valtuuta.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Lisää käyttäjiä ja määritä käyttöoikeuksia

Voit lisätä käyttäjiä ohjatussa toiminnossa, mutta voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallinta keskukseen. Lisäksi jos sinulla on paikallinen toimi alueen ohjaus kone, voit lisätä käyttäjiä [Azure AD Connectin](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)avulla.

#### <a name="add-users-in-the-wizard"></a>Lisää käyttäjiä ohjatussa toiminnossa

Kaikki käyttäjät, jotka lisäät ohjatussa toiminnossa, saavat automaattisesti Microsoft 365-yritys käyttö oikeuden.

![Ohjatun toiminnon lisää uusia käyttäjiä-sivun kuva kaappaus](media/addnewuserspage.png)

1. Jos Microsoft 365-liiketoiminta tilauksessasi on aiemmin luotuja käyttäjiä (Jos esimerkiksi käytit Azure AD Connectia), saat mahdollisuuden määrittää heille käyttö oikeudet nyt. Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.

3. Kun olet lisännyt käyttäjät, saat myös mahdollisuuden jakaa tunniste tiedot lisättyjen uusien käyttäjien kanssa. Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.

4. Ohita sähköpostiviestien siirtäminen valitsemalla **Siirrä sähköpostiviestejä** -sivulla **Seuraava**. 

    Jos siirryt toisesta Sähkö posti palvelusta ja haluat kopioida tietosi myöhemmin, voit [siirtää sähkö postin ja yhteys tiedot Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e)-palveluun.


### <a name="connect-your-domain"></a>Toimialueen yhdistäminen

> [!NOTE]
> Jos valitsit. onmicrosoft-toimi alueen tai käytät Azure AD Connectia käyttäjien määrittämisestä, et näe tätä vaihetta.
  
Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.
  
1. Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa. Jos näin ei ole, [Vaihda nimi palvelimet, jotta voit määrittää Office 365-palvelimen minkä tahansa toimi alueen rekisterin pitäjän kanssa](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Jos sinulla on aiemmin luotuja DNS-tietueita, esimerkiksi olemassa oleva Web-sivusto, mutta DNS-isäntä on otettu käyttöön [toimi alueen yhdistämä](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), valitse **Lisää tietueita minulle**. 
    - Jos sinulla on aiemmin luotuja DNS-tietueita muiden DNS-Isän tien kanssa (ei käytössä toimi alueen yhteydessä), haluat hallita omia DNS-tietueita ja varmistaa, että olemassa olevat palvelut ovat yhteydessä toisiinsa. Lisä tietoja on kohdassa [toimi alueen perusteet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .

        ![Yhdistä verkko tunnuksesi sivu, jolla hallitsen omia DNS-tietueita.](media/connectyourdomainpage.png)

2. Noudata ohjatun toiminnon ohjeita, ja Sähkö posti ja muut palvelut määritetään puolestasi.

### <a name="set-up-security-policies-and-device-configurations"></a>Suojaus käytäntöjen ja laite konfiguraatioiden määrittäminen 

Ohjatussa toiminnossa käyttöön luomat käytännöt kohdistetaan automaattisesti [Suojaus ryhmään](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) nimeltä *Kaikki käyttäjät*. Voit myös luoda lisä ryhmiä määrittämään käytäntöjä hallinta keskuksessa.

1. **Suojaa työtiedostojasi mobiililaitteilla** -vaihto ehto **suojaa työtiedostot, kun laitteet katoavat tai varastetaan** , valitaan oletusarvoisesti. Sinulla on mahdollisuus ottaa käyttöön Hallitse, **miten käyttäjät voivat käyttää Office-tiedostoja mobiililaitteissa**, ja tätä suositellaan.

    ![Kuva kaappaus suojaa työtiedostot mobiililaitteiden sivulla.](media/protectworkfilesondevices.png)

     - Laajenna **suojaa työtiedostot, kun laitteet katoavat tai varastetaan** näyttämään [oletus arvot](protect-work-files-on-lost-or-stolen-device.md):

        ![Kuva kaappaus oletus arvoista tiedostojen suojaamiseksi kadonneita laitteita.](media/protectworkfilesondevicesdefault.png)

    - Valitse **Hallitse, miten käyttäjät voivat käyttää Office-tiedostoja mobiililaitteissa** ja laajentaa sitä näyttämään [oletus arvot](manage-user-access-on-mobile-devices.md). Microsoft suosittelee, että hyväksyt oletus arvot asennuksen aikana, jotta voit luoda sovellus käytäntöjä Androidille, iOS:lle ja Windows 10: lle, jotka koskevat kaikkia käyttäjiä. Voit luoda lisää käytäntöjä asennuksen päätyttyä.

        ![Kuva kaappaus Office-tiedostojen suojaus asetuksista mobiililaitteilla.](media/useraccessonmobile.png)

2. Tieto suojaa koskevien tietojen ja laitteiden viimeisessä vaiheessa voit määrittää käytäntöjä Windows 10-laitteiden suojaamiseksi. Näitä asetuksia käytetään automaattisesti, kun käyttäjän Windows 10 muodostaa yhteyden organisaatioosi. Voit tarkastella ja muokata [oletus arvoja](secure-windows-10-devices.md)laajentamalla **suojatut Windows 10-laitteet** .
3. Voit myös halutessasi [asentaa Officen automaattisesti](install-office-on-windows-10-during-setup.md) Windows 10-laitteisiin.

    ![Kuva kaappaus asetettu Windows 10 laitteen kokoonpano sivu.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a>Office 365-asiakas sovellusten käyttöönotto

Jos valitsit, että Office-sovellukset asennetaan automaattisesti asennuksen aikana, sovellukset asennetaan Windows 10-laitteisiin sen jälkeen, kun käyttäjät ovat kirjauduneet Azure ADIIN Windows-laitteistaan työn tunniste tiedoilla.
Jos haluat asentaa Officen mobiililaitteisiin iOS-tai Android-laitteisiin, katso [Microsoft 365-yritys käyttäjien mobiililaitteiden määrittäminen](set-up-mobile-devices.md).

Voit myös asentaa Officen yksitellen. Katso ohjeet [Officen asentamisesta PC:hen tai Maciin](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .
