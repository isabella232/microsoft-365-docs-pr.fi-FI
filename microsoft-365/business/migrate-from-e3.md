---
title: Siirtyminen Microsoft 365-yritykseen Office 365 E3-tieto koneesta
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Opi siirtämään yrityksesi Microsoft 365 Business Premiumiin Office 365 E3-tieto koneesta.
ms.openlocfilehash: eebf78c24ed4bfd1a4fc2d843f37aebbe3d35e31
ms.sourcegitcommit: c1dd5be42fe0c5dcc7c05817c941edd9076febf8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/02/2020
ms.locfileid: "49558248"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Siirtyminen Office 365 E3-tieto koneesta Microsoft 365 Business Premiumiin 

Microsoft 365 Business Premiumissa on kaikki, mitä tarvitset pien yrityksellesi, yhdistämällä luokkansa parhaat pilvipohjaiset tuottavuus sovellukset yksinkertaiseen laitteiden hallintaan ja tieto turvaan. Jos sinulla on tällä hetkellä Office 365 E3-tilaus, mutta sinulla ei ole enempää kuin 300 työn tekijää, harkitse siirtymistä käyttämään Microsoft 365 Business Premiumia tieto turva ominaisuuksien lisäämiseen.

Siirtäminen on helppoa: ensin vaihdat käyttö oikeuksia ja kaikki tiedot ja käyttäjä tiedot nykyisessä paketilassasi säilytetään. Siirron jälkeen sinun on määritettävä Microsoft 365 Business Premiumiin lisätyt ominaisuudet.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Office 365 E3-ja Microsoft 365 Business Premium-erot

Tässä taulukossa esitellään Microsoft 365 Business Premiumin ja Office 365 E3-ohjelmien erot.

| Ominaisuus    | Microsoft 365 Business Premiumin tuki    | Office 365 E3-tuki | 
|:-------|:-----|:-----|
| **Paikallinen**        | | | 
| Office-sovellukset<sup>1</sup>    | Microsoft 365-sovellukset yrityksille    | Microsoft 365 -yrityssovellukset | 
| **Pilvi palveluiden tuottavuus sovellukset**        | | | 
| Exchange Online ja Outlook    | 50 gt tallennus tilan rajoitus posti laatikkoa kohden ja rajoittamaton Exchange Online-arkistointi    | 100 gt tallennus tilan rajoitus posti laatikkoa kohden ja rajoittamaton Exchange Online-arkistointi | 
| Teams    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3-pakettiin](../media/check-mark.png) | 
| OneDrive for Business    | 1 TERATAVUN tallennus tila raja käyttäjää kohden    | Rajoittamattomat | 
| Yammer, SharePoint Online, Planner, Streamin    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3-pakettiin](../media/check-mark.png) | 
| StaffHub    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3-pakettiin](../media/check-mark.png) | 
| Outlook Customer Managerilla, Mireiq    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | | 
| **Uhkien suojaus**        | | | 
| Office 365-paketin 1 Defender | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | Ei sisälly, mutta se voidaan lisätä | 
| **Tunniste tietojen hallinta**        | | | 
| Omatoiminen Sala sanan palautus yhdistelmä Azure Active Directory (Azure AD)-tileillä, Azure AD Multi-Factor-todennus (MFA), ehdollinen käyttö oikeus, Sala sanan palauttaminen paikallisille identiteeteille|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    |  | 
| **Laitteen ja sovellusten hallinta**        | | |
| Microsoft Intune, Windowsin AutoPilot|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    |  |
| Jaettujen tieto koneiden Akti vointi|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3-pakettiin](../media/check-mark.png)| 
| Windows 10 Pron päivitys oikeudet Win 7/8.1 Pro-käyttö oikeuksista|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    || 
| **Tieto turva**        | | |
|Office 365-tietojen menetyksen estäminen|    ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)|![Sisältyy Office 365 E3-pakettiin](../media/check-mark.png)|
|Azure Information Protectionin tieto turva sopimus 1, BitLocker-valvonta|![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)||
|Azuren tieto turva sopimus 1, herkkyys Tunnisteet|![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)||
|**Client Access License (CAL-käyttö oikeus)**|||
|Enterprise CAL-ohjelmisto paketti (Exchange, SharePoint, Skype)||![Sisältyy Office 365 E3-pakettiin](../media/check-mark.png)|

<sup>1</sup> Office-sovellusten Microsoft 365 Business Premium-versioon ei kuulu määrä Akti vointia ryhmä käytännöllä, sovellustelemetrialla, päivitys komponenteilla, laskenta taulukon vertailujen ja kysely-tai yritys tietojen avulla.

## <a name="migration"></a>Siirto

Jos haluat siirtää tila uksen, Katso ohjeet artikkelista palvelu [pakettien muuttaminen manuaalisesti](../commerce/subscriptions/change-plans-manually.md) , jotta voit siirtyä vain muutamasta henkilöstä Microsoft 365 Business Premiumiin. Voit myös [päivittää kaikki automaattisesti](../commerce/subscriptions/upgrade-to-different-plan.md)tai käyttää kumppania, jos haluat siirtää E3-tilauksesi ja käyttö oikeutesi Microsoft 365 Business Premium-tila ukseen.
Seuraavissa osissa kuvataan muutokset, jotka sinun on tehtävä ja mitä voit tehdä siirron jälkeen.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 E3-tila uksen määritykset ja tiedot
Sinun ei tarvitse tehdä muutoksia nykyiseen tilaukseesi tai tiedoihisi ennen siirtoa, joka sisältää seuraavat tiedot:

