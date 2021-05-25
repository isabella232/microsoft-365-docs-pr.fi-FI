---
title: Määritä Microsoft 365 Business Premium
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
description: Tutustu määritykseen, Microsoft 365 Business Premium, kuten toimialueen ja käyttäjien lisääminen, suojauskäytäntöjen määrittäminen ja paljon muuta.
ms.openlocfilehash: 3e15f16db2a233d2e11d444600398102b075932d
ms.sourcegitcommit: 686f192e1a650ec805fe8e908b46ca51771ed41f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/24/2021
ms.locfileid: "52624385"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Asetusten Microsoft 365 Business Premium määrittäminen ohjatussa määritystoiminnossa

## <a name="watch-overview-of-microsoft-365-setup"></a>Katso: Yleiskatsaus Microsoft 365 asetuksiin

Tässä videossa on yleiskatsaus Microsoft 365 Business Premium määrityksestä.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a>Toimialueen, käyttäjien ja käytännöt lisääminen

Kun ostat Microsoft 365 Business Premium, voit käyttää omaa toimialuetta tai ostaa sellaisen [rekisteröitymisen yhteydessä.](sign-up.md)

- Jos ostit uuden toimialueen rekisteröityessäsi, toimialueesi on kaikki määritetty ja voit siirtyä Lisää käyttäjiä -alueeseen [ja määrittää käyttöoikeuksia.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>Toimialueen lisääminen sisäänkirjautumista varten

1. Kirjaudu Microsoft 365 [hallintakeskukseen yleisen](https://admin.microsoft.com) järjestelmänvalvojan tunnistetiedoilla. 

2. Käynnistä **ohjattu toiminto valitsemalla** Siirry asennukseen.

    ![Valitse Siirry asennukseen.](../media/gotosetupinadmincenter.png)

3. Voit **halutessasi asentaa Office sovellukset** omaan tietokoneeseesi Asenna omat sovellukset -sivulla.
    
4. Kirjoita **Lisää toimialue -vaiheessa** toimialuenimi, jota haluat käyttää (kuten contoso.com).

    > [!IMPORTANT]
    > Jos olet ostanut toimialueen rekisteröitymisen aikana, Lisää toimialue -vaihetta **ei ole** tässä. Siirry sen sijaan Lisää käyttäjiä -ylle. [](#add-users-and-assign-licenses)

    ![Näyttökuva Mukauta kirjautumista -sivusta.](../media/adddomain.png)

    
4. Noudata ohjatun toiminnon ohjeita kohdassa DNS-tietueiden luominen missä tahansa [DNS-isännöintipalvelussa Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) vahvistaa, että omistat toimialueen. Jos tiedät toimialueesi isännän, katso myös [isäntäkohtaiset ohjeet](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Jos isännöintipalvelusi on GoDaddy [](/office365/admin/get-help-with-domains/domain-connect)tai jokin muu isännöintipalvelu, jossa on käytössä toimialue, prosessi on helppo, ja sinua pyydetään automaattisesti kirjautumaan sisään ja antamaan Microsoftin todentaa puolestasi.

    ![Valitse GoDaddyn Vahvista käyttö -sivulla Valtuuta.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Lisää käyttäjiä ja määritä käyttöoikeuksia

Voit lisätä käyttäjiä ohjatussa toiminnossa, mutta voit myös [lisätä käyttäjiä myöhemmin](../admin/add-users/add-users.md) hallintakeskuksessa. Lisäksi jos sinulla on paikallinen toimialueen ohjauskone, voit lisätä käyttäjiä, joilla on [Azure AD Näyttöyhteys.](/azure/active-directory/hybrid/how-to-connect-install-express)

#### <a name="add-users-in-the-wizard"></a>Käyttäjien lisääminen ohjatussa toiminnossa

Kaikki ohjatussa toiminnossa lisäät käyttäjät saavat automaattisesti Microsoft 365 Business Premium käyttöoikeuden.

![Näyttökuva ohjatun toiminnon Lisää uusia käyttäjiä -sivusta](../media/addnewuserspage.png)

1. Jos Microsoft 365 Business Premium on olemassa olevia käyttäjiä (jos esimerkiksi käytit Azure AD Näyttöyhteys:tä), voit määrittää heille käyttöoikeudet nyt. Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.

2. Kun olet lisännyt käyttäjät, voit myös jakaa tunnistetiedot lisäämisen uusien käyttäjien kanssa. Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.

### <a name="connect-your-domain"></a>Toimialueen yhdistäminen

> [!NOTE]
> Jos päätit käyttää .onmicrosoft-toimialuetta tai määrittää Näyttöyhteys Azure AD:llä, et näe tätä vaihetta.
  
Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.
  
1. Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa. Jos näin ei ole, muuta nimipalvelimia niin, että [ne Microsoft 365 toimialuerekisteröijän kanssa.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md) 

    - Jos sinulla on olemassa olevia DNS-tietueita, esimerkiksi olemassa oleva sivusto, mutta DNS-isännöintipalvelusi on otettu käyttöön toimialueen [yhteydessä](/office365/admin/get-help-with-domains/domain-connect), valitse **Lisää tietueet minulle**. Hyväksy **Valitse verkkopalvelut -sivulla** kaikki oletusasetukset, valitse Seuraava ja **valitse** DNS-isännöintipalvelun sivulla Valtuuta.
    - Jos sinulla on aiemmin luotuja DNS-tietueita muiden DNS-isännöintipalvelujen kanssa (ei otettu käyttöön toimialueen yhdistettynä), sinun on hallittava omia DNS-tietueitasi ja varmistaa, että olemassa olevat palvelut ovat yhteydessä toisiinsa. Lisätietoja on toimialueen perustoimialueissa. [](/office365/admin/get-help-with-domains/dns-basics)

        ![Aktivoi tietueet -sivu.](../media/activaterecords.png)

2. Noudata ohjatun toiminnon ohjeita, niin sähköposti ja muut palvelut määritetään sinulle.

### <a name="protect-your-organization"></a>Suojaa organisaatiosi 

Ohjatussa toiminnossa määrittänyt käytännöt otetaan [](/office365/admin/create-groups/compare-groups#security-groups) automaattisesti käyttöön Kaikki käyttäjät *-käyttöoikeusryhmässä.* Voit myös luoda muita ryhmiä, joissa käytäntöjä määritetään hallintakeskuksessa.

1. Paranna **kehittyneiden kyberuhkien** suojausta -sivulla on suositeltavaa hyväksyä oletusasetukset, jotta [Office 365 Advance Threat Protectionin](../security/office-365-security/defender-for-office-365.md) tarkistustiedostot ja linkit Office sovelluksissa.

    ![Näyttökuva Lisää suojausta -sivusta.](../media/increasetreatprotection.png)


2. Hyväksy **Estä** luottamuksellisten tietojen vuodot -sivulla oletusarvot, jotka Office 365 Tietojen menetyksen estäminen (DLP) -asetuksen käyttöön, jotta voit seurata luottamuksellisia tietoja Office-sovelluksissa ja estää niiden tahattoman jakamisen organisaation ulkopuolelle.

3. Jätä **Mobiilisovellusten Office** -sivulla Mobiilisovellusten hallinta käyttöön, laajenna asetukset, tarkista ne ja valitse sitten Luo **mobiilisovellusten hallintakäytäntö**.

    ![Näyttökuva Suojaa Office mobiiliversiossa -sivusta.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Suojattu Windows 10 tietokoneet

Valitse vasemmassa siirtymisruudussa **Asetukset** ja valitse sitten **Kirjautumis-** ja suojaus -kohdassa **Suojaa Windows 10 tietokoneet**. Aloita **valitsemalla** Näytä. Katso [Windows 10 tietokoneen suojaaminen.](secure-win-10-pcs.md)

## <a name="deploy-office-365-client-apps"></a>Asiakassovellusten Office 365 käyttöönotto

Jos päätit asentaa Office-sovellukset automaattisesti asennuksen aikana, sovellukset asennetaan Windows 10-laitteisiin, kun käyttäjät ovat kirjautuneet Sisään Azure AD:iin Windows-laitteistaan työtunnuksilla.

Jos haluat asentaa Office iOS- tai Android-laitteisiin, katso mobiililaitteiden [Microsoft 365 Business Premium käyttöön.](set-up-mobile-devices.md)

Voit myös asentaa Office erikseen. Katso [Office PC: lle tai Macille](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) asennusohjeet.

## <a name="related-content"></a>Aiheeseen liittyvä sisältö

[Microsoft 365 yrityksille 2010 -koulutusvideoita](../business-video/index.yml) (linkkisivu)
