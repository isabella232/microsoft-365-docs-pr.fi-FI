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
description: Tutustu Microsoft 365 Business Premiumin määritys vaiheisiin, joita ovat esimerkiksi toimi alueen ja käyttäjien lisääminen, tieto turva käytäntöjen määrittäminen ja paljon muuta.
ms.openlocfilehash: cc20637d7a78bd34ecb61a4ed46eb06d564d63df
ms.sourcegitcommit: 25afc0c34edc7f8a5eb389d8c701175256c58ec8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/01/2020
ms.locfileid: "47324492"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Microsoft 365 Business Premiumin määrittäminen ohjatussa määritys toiminnossa

Katsomalla tämän videon saat yleiskatsauksen Microsoft 365 Business Premium-asennuksesta.<br><br>

## <a name="add-your-domain-users-and-set-up-policies"></a>Toimi alueen, käyttäjien ja käytäntöjen määrittäminen

Kun ostat Microsoft 365 Business Premiumin, sinulla on mahdollisuus käyttää omaa toimi aluettasi tai ostaa se [rekisteröitymisen](sign-up.md)yhteydessä.

- Jos olet ostanut uuden toimi alueen rekisteröityessäsi, toimi alueesi on määritetty ja voit siirtyä [käyttäjien lisäämiseen ja käyttö oikeuksien määrittämiseen](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Toimi alueen lisääminen kirjautumisen mukauttamiseen

1. Kirjaudu sisään [Microsoft 365-hallinta keskukseen](https://admin.microsoft.com) käyttämällä yleisiä järjestelmänvalvojan tunniste tietoja. 

2. Käynnistä ohjattu toiminto valitsemalla **Siirry asetuksiin** .

    ![Valitse Siirry asetuksiin.](../media/gotosetupinadmincenter.png)

3. **Asenna Office-sovellukset** -sivulla voit halutessasi asentaa sovellukset omaan tieto koneeseesi.
    
4. Kirjoita **Lisää toimi alue** -vaiheeseen haluamasi toimi alueen nimi (esimerkiksi contoso.com).

    > [!IMPORTANT]
    > Jos ostit toimi alueen rekisteröitymisen aikana, et näe **Lisää toimi alue** vaihetta tässä. Siirry kohtaan [Lisää käyttäjiä](#add-users-and-assign-licenses) .

    ![Näyttö kuva Mukauta kirjautumissivusi-sivusta.](../media/adddomain.png)

    
4. Noudattamalla ohjatun toiminnon ohjeita voit [luoda DNS-tietueita missä tahansa Microsoft 365-palvelun DNS-isännöinti palvelussa](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , joka vahvistaa, että omistat toimi alueen. Jos tiedät toimi alueen isännältä, Katso myös [tarkat isännöinti ohjeet](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Jos isännöinti palvelusi on GoDaddy tai jokin muu palvelin, jossa on käytössä [Domain Connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), prosessi on helppo, ja sinua pyydetään automaattisesti Kirjautu maan sisään ja päästämään Microsoft todennetaan puolestasi.

    ![Valitse GoDaddy-vahvistuksen käyttäminen-sivulla Valtuuta.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Lisää käyttäjiä ja määritä käyttöoikeuksia

Voit lisätä käyttäjiä ohjatussa toiminnossa, mutta voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallinta keskuksessa. Lisäksi jos sinulla on paikallinen toimi alueen ohjaus kone, voit lisätä käyttäjiä [Azure AD Connectin](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)avulla.

#### <a name="add-users-in-the-wizard"></a>Käyttäjien lisääminen ohjatussa toiminnossa

Kaikki ohjatussa toiminnossa lisättävät käyttäjät saavat automaattisesti Microsoft 365 Business Premium-käyttö oikeuden.

![Näyttö kuva ohjatun toiminnon lisää uusia käyttäjiä-sivusta](../media/addnewuserspage.png)

1. Jos Microsoft 365 Business Premium-tilauksessasi on olemassa olevia käyttäjiä (jos olet esimerkiksi käyttänyt Azure AD Connectia), saat vaihto ehdon määrittää heille käyttö oikeuksia nyt. Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.

2. Kun olet lisännyt käyttäjät, saat myös mahdollisuuden jakaa tunniste tiedot lisäämiesi uusien käyttäjien kanssa. Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.

### <a name="connect-your-domain"></a>Toimialueen yhdistäminen

> [!NOTE]
> Jos päätät käyttää. oMicrosoft-toimi aluetta tai käyttää Azure AD Connectia käyttäjien määrittämiseen, et näe tätä vaihetta.
  
Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.
  
1. Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa. Jos näin ei tapahdu, [Muuta nimi palvelimia, jotta voit määrittää Microsoft 365 minkä tahansa toimi alueen rekisteröinti palvelun avulla](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar). 

    - Jos sinulla on aiemmin luotuja DNS-tietueita, kuten aiemmin luotua sivustoa, mutta DNS-isäntä on otettu käyttöön [toimi alueen yhteydessä](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), valitse **Lisää tietueet**. Hyväksy **Valitse online-palvelut** -sivulla kaikki oletus asetukset ja valitse sitten **Seuraava**ja valitse **Valtuuta** DNS-isännän sivulla.
    - Jos sinulla on aiemmin luotuja DNS-tietueita muiden DNS-Isän tien kanssa (ei otettu käyttöön toimi alueen yhteydessä), sinun kannattaa hallita omia DNS-tietueitasi ja varmistaa, että olemassa olevat palvelut pysyvät yhteydessä. Lisä tietoja on kohdassa [toimi alueen perusteet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .

        ![Aktivoi tietueet-sivu.](../media/activaterecords.png)

2. Noudata ohjatun toiminnon ohjeita ja Sähkö posti ja muut palvelut määritetään puolestasi.

### <a name="protect-your-organization"></a>Organisaation suojaaminen 

Ohjatussa toiminnossa määritetyt käytännöt otetaan automaattisesti käyttöön *kaikille käyttäjille*- [käyttö oikeus ryhmälle](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) . Voit myös luoda lisää ryhmiä, joiden avulla käytäntöjä voi määrittää hallinta keskuksessa.

1. **Kehittyneiden cyber-uhkien lisä suojauksen**ansiosta on suositeltavaa, että hyväksyt oletus asetukset, joiden avulla voit antaa [Office 365 Advance Threat Protectionin](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) etsiä tiedostoja ja linkkejä Office-sovelluksissa.

    ![Näyttö kuva lisää suojaus-sivusta.](../media/increasetreatprotection.png)


2. Hyväksy luottamuksellisten tietojen **estäminen** -sivulla oletus asetukset, jotta voit ottaa Office 365-tietojen menetyksen estämisen (DLP) käyttöön, jotta voit jäljittämään luottamukselliset tiedot Office-sovelluksissa ja estää niiden tahattoman jakamisen organisaation ulkopuolelta.

3. **Jos haluat suojata tietoja Office mobiililaitteille** -sivulla, poistu mobiilisovellusten Hallin nasta, Laajenna asetukset ja tarkista ne ja valitse sitten **Luo mobiilisovelluksen hallinta käytännön**.

    ![Näyttö kuva tietojen suojaamisesta Office for Mobile-sivulla.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Windows 10-tieto koneiden suojaaminen

Valitse vasemmanpuoleisessa siirtymis ruudussa **määritys** ja valitse sitten **Kirjautuminen ja suojaus**-kohdassa **suojaa Windows 10-tieto koneet**. Aloita valitsemalla **Näytä** . Katso täydelliset ohjeet artikkelista [Windows 10-tieto koneen suojaaminen](secure-win-10-pcs.md) .

## <a name="deploy-office-365-client-apps"></a>Office 365-asiakas sovellusten käyttöönotto

Jos valitsit Office-sovellusten automaattisen asentamisen asennuksen aikana, sovellukset asennetaan Windows 10-laitteisiin, kun käyttäjät ovat kirjautuneet Azure AD:hen Windows-laitteistaan heidän työtunniste tiedoillaan.

Jos haluat asentaa Officen mobiililaitteeseen iOS-tai Android-laitteisiin, Katso lisä tietoja artikkelista [mobiililaitteiden määrittäminen Microsoft 365 Business Premium-käyttäjille](set-up-mobile-devices.md).

Voit myös asentaa Officen yksitellen. Katso ohjeet artikkelista [Officen asentaminen PC-tai Mac-tieto koneeseen](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) .

## <a name="see-also"></a>Tutustu myös seuraaviin ohjeartikkeleihin:

[Microsoft 365 for Business-koulutus videot](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
