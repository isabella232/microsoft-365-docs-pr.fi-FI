---
title: Microsoft 365 Business Premiumin määritäminen
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
description: Tutustu Microsoft 365 Business Premiumin määritysvaiheisiin, kuten toimialueen ja käyttäjien lisäämiseen, suojauskäytäntöjen määrittämiseen ja paljon muuta.
ms.openlocfilehash: a06fb48ef5e1386a5c7b4df08500125f37943df6
ms.sourcegitcommit: dcb97fbfdae52960ae62b6faa707a05358193ed5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/25/2021
ms.locfileid: "51198428"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Microsoft 365 Business Premiumin määrittäminen ohjatussa määritystoiminnossa

Tässä videossa on yleiskuvaus Microsoft 365 Business Premiumin määrityksestä.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a>Lisää toimialue, käyttäjät ja määritä käytännöt

Kun ostat Microsoft 365 Business Premiumin, voit käyttää omaa toimialuetta tai ostaa sellaisen [rekisteröitymisen aikana.](sign-up.md)

- Jos ostit uuden toimialueen rekisteröityessäsi, toimialueesi on määritetty, ja voit siirtyä Lisää käyttäjiä -asentoon [ja määrittää käyttöoikeuksia.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>Toimialueen lisääminen sisäänkirjautumista varten

1. Kirjaudu [Microsoft 365 -hallintakeskukseen yleisen](https://admin.microsoft.com) järjestelmänvalvojan tunnistetiedoilla. 

2. Käynnistä **ohjattu toiminto valitsemalla** Siirry asennukseen.

    ![Valitse Siirry asennukseen.](../media/gotosetupinadmincenter.png)

3. Asenna **Office-sovellukset -sivulla** voit halutessasi asentaa sovellukset omaan tietokoneeseesi.
    
4. Kirjoita **Lisää toimialue -vaiheeseen** toimialuenimi, jota haluat käyttää (kuten contoso.com).

    > [!IMPORTANT]
    > Jos olet ostanut toimialueen rekisteröitymisen aikana, Lisää toimialue -vaihetta ei **ole** tässä. Siirry sen sijaan Lisää käyttäjiä -ylle. [](#add-users-and-assign-licenses)

    ![Näyttökuva Mukauta kirjautumissivua -ruudusta.](../media/adddomain.png)

    
4. Luo DNS-tietueet missä tahansa [Microsoft 365:n](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) DNS-isännöintipalvelussa ohjatun toiminnon ohjeiden mukaisesti, joka vahvistaa, että omistat toimialueen. Jos tiedät toimialueesi isännän, tutustu myös [isäntäkohtaisiin ohjeisiin.](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)

    Jos isännöintipalvelusi on GoDaddy tai jokin muu isännöintipalvelu on otettu käyttöön toimialueen [yhteydessä,](/office365/admin/get-help-with-domains/domain-connect)prosessi on helppoa, ja sinua pyydetään automaattisesti kirjautumaan sisään ja antamaan Microsoftin todentaa asia puolestasi.

    ![Valitse GoDaddyn Vahvista käyttö -sivulla Valtuuta.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Lisää käyttäjiä ja määritä käyttöoikeuksia

Voit lisätä käyttäjiä ohjatussa toiminnossa, mutta voit myös [lisätä käyttäjiä](../admin/add-users/add-users.md) myöhemmin hallintakeskuksessa. Lisäksi, jos sinulla on paikallinen toimialueen ohjauskone, voit lisätä käyttäjiä [Azure AD Connectilla.](/azure/active-directory/hybrid/how-to-connect-install-express)

#### <a name="add-users-in-the-wizard"></a>Käyttäjien lisääminen ohjatussa toiminnossa

Kaikille ohjatussa toiminnossa lisäämiesi käyttäjien käyttöön määritetään automaattisesti Microsoft 365 Business Premium -käyttöoikeus.

![Näyttökuva ohjatun toiminnon Lisää uusia käyttäjiä -sivusta](../media/addnewuserspage.png)

1. Jos Microsoft 365 Business Premium -tilauksessasi on aiemmin luotuja käyttäjiä (jos olet esimerkiksi käyttänyt Azure AD Connectia), voit määrittää heille käyttöoikeuksia nyt. Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.

2. Kun olet lisännyt käyttäjät, voit myös jakaa tunnistetiedot lisäätyille uusille käyttäjille. Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.

### <a name="connect-your-domain"></a>Toimialueen yhdistäminen

> [!NOTE]
> Jos päätit käyttää .onmicrosoft-toimialuetta tai olet määrittänyt käyttäjiä Azure AD Connectin avulla, et näe tätä vaihetta.
  
Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.
  
1. Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa. Jos näin ei ole, [muuta nimipalvelimet niin, että Microsoft 365 määritetään minkä tahansa toimialuerekisteröijän kanssa.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md) 

    - Jos sinulla on aiemmin luotuja DNS-tietueita, esimerkiksi aiemmin luotu verkkosivusto, mutta DNS-isännöintipalvelusi on otettu käyttöön [toimialueen](/office365/admin/get-help-with-domains/domain-connect)yhteydessä, valitse **Lisää tietueet minulle.** Hyväksy **Valitse verkkopalvelut -sivulla** kaikki oletusasetukset, valitse Seuraava  ja valitse DNS-isännöintipalvelun sivulla Valtuuta.
    - Jos sinulla on aiemmin luotuja DNS-tietueita muiden DNS-isännöintipalvelujen kanssa (toimialueiden yhdistäminen ei ole käytössä), sinun on hallittava omia DNS-tietueitasi ja varmistaa, että olemassa olevat palvelut ovat yhteydessä toisiinsa. Lisätietoja on toimialueen perustoimialueissa. [](/office365/admin/get-help-with-domains/dns-basics)

        ![Aktivoi tietueet -sivu.](../media/activaterecords.png)

2. Noudata ohjatun toiminnon ohjeita, ja sähköposti ja muut palvelut määritetään sinulle.

### <a name="protect-your-organization"></a>Suojaa organisaatiosi 

Ohjatussa toiminnossa määritettyjä käytäntöjä käytetään automaattisesti Kaikki käyttäjät [-käyttöoikeusryhmässä.](/office365/admin/create-groups/compare-groups#security-groups)  Voit myös luoda muita ryhmiä, jotta voit määrittää käytäntöjä hallintakeskuksessa.

1. **Edistyneiltä** kyberuhkilta suojauksen lisäämisen osalta on suositeltavaa hyväksyä oletusasetukset, jotta [Office 365 Advance Threat Protection](../security/office-365-security/defender-for-office-365.md) -sovelluksen tiedostot ja linkit voidaan tarkistaa Office-sovelluksissa.

    ![Näyttökuva Suurenna suojausta -sivusta.](../media/increasetreatprotection.png)


2. Hyväksy **Estä** luottamuksellisten tietojen vuodot -sivulla oletusarvot, joilla Office 365:n tietojen menetyksen estäminen (DLP) voidaan ottaa käyttöön, jotta voit seurata luottamuksellisia tietoja Office-sovelluksissa ja estää niiden tahattoman jakamisen organisaation ulkopuolelle.

3. Jätä Suojaa **tiedot Officen** mobiiliversiossa -sivulla mobiilisovellusten hallinta käyttöön, laajenna asetuksia ja tarkista ne ja valitse sitten Luo **mobiilisovelluksen hallintakäytäntö.**

    ![Näyttökuva Suojaa tiedot Office for Mobile -sivulla.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Windows 10 -tietokoneiden suojaaminen

Valitse vasemmassa siirtymisruudussa **Asetukset** ja valitse sitten Sisäänkirjautuminen ja suojaus **-kohdassa** **Suojaa Windows 10 -tietokoneet.** Aloita **valitsemalla** Näytä. Katso [täydelliset ohjeet Windows 10 -tietokoneiden](secure-win-10-pcs.md) suojaamista varten.

## <a name="deploy-office-365-client-apps"></a>Office 365 -asiakassovellusten käyttöönotto

Jos päätit asentaa Office-sovellukset automaattisesti asennuksen aikana, sovellukset asennetaan Windows 10 -laitteisiin, kun käyttäjät ovat kirjautuneet Azure AD:lle Windows-laitteistaan työtunnuksilla.

Lisätietoja Officen asentamisesta iOS- tai Android-mobiililaitteisiin on kohdassa Mobiililaitteiden asentaminen [Microsoft 365 Business Premium -käyttäjille.](set-up-mobile-devices.md)

Voit asentaa Officen myös yksitellen. Katso [ohjeet Officen asentamisesta PC- tai Mac-tietokoneeseen.](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658)

## <a name="see-also"></a>Tutustu myös seuraaviin ohjeartikkeleihin:

[Microsoft 365 for Business -koulutusvideot](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
