---
title: Siirtyminen Microsoft 365 Businessiin Office 365 E3:sta
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
description: Opi siirtämään yrityksesi Microsoft 365 Business Premiumiin Office 365 E3:sta.
ms.openlocfilehash: 3f9fd70b2d31b32027981e638de249d92e98ea08
ms.sourcegitcommit: 2a708650b7e30a53d10a2fe3164c6ed5ea37d868
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2021
ms.locfileid: "51164529"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Siirtyminen Office 365 E3:sta Microsoft 365 Business Premiumiin

Microsoft 365 Business Premium sisältää kaiken, mitä tarvitset pienyritystä varten yhdistämällä luokkansa parhaat pilvipohjaiset tuottavuussovellukset yksinkertaiseen laitehallintaan ja tietoturvaan. Jos sinulla on tällä hetkellä Office 365 E3 -tilaus, mutta yrityksessäsi ei ole yli 300 työntekijää, harkitse siirtymistä Microsoft 365 Business Premiumiin lisä suojausominaisuuksia varten.

Siirtyminen on helppoa: Ensin vaihdat käyttöoikeuksia, ja kaikki nykyisen tilauksesi tiedot ja käyttäjätiedot säilytetään. Siirron jälkeen sinun on määritettävä Microsoft 365 Business Premiumiin lisätyt ominaisuudet.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Office 365 E3:n ja Microsoft 365 Business Premiumin erot

Tässä taulukossa on esitetty Microsoft 365 Business Premiumin ja Office 365 E3:n väliset erot.

| Ominaisuus    | Microsoft 365 Business Premiumin tuki    | Tuki Office 365 E3:ssa | 
|:-------|:-----|:-----|
| **Paikallinen**        | | | 
| Office-sovellukset<sup>1</sup>    | Microsoft 365 -sovellukset yrityksille    | Microsoft 365 -sovellukset yrityksille | 
| **Pilvipalvelun tuottavuussovellukset**        | | | 
| Exchange Online ja Outlook    | 50 Gigatavun tallennustilaraja postilaatikkoa kohden ja rajoittamaton Exchange Online Archiving    | 100 Gigatavun tallennustilaraja postilaatikkoa kohden ja rajoittamaton Exchange Online Archiving | 
| Teams    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3-versioon](../media/check-mark.png) | 
| OneDrive for Business    | 1 Tt tallennustilaraja käyttäjää kohden    | Rajoittamaton | 
| Yammer, SharePoint Online, Planner, Stream    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3-versioon](../media/check-mark.png) | 
| StaffHub    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3-versioon](../media/check-mark.png) | 
| Outlook Customer Manager    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | | 
| **Threat Protection**        | | | 
| Defender for Office 365 Plan 1 | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | Ei sisälly, mutta se voidaan lisätä | 
| **Käyttäjätietojen hallinta**        | | | 
| Azure Active Directory (Azure AD) -yhdistelmätilien omatoiminen salasanan palautus, Azure AD:n monimenetelmäinen todentaminen (MFA), ehdollinen käyttöoikeus, paikallisen käyttäjäryhmän salasanan palautus|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    |  | 
| **Laitteiden ja sovellusten hallinta**        | | |
| Microsoft Intune, Windows AutoPilot|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    |  |
| Jaetun tietokoneen aktivointi|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3-versioon](../media/check-mark.png)| 
| Oikeuksien päivittäminen Windows 10 Proon Win 7/8.1 Pro -käyttöoikeuksista|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    || 
| **Tietojen suojaus**        | | |
|Office 365:n tietojen menetyksen estäminen|    ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)|![Sisältyy Office 365 E3-versioon](../media/check-mark.png)|
|Azure Information Protection Plan 1, Bitlocker-pakotus|![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)||
|Azure Information Protection Plan 1, luottamuksellisuusmerkinnät|![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)||
|**Client Access License (CAL-oikeudet)**|||
|Enterprise CAL Suite (Exchange, SharePoint, Skype)||![Sisältyy Office 365 E3-versioon](../media/check-mark.png)|

<sup>1</sup> Office-sovellusten Microsoft 365 Business Premium -versio ei sisällä volyymiaktivointia ryhmäkäytännön, sovelluksen telemetriatietojen, päivitysohjausobjektien, laskentataulukon vertailun ja kyselyn tai liiketoimintatietojen avulla.

## <a name="migration"></a>Siirto

Jos haluat siirtää [](../commerce/subscriptions/change-plans-manually.md) tilauksen, katso ohjeet microsoft 365 Business Premiumiin, jos haluat siirtää palvelupaketit manuaalisesti. Voit myös päivittää [kaikki automaattisesti tai](../commerce/subscriptions/upgrade-to-different-plan.md)siirtää E3-tilauksesi ja -käyttöoikeutesi Microsoft 365 Business Premium -tilaukseen yhdessä kumppanin kanssa.
Seuraavissa osissa kuvataan mahdolliset muutokset ja se, mitä voit tehdä siirron jälkeen.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 E3 -tilauksen määritykset ja tiedot
Sinun ei tarvitse tehdä muutoksia nykyiseen tilaukseesi tai tietoihin ennen sen muutosta, joka sisältää seuraavat:

