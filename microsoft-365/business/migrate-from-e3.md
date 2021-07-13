---
title: Siirtyminen Microsoft 365 Business -Office 365 E3
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
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
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
description: Jos sinulla on Office 365 E3 tilaus, mutta yrityksessä on enintään 300 työntekijää, harkitse siirtymistä Microsoft 365 Business Premium.
ms.openlocfilehash: c1b4da07b3bf28cce1a48424ab45cde6ea54d367
ms.sourcegitcommit: 00f001019c653269d85718d410f970887d904304
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/12/2021
ms.locfileid: "53394167"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Siirtyminen Office 365 E3 Microsoft 365 Business Premium

Microsoft 365 Business Premium sisältää kaiken pienyritystäsi varten yhdistämällä luokkansa parhaat pilvipohjaiset tuottavuussovellukset yksinkertaiseen laitehallintaan ja tietoturvaan. Jos sinulla on Office 365 E3 tilaus, mutta yrityksessä on enintään 300 työntekijää, harkitse siirtymistä Microsoft 365 Business Premium suojausominaisuuksia varten.

Siirtyminen on helppoa: Ensin vaihdat käyttöoikeuksia, ja kaikki nykyisen tilauksesi tiedot ja käyttäjätiedot säilytetään. Siirron jälkeen sinun on määritettävä toiminnot, jotka lisätään Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Erot Office 365 E3 ja Microsoft 365 Business Premium

Tässä taulukossa on esitetty Microsoft 365 Business Premium ja Office 365 E3.

| Ominaisuus    | Tuki Microsoft 365 Business Premium    | Tuki Office 365 E3 |
|:-------|:-----|:-----|
| **Paikallinen**        | | |
| Office sovellukset<sup>1</sup>    | Microsoft 365 -sovellukset yrityksille    | Microsoft 365 -sovellukset yrityksille |
| **Pilvitallennussovellukset**        | | |
| Exchange Online ja Outlook    | Postilaatikkokohtainen 50 gigatavun tallennustilaraja ja rajoittamaton Exchange Online Archiving    | 100 Gigatavun tallennustilaraja postilaatikkoa kohden ja rajoittamaton Exchange Online Archiving |
| Teams    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Office 365 E3](../media/check-mark.png) | 
| OneDrive for Business    | 1 Tt tallennustilaraja käyttäjää kohden    | Rajoittamaton | 
| Yammer, SharePoint Online, Planner, Stream    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Office 365 E3](../media/check-mark.png) | 
| StaffHub    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Office 365 E3](../media/check-mark.png) |
| **Threat Protection**        | | |
| Defender for Office 365 Plan 1 | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | Ei sisälly, mutta voidaan lisätä |
| **Käyttäjätietojen hallinta**        | | |
| Omatoiminen salasanan vaihtaminen yhdistelmäympäristön Azure Active Directory (Azure AD) -tileissä, Azure AD:n monimenetelmäinen todentaminen (MFA), ehdollinen käyttöoikeus, paikallisen käyttäjätiedot salasanalla kirjoittamisen palautus|     ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| **Laite- ja sovellushallinta**        | | |
| Microsoft Intune, Windows AutoPilot|     ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| Jaetun tietokoneen aktivointi|     ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Office 365 E3](../media/check-mark.png)| 
| Päivitä käyttöoikeudet Windows 10 Pro Win 7/8.1 -Pro käyttöoikeuksista|     ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    ||
| **Tietojen suojaus**        | | |
|Office 365 Tietojen menetyksen estäminen|    ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)|![Sisältyy Office 365 E3](../media/check-mark.png)|
|Azure Information Protection Plan 1, BitLocker-pakotus|![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)||
|Azure Information Protection Plan 1, luottamuksellisuusmerkinnät|![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)||
|**Client Access License (CAL-oikeudet)**|||
|Enterprise CAL Suite (Exchange, SharePoint, Skype)||![Sisältyy Office 365 E3](../media/check-mark.png)|

<sup>1</sup> Microsoft 365 Business Premium-sovellusten Office ei sisällä volyymiaktivoinnin ryhmäkäytännön, sovelluksen telemetriatietojen, päivitysohjausobjektien, laskentataulukon vertailun ja kyselyn tai liiketoimintatietojen kautta.

## <a name="migration"></a>Siirto

Jos haluat siirtää tilauksen, katso ohjeet [tilauksen](../commerce/subscriptions/change-plans-manually.md) manuaaliseen Microsoft 365 Business Premium. Voit myös päivittää [kaikki automaattisesti tai](../commerce/subscriptions/upgrade-to-different-plan.md)siirtää E3-tilauksesi ja -käyttöoikeutesi kumppanin kanssa Microsoft 365 Business Premium tilaukseen.
Seuraavissa osissa kuvataan, mitä muutoksia on tehtävä (jos niitä on) ja mitä voit tehdä siirron jälkeen.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 E3 määrittäminen ja tiedot
Sinun ei tarvitse tehdä muutoksia nykyiseen tilaukseesi tai tietoihin ennen sen muutosta, joka sisältää seuraavat:

- Tilausmääritykset, kuten DNS-tietueet ja toimialuenimet.
- Käyttäjä- ja ryhmätilit ja todentamisasetukset, kuten monimenetelmäinen todentaminen tai ehdolliset käyttöoikeuskäytännöt.
- Tuottavuuspalvelun määritykset ja niiden tiedot, kuten Teams, Exchange Online postilaatikot, SharePoint online-sivustot, OneDrive for Business kansiot OneNote muistikirjat.
- Office skaalataan automaattisesti. Office 365 modernit käyttöoikeudet tarkistavat käyttäjän käyttöoikeusmäärityksen 72 tunnin välein ja muuntaa Office-sovellukset käyttäjän tilausta vastaavaksi versioksi.

### <a name="windows-10"></a>Windows 10

Jos Windows ei ole vielä Windows Pro Creator -päivityksessä, päivitä ne Windows Pro [Creators -päivitykseen.](upgrade-to-windows-pro-creators-update.md)

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Käyttäjien laitteiden ja tiedostojen suojaamista varten määritettyjen käytäntöjä

> [!NOTE]
> Jos määrität Office 365 mobiililaitteiden hallintakäytännöt ja -laitteet, kyseiset  laitteet näkyvät Laitteet-sivun Microsoft 365 -hallintakeskus. Kaikki määrittämäsi käytännöt näkyvät Intune-portaalin perinteiset [käytännöt -luettelossa.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)

Kun olet määrittänyt käyttöoikeudet Microsoft 365 Business Premium, voit alkaa suojata käyttäjien laitteita ja tiedostoja.

Jos olet päivittänyt kaikki organisaation käyttäjät Microsoft 365 Business Premium, näet ohjatun määritystoiminnon aloitussivulla ja voit suojata tiedostoja ja mobiililaitteita ohjatun [Microsoft 365 Business Premium](set-up.md) määritystoiminnon määritysvaiheiden mukaisesti.

Voit myös suorittaa nämä vaiheet Laitteet-sivulla:
  
1. Valitse hallintakeskuksen vasemmassa siirtymispalkin **laitekäytännöt** \> .

2. Valitse **Laitekäytännöt-sivulla** **Lisää**.

3. Anna **käytännön nimi** Lisää käytäntö -ruudussa ja valitse sitten **käytäntötyyppi** avattavasta luettelosta.

     Voit määrittää sovelluskäytäntöjä Android- ja iPhone-laitteissa sekä Windows 10-laitteissa olevien tiedostojen suojaamista varten sekä määrittää laitemäärityskäytännöt yrityksen omistamia Windows 10 laitteita varten. Lisätietoja on seuraavissa linkeissä:

  - [Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten](app-protection-settings-for-android-and-ios.md)

  - [Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille](protection-settings-for-windows-10-devices.md)

  - [Laitteiden suojausasetusten määrittäminen Windows 10 tietokoneisiin](protection-settings-for-windows-10-pcs.md)
  
4. Kun olet määrittänyt käytännöt, sinä ja työntekijäsi voitte määrittää laitteita:

  - Katso [ohjeet Windows laitteiden Microsoft 365 Business Premium käyttäjille](set-up-windows-devices.md) Windows varten. 

  - Katso [ohjeet Android-puhelimiin ja iPhoneen Microsoft 365 Business Premium](set-up-mobile-devices.md) mobiililaitteiden Microsoft 365 Business Premium mobiililaitteille. 
  
### <a name="mailbox-size"></a>Postilaatikon koko

Microsoft 365 Business Premium tallennustilaraja on 50 gigatavua, sillä se käyttää Exchange Online 1:tä. Kun siirto Microsoft 365 Business Premium:lle ja joku käyttäjistä ylittää 50 Gt postilaatikon tallennustilaa, on suositeltavaa määrittää tälle käyttäjälle Exchange Online -käyttöoikeuspaketti 2 ja poistaa Exchange Online -käyttöoikeuspaketti 1, koska molempia ei voi määrittää.

### <a name="threat-protection"></a>Uhkien suojaus

Kun olet Microsoft 365 Business Premium, sinulla on Defender for Office 365. Tutustu [yleiskatsaukseen Office 365 Microsoft Defender for](../security/office-365-security/defender-for-office-365.md) Office 365. Lisätietoja on ohjeaiheessa [Lokero](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)linkkien Lokero ja [tietojenkalastelun](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5) [torjunnan](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)Office 365.

### <a name="sensitivity-labels"></a>Luottamuksellisuusmerkinnät

Jos haluat aloittaa luottamuksellisuusotsikoiden käytön, katso [Luottamuksellisuusotsikoiden yleiskatsaus](../compliance/sensitivity-labels.md) ja [luo ja hallitse luottamuksellisuusotsikoiden](../business-video/create-sensitivity-labels.md) videota.

## <a name="related-content"></a>Aiheeseen liittyvä sisältö

[Palvelusuunnitelmien muuttaminen manuaalisesti](../commerce/subscriptions/change-plans-manually.md) (artikkeli)\
[Päivitä Windows -Windows 10 Pro](upgrade-to-windows-pro-creators-update.md) (video)\
[Android- tai iOS-laitteiden sovellusten suojausasetusten määrittäminen](app-protection-settings-for-android-and-ios.md) (artikkeli)\
[Sovellusten suojausasetusten määrittäminen tai muokkaaminen Windows 10 laitteissa](protection-settings-for-windows-10-devices.md) (artikkeli)\
[]