- Tila uksen määritykset, kuten DNS-tietueet ja toimi alue nimet.
- Käyttäjä-ja ryhmä tunnukset sekä todennus asetukset, kuten usean tekijän todentaminen tai ehdolliset käyttö oikeus käytännöt.
- Tuottavuus palvelu määritykset ja niiden tiedot, kuten tiimit, Exchange Online-posti laatikot, SharePoint Online-sivustot, OneDrive for Business-kansiot ja OneNote-muisti kirjat.
- Office-sovellukset skaalautuvat automaattisesti. Office 365 Modern Licensing tarkistaa käyttäjän käyttö oikeus Varauksen 72 tunnin välein ja muuntaa Office-sovellukset käyttäjän tilausta vastaavaksi versioksi.

### <a name="windows-10"></a>Windows 10

Jos Windows ei ole vielä Windows Pro Creator-päivityksessä, [Päivitä ne Windows Pro Creators](upgrade-to-windows-pro-creators-update.md)-päivitykseen.

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Käytäntöjen määrittäminen käyttäjien laitteiden ja tiedostojen suojaamiseksi

> [!NOTE]
> Jos määrität Office 365 MDM-käytännöt ja-laitteet, kyseiset laitteet näkyvät Microsoft 365-hallinta keskuksen **laitteet** -sivulla. Määrittämäsi käytännöt näkyvät perinteisten käytäntöjen luettelossa [Intune-portaalissa](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).

Kun olet määrittänyt käyttö oikeudet Microsoft 365 Business Premiumiin, voit aloittaa käyttäjien laitteiden ja tiedostojen suojaamisen.

Jos olet päivittänyt kaikki organisaatiosi käyttäjät Microsoft 365 Business Premiumiin, näet ohjatun määritys toiminnon aloitus sivulla ja voit suojata tiedostot ja mobiililaitteet noudattamalla [ohjattua määritys toimintoa microsoft 365 Business Premiumin määrittäminen](set-up.md) .

Voit suorittaa nämä vaiheet myös laitteet-sivulla:
  
1. Valitse hallinta keskuksen vasemmanpuoleisesta siirtymis ruudusta **laitteet** - \> **käytännöt**.
    
2. Valitse **laite käytännöt** -sivulla **Lisää**.
    
3. Anna käytännölle nimi **Lisää käytäntöä** -ruudussa ja valitse sitten avattavasta luettelosta haluamasi **käytäntöjen tyyppi** . 
    
     Voit määrittää sovellus käytäntöjä, jotka suojaavat tiedostoja Android-ja iPhone-laitteissa sekä Windows 10: ssä, ja voit määrittää laitteiden määritys käytäntöjä yrityksen omistamille Windows 10-laitteille. Lisä tietoja on seuraavissa linkeissä:
    
  - [Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten](app-protection-settings-for-android-and-ios.md)
    
  - [Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille](protection-settings-for-windows-10-devices.md)
    
  - [Laitteen suojaus asetusten määrittäminen Windows 10-tieto koneisiin](protection-settings-for-windows-10-pcs.md)
  
4. Kun olet määrittänyt käytännöt, sinä ja työn tekijäsi voitte määrittää laitteita:
    
  - Lisä tietoja on artikkelissa [Windows-laitteiden määrittäminen Microsoft 365 Business Premium-käyttäjille](set-up-windows-devices.md) Windows-laitteille. 
    
  - Lisä tietoja on artikkelissa [mobiililaitteiden määrittäminen Microsoft 365 Business Premium-käyttäjille](set-up-mobile-devices.md) Android-puhelimiin ja iPhoneja koskevia ohjeita varten. 
  
### <a name="mailbox-size"></a>Posti laatikon koko

Microsoft 365 Business Premiumin tallennus tila rajoitus on 50 gt, kun se käyttää Exchange Online-palvelu paketin 1. Vaikka Microsoft 365 Business Premiumiin siirryttäessä käyttäjät ylittäisivät 50 Giga tavua posti laatikon tallennus tilaa, on suositeltavaa, että määrität tämän käyttäjän Exchange Online-palvelu paketin 2 ja poistat Exchange Online-palvelu paketin 1, koska molempien määrittäminen ei ole mahdollista.


### <a name="threat-protection"></a>Uhkien suojaus

Kun olet muuttanut Microsoft 365 Business Premiumiin, sinulla on Office 365 Defender. Katso yleiskuvaus artikkelista [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) . Lisä tietoja on kohdassa [turvallisten linkkien](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)määrittäminen, [turvallisten liitteiden](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)määrittäminen ja [Tietojenkalastelutietojen määrittäminen Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)-sovelluksessa.

### <a name="sensitivity-labels"></a>Luottamuksellisuusmerkinnät

Jos haluat käyttää herkkyys otsikoita, katso [Yleiskatsaus herkkyys merkinnöistä](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) ja [Luo ja hallitse herkkyys otsikoita](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) -video.