- Tilausmääritykset, kuten DNS-tietueet ja toimialuenimet.
- Käyttäjä- ja ryhmätilit ja todennusasetukset, kuten monimenetelmäinen todentaminen tai ehdollisten käyttöoikeuksien käytännöt.
- Tuottavuuspalvelun määritykset ja niiden tiedot, kuten Teams, Exchange Online -postilaatikot, SharePoint Online -sivustot, OneDrive for Business -kansiot ja OneNote-muistikirjat.
- Office-sovellukset skaalataan automaattisesti. Office 365:n modernit käyttöoikeudet tarkistavat käyttäjän käyttöoikeuksien määrityksen 72 tunnin välein ja muuntavat Office-sovellukset käyttäjän tilausta vastaavaksi versioksi.

### <a name="windows-10"></a>Windows 10

Jos Windows ei ole vielä Windows Pro Creator -päivityksessä, [päivitä ne Windows Pro Creators -päivitykseen.](upgrade-to-windows-pro-creators-update.md)

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Käyttäjien laitteiden ja tiedostojen suojaamista kuvaavat käytännöt

> [!NOTE]
> Jos määrität Office 365:n mobiililaitteiden hallintakäytännöt ja  -laitteet, kyseiset laitteet näkyvät Microsoft 365 -hallintakeskuksen Laitteet-sivulla. Kaikki määrittämäsi käytännöt näkyvät [Intune-portaalin perinteisen käytännöt -luettelossa.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)

Kun olet määrittänyt käyttöoikeudet Microsoft 365 Business Premiumiin, voit alkaa suojata käyttäjien laitteita ja tiedostoja.

Jos olet päivittänyt kaikki organisaatiosi käyttäjät Microsoft 365 Business Premiumiin, näet ohjatun määritystoiminnon aloitussivulla ja voit suojata tiedostoja ja mobiililaitteita ohjatun määritystoiminnon ohjeiden mukaisesti. [](set-up.md)

Voit myös suorittaa nämä vaiheet Laitteet-sivulla:
  
1. Siirry hallintakeskuksen vasemmassa siirtymispalkin **Laitekäytännöt-ryhmässä.** \> 
    
2. Valitse **Laitekäytännöt-sivulla** **Lisää.**
    
3. Anna **käytännön nimi** Lisää käytäntö -ruudussa ja valitse sitten **käytäntötyyppi** avattavasta luettelosta. 
    
     Voit määrittää sovelluskäytäntöjä android- ja iPhone-laitteiden sekä Windows 10:n tiedostojen suojaamista varten ja määrittää laitemäärityskäytännöt yrityksen omistamia Windows 10 -laitteita varten. Lisätietoja on seuraavissa linkeissä:
    
  - [Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten](app-protection-settings-for-android-and-ios.md)
    
  - [Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille](protection-settings-for-windows-10-devices.md)
    
  - [Laitesuojausasetusten määrittäminen Windows 10 -tietokoneisiin](protection-settings-for-windows-10-pcs.md)
  
4. Kun olet määrittänyt käytäntöjä, sinä ja työntekijäsi voitte määrittää laitteita:
    
  - Katso [Windows-laitteiden ohjeet Microsoft 365 Business Premium](set-up-windows-devices.md) -käyttäjien Windows-laitteiden määritäminen -ohjeista. 
    
  - Ohjeita [Android-puhelimiin ja iPhone-puhelimiin](set-up-mobile-devices.md) on kohdassa Mobiililaitteiden määritäminen Microsoft 365 Business Premium -käyttäjille. 
  
### <a name="mailbox-size"></a>Postilaatikon koko

Microsoft 365 Business Premiumin tallennustilaraja on 50 Gigatavua, koska se käyttää Exchange Online -palvelupakettia 1. Microsoft 365 Business Premiumiin vaihdon aikana on suositeltavaa määrittää käyttäjälle Exchange Online -palvelupaketti 2 ja poistaa Exchange Online -palvelupaketti 1, sillä molempia ei voi määrittää.


### <a name="threat-protection"></a>Uhkien torjunta

Kun olet siirtyminen Microsoft 365 Business Premiumiin, sinulla on Defender for Office 365. Katso [yleistietoja Microsoft Defender for Office 365:stä.](../security/defender-365-security/defender-for-office-365.md) Lisätietoja on ohjeaiheessa Turvallisten linkkien [määritys,](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)turvallisten liitteiden määritys ja [tietojenkalastelun](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)torjunnan määritys [Defender for Office 365:ssä.](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)

### <a name="sensitivity-labels"></a>Luottamuksellisuusmerkinnät

Lisätietoja luottamuksellisuusotsikoiden käyttämisestä on ohjeaiheessa [Luottamuksellisuusotsikoiden yleiskatsaus](../compliance/sensitivity-labels.md) sekä luottamuksellisuusotsikoiden luominen [ja](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) hallinta videossa.
