---
title: Siirtyminen Microsoft 365 Businessiin Office 365 E3:sta
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
search.appverid:
- BCS160
- MET150
description: Opi siirtämään yrityksesi Microsoft 365 Business Premiumiin Office 365 E3:sta.
ms.openlocfilehash: f2b7962918186f4a1063c5a66596135c2972ec71
ms.sourcegitcommit: 07dea2aa98daf0c4086f8590375167830027c802
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/13/2021
ms.locfileid: "51749996"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Siirtyminen Office 365 E3:sta Microsoft 365 Business Premiumiin

Microsoft 365 Business Premium sisältää kaiken, mitä tarvitset pienyritystäsi varten yhdistämällä luokkansa parhaat pilvipohjaiset tuottavuussovellukset yksinkertaiseen laitehallintaan ja tietoturvaan. Jos sinulla on tällä hetkellä Office 365 E3 -tilaus, mutta yrityksessäsi ei ole yli 300 työntekijää, voit siirtyä Microsoft 365 Business Premiumiin suojausominaisuuksien lisäominaisuuksia varten.

Siirtyminen on helppoa: Ensin vaihdat käyttöoikeuksia, ja kaikki nykyisen tilauksesi tiedot ja käyttäjätiedot säilytetään. Siirron jälkeen sinun on määritettävä Microsoft 365 Business Premiumiin lisätyt ominaisuudet.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Office 365 E3:n ja Microsoft 365 Business Premiumin erot

Tässä taulukossa on esitetty Microsoft 365 Business Premiumin ja Office 365 E3:n väliset erot.

| Ominaisuus    | Microsoft 365 Business Premiumin tuki    | Tuki Office 365 E3:ssa | 
|:-------|:-----|:-----|
| **Paikallinen**        | | | 
| Office-sovellukset<sup>1</sup>    | Microsoft 365 -sovellukset yrityksille    | Microsoft 365 -sovellukset yrityksille | 
| **Pilvitallennussovellukset**        | | | 
| Exchange Online ja Outlook    | 50 gigatavun tallennustilaraja postilaatikkoa kohden ja rajoittamaton Exchange Online Archiving    | 100 Gigatavun tallennustilaraja postilaatikkoa kohden ja rajoittamaton Exchange Online Archiving | 
| Teams    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:lle](../media/check-mark.png) | 
| OneDrive for Business    | 1 Tt tallennustilaraja käyttäjää kohden    | Rajoittamaton | 
| Yammer, SharePoint Online, Planner, Stream    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:lle](../media/check-mark.png) | 
| StaffHub    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:lle](../media/check-mark.png) | 
| MileIQ    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | | 
| **Threat Protection**        | | | 
| Defender for Office 365 Plan 1 | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | Ei sisälly, mutta voidaan lisätä | 
| **Käyttäjätietojen hallinta**        | | | 
| Azure Active Directory (Azure AD) -yhdistelmätilien omatoiminen salasanan palautus, Azure AD:n monimenetelmäinen todentaminen (MFA), ehdollinen käyttöoikeus, paikallisen käyttäjätiedot salasanalla kirjoitettavan salasanan palautus|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    |  | 
| **Laite- ja sovellushallinta**        | | |
| Microsoft Intune, Windows AutoPilot|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    |  |
| Jaetun tietokoneen aktivointi|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:lle](../media/check-mark.png)| 
| Oikeuksien päivittäminen Windows 10 Pro -käyttöoikeuteen Win 7/8.1 Pro -käyttöoikeuksista|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    || 
| **Tietojen suojaus**        | | |
|Office 365:n tietojen menetyksen estäminen|    ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)|![Sisältyy Office 365 E3:lle](../media/check-mark.png)|
|Azure Information Protection Plan 1, BitLocker-pakotus|![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)||
|Azure Information Protection Plan 1, luottamuksellisuusmerkinnät|![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)||
|**Client Access License (CAL-oikeudet)**|||
|Enterprise CAL Suite (Exchange, SharePoint, Skype)||![Sisältyy Office 365 E3:lle](../media/check-mark.png)|

<sup>1</sup> Office-sovellusten Microsoft 365 Business Premium -versio ei sisällä volyymiaktivoinnin ryhmäkäytännön, sovellustelemetrian, päivitysohjausobjektien, laskentataulukon vertailun ja kyselyn tai liiketoimintatietojen kautta.

## <a name="migration"></a>Siirto

Jos haluat siirtää tilauksesi, [katso](../commerce/subscriptions/change-plans-manually.md) ohjeet palvelupaketit manuaalisesti, jos haluat siirtää vain muutamia henkilöitä Microsoft 365 Business Premiumiin. Voit myös päivittää [kaikki automaattisesti tai](../commerce/subscriptions/upgrade-to-different-plan.md)siirtää E3-tilauksesi ja -käyttöoikeutesi Microsoft 365 Business Premium -tilaukseen kumppanin kanssa.
Seuraavissa osissa kuvataan, mitä muutoksia on tehtävä (jos niitä on) ja mitä voit tehdä siirron jälkeen.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 E3 -tilauksen määritys ja tiedot
Sinun ei tarvitse tehdä muutoksia nykyiseen tilaukseesi tai tietoihin ennen sen muutosta, joka sisältää seuraavat:

- Tilausmääritykset, kuten DNS-tietueet ja toimialuenimet.
- Käyttäjä- ja ryhmätilit ja todentamisasetukset, kuten monimenetelmäinen todentaminen tai ehdolliset käyttöoikeuskäytännöt.
- Tuottavuuspalvelun määritykset ja niiden tiedot, kuten Teams, Exchange Online -postilaatikot, SharePoint Online -sivustot, OneDrive for Business -kansiot ja OneNote-muistikirjat.
- Office-sovellukset skaalataan automaattisesti. Office 365:n modernit käyttöoikeudet tarkistavat käyttäjän käyttöoikeusmäärityksen 72 tunnin välein ja muuntaa Office-sovellukset käyttäjän tilausta vastaavaksi versioksi.

### <a name="windows-10"></a>Windows 10

Jos Windows ei ole vielä Windows Pro Creator -päivityksessä, [päivitä ne Windows Pro Creators -päivitykseen.](upgrade-to-windows-pro-creators-update.md)

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Käyttäjien laitteiden ja tiedostojen suojaamista varten määritettyjen käytäntöjä

> [!NOTE]
> Jos määrität Office 365:n mobiililaitteiden hallintakäytännöt ja  -laitteet, kyseiset laitteet näkyvät Laitteet-sivulla Microsoft 365 -hallintakeskuksessa. Kaikki määrittämäsi käytännöt näkyvät Intune-portaalin perinteiset [käytännöt -luettelossa.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)

Kun olet määrittänyt käyttöoikeudet Microsoft 365 Business Premiumiin, voit alkaa suojata käyttäjien laitteita ja tiedostoja.

Jos olet päivittänyt kaikki organisaation käyttäjät Microsoft 365 Business Premiumiin, näet ohjatun määritystoiminnon aloitussivulla ja voit suojata tiedostoja ja mobiililaitteita ohjatun määritystoiminnon ohjeiden mukaisesti Microsoft [365 Business Premiumin](set-up.md) määrittäminen.

Voit myös suorittaa nämä vaiheet Laitteet-sivulla:
  
1. Valitse hallintakeskuksen vasemmassa siirtymispalkin **laitekäytännöt** \> .
    
2. Valitse **Laitekäytännöt-sivulla** **Lisää**.
    
3. Anna **käytännön nimi** Lisää käytäntö -ruudussa ja valitse sitten **käytäntötyyppi** avattavasta luettelosta. 
    
     Voit määrittää sovelluskäytäntöjä Android- ja iPhone-laitteiden sekä Windows 10:n tiedostojen suojaamista varten ja määrittää laitemäärityskäytännöt yrityksen omistamia Windows 10 -laitteita varten. Lisätietoja on seuraavissa linkeissä:
    
  - [Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten](app-protection-settings-for-android-and-ios.md)
    
  - [Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille](protection-settings-for-windows-10-devices.md)
    
  - [Laitteiden suojausasetusten määrittäminen Windows 10 -tietokoneille](protection-settings-for-windows-10-pcs.md)
  
4. Kun olet määrittänyt käytännöt, sinä ja työntekijäsi voitte määrittää laitteita:
    
  - Ohjeet [Windows-laitteille ovat kohdassa Windows-laitteiden asennus Microsoft 365 Business Premium](set-up-windows-devices.md) -käyttäjille. 
    
  - Ohjeita [Android-puhelimiin ja iPhone-puhelimiin](set-up-mobile-devices.md) on kohdassa Mobiililaitteiden määritäminen Microsoft 365 Business Premium -käyttäjille. 
  
### <a name="mailbox-size"></a>Postilaatikon koko

Microsoft 365 Business Premiumin tallennustilaraja on 50 gigatavua, sillä se käyttää Exchange Online -palvelupakettia 1. Kun siirto Microsoft 365 Business Premiumiin on suositeltavaa, että joku käyttäjistä ylittää 50 Gt postilaatikon tallennustilaa, on suositeltavaa määrittää käyttäjälle Exchange Online -palvelupaketti 2 ja poistaa Exchange Online -palvelupaketti 1, koska molempia ei voi määrittää.


### <a name="threat-protection"></a>Uhkien suojaus

Kun olet siirtyminen Microsoft 365 Business Premiumiin, sinulla on Defender for Office 365. Tutustu [yleiskatsaukseen microsoft Defender for Office 365:ssä.](../security/office-365-security/defender-for-office-365.md) Lisätietoja on kohdassa [Turvallisten](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)linkkien määritys , Turvallisten liitteiden määritys ja [Tietojenkalastelun](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)esto -määritys [Office 365:n Defenderissä.](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)

### <a name="sensitivity-labels"></a>Luottamuksellisuusmerkinnät

Jos haluat aloittaa luottamuksellisuusotsikoiden käytön, katso [Luottamuksellisuusotsikoiden yleiskatsaus](../compliance/sensitivity-labels.md) ja [luo ja hallitse luottamuksellisuusotsikoiden](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) videota.
