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
description: Lue tietoja siitä, miten voit siirtää yrityksesi Microsoft 365 Business Premiumiin Office 365 E3:sta.
ms.openlocfilehash: d72f0c52a745ff973868b6fdaa95efa1a37a3dbd
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/18/2020
ms.locfileid: "45081812"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Siirtyminen Office 365 E3:sta Microsoft 365 Business Premiumiin 

Microsoft 365 Business Premiumissa on kaikki mitä tarvitset pienyrityksellesi, ja siinä yhdistyvät luokkansa parhaat pilvipohjaiset tuottavuussovellukset sekä yksinkertainen laitehallinta ja -suojaus. Jos sinulla on tällä hetkellä Office 365 E3 -tilaus, mutta sinulla ei ole enempää kuin 300 työntekijää, harkitse siirtymistä Microsoft 365 Business Premiumiin lisäsuojausominaisuuksien saamiseksi.

Siirtäminen on helppoa: Ensin vaihdat käyttöoikeuksia ja kaikki nykyisen tilauksesi tiedot ja käyttäjätiedot säilytetään. Siirron jälkeen sinun on määritettävä Microsoft 365 Business Premiumiin lisätyt ominaisuudet.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Erot Office 365 E3:n ja Microsoft 365 Business Premiumin välillä

Tässä taulukossa esitetään Microsoft 365 Business Premiumin ja Office 365 E3:n väliset erot.

| Ominaisuus    | Microsoft 365 Business Premiumin tuki    | Office 365 E3:n tuki | 
|:-------|:-----|:-----|
| **Paikallinen**        | | | 
| Office-sovellukset<sup>1</sup>    | Microsoft 365 -sovellukset yrityksille    | Microsoft 365 -sovellukset yrityksille | 
| **Pilvituottavuussovellukset**        | | | 
| Exchange Online ja Outlook    | 50 Gt:n tallennustilarajoitus postilaatikkoa kohden ja rajoittamaton Exchange Online -arkistointi    | 100 Gt:n tallennustilarajoitus postilaatikkoa kohden ja rajoittamaton Exchange Online -arkistointi | 
| Joukkueet    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:een](../media/check-mark.png) | 
| OneDrive for Business    | 1 Tt:n tallennusraja käyttäjää kohden    | Rajoittamaton | 
| Yammer, SharePoint Online, Suunnittelija, Stream    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:een](../media/check-mark.png) | 
| HenkilökuntaHub    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:een](../media/check-mark.png) | 
| Outlook-asiakaspäällikkö, MileIQ    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | | 
| **Uhkien torjunta**        | | | 
| Office 365 Advanced Threat Protection (ATP) -palvelupaketti 1 | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | Ei sisälly, mutta voidaan lisätä | 
| **Identiteetin hallinta**        | | | 
| Azure Active Directory (Azure AD) -hybriditilien, Azure multi-factor-todennuksen (MFA), ehdollisen käytön, paikallisten käyttäjätietojen salasanan takaisinkutsun oletusasetusten palauttaminen|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    |  | 
| **Laite- ja sovellushallinta**        | | |
| Microsoft Intune, Windowsin automaattiohjaus|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    |  |
| Jaetun tietokoneen aktivointi|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Office 365 E3:een](../media/check-mark.png)| 
| Windows 10 Pron päivitysoikeudet Win 7/8.1 Pro -käyttöoikeuksista|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    || 
| **Tietojen suojaaminen**        | | |
|Office 365:n tietojen menetyksen estäminen|    ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)|![Sisältyy Office 365 E3:een](../media/check-mark.png)|
|Azure Information Protection Plan 1, Bitlocker-valvonta|![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)||
|Azure Information Protection Plan 1, Herkkyysmerkinnät|![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)||
|**Client Access License (CAL-käyttöoikeudet)**|||
|Enterprise CAL Suite (Exchange, SharePoint, Skype)||![Sisältyy Office 365 E3:een](../media/check-mark.png)|

<sup>1</sup> Office-sovellusten Microsoft 365 Business Premium -versio ei sisällä volyymiaktivointia ryhmäkäytännön, sovellustelemetrian, päivitysohjausobjektien, laskentataulukoiden vertailun ja kyselyjen tai yritystietojen avulla.

## <a name="migration"></a>Siirron

Lisätietoja tilauksen siirtämisestä on [ohjeaiheessa Palvelupakettien muuttaminen manuaalisesti,](../commerce/subscriptions/change-plans-manually.md) jos haluat siirtää vain muutaman henkilön Microsoft 365 Business Premiumiin. Voit myös [päivittää kaikki automaattisesti](../commerce/subscriptions/upgrade-to-different-plan.md)tai siirtää E3-tilauksesi ja -käyttöoikeutesi Microsoft 365 Business Premium -tilaukseen yhteistyössä kumppanin kanssa.
Seuraavissa osissa kuvataan muutokset, jotka sinun on tehtävä, jos sellaisia on, ja mitä voit tehdä siirron jälkeen.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 E3 -tilauksen määritys ja tiedot
Sinun ei tarvitse tehdä muutoksia nykyiseen tilaukseesi tai tietoihin ennen siirtämistä, joka sisältää:

- Tilauksen määritykset, kuten DNS-tietueet ja toimialuenimet.
- Käyttäjä- ja ryhmätilit ja todennusasetukset, kuten monivaiheinen todennus tai ehdollisen käytön käytännöt.
- Tuottavuuspalvelun määritykset ja niiden tiedot, kuten Teams, Exchange Online -postilaatikot, SharePoint Online -sivustot, OneDrive for Business -kansiot ja OneNote-muistikirjat.
- Office-sovellukset skaalautuvat automaattisesti. Office 365:n nykyaikaiset käyttöoikeudet tarkistavat käyttäjän käyttöoikeusmäärityksen 72 tunnin välein ja muuntavat Office-sovellukset käyttäjätilausta vastaavaksi versioksi.

### <a name="windows-10"></a>Windows 10

Jos Windows ei ole vielä Windows Pro Creator -päivityksessä, [päivitä ne Windows Pro Creators -päivitykseen](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Käyttäjälaitteiden ja tiedostojen suojaaminen käytäntöjen määrittäminen

> [!NOTE]
> Jos määrität Office 365:n MDM-käytännöt ja -laitteet, nämä laitteet näkyvät Microsoft 365 -hallintakeskuksen **Laitteet-sivulla.** Kaikki määrittämäsi käytännöt näkyvät [Intune-portaalin](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)klassisten käytäntöjen luettelossa.

Kun olet määrittänyt käyttöoikeudet Microsoft 365 Business Premiumiin, voit alkaa suojata käyttäjien laitteita ja tiedostoja.

Jos olet päivittänyt kaikki organisaation jäsenet Microsoft 365 Business Premiumiin, näet ohjatun asennustoiminnon kotisivulla ja voit suojata tiedostoja ja mobiililaitteita [noudattamalla Ohjatun asennustoiminnon ohjatun asennustoiminnon](set-up.md) määritystoimintoa.

Voit suorittaa nämä vaiheet myös Laitteet-sivulla:
  
1. Siirry hallintakeskuksen vasemmassa siirtymisruudussa **Devices** \> **Laitekäytännöt -kohtaan**.
    
2. Valitse **Laitekäytännöt-sivulla** **Lisää**.
    
3. Anna **lisää käytäntö** -ruudussa käytännön nimi ja valitse sitten avattavasta valikosta **käytäntötyyppi.** 
    
     Voit määrittää sovelluskäytännöt tiedostojen suojaamiseksi Android- ja iPhone-laitteissa sekä Windows 10:ssä ja voit määrittää laitteen määrityskäytännöt yrityksen omistamille Windows 10 -laitteille. Lisätietoja on seuraavissa linkeissä:
    
  - [Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten](app-protection-settings-for-android-and-ios.md)
    
  - [Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille](protection-settings-for-windows-10-devices.md)
    
  - [Laitteen suojausasetusten määrittäminen Windows 10 -tietokoneille](protection-settings-for-windows-10-pcs.md)
  
4. Kun olet määrittänyt käytännöt, sinä ja työntekijäsi voitte määrittää laitteita:
    
  - Lisätietoja Windows-laitteiden vaiheista [on ohjeaiheessa Windows-laitteiden määrittäminen Microsoft 365 Business Premium -käyttäjille.](set-up-windows-devices.md) 
    
  - Lisätietoja Android-puhelimista ja iPhoneista on ohjeaiheessa [Mobiililaitteiden määrittäminen Microsoft 365 Business Premium -käyttäjille.](set-up-mobile-devices.md) 

### <a name="threat-protection"></a>Uhkien torjunta

Kun olet siirtynyt Microsoft 365 Business Premiumiin, sinulla on Office 365 ATP. Yleiskatsaus on [kohdassa Office 365 ATP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) Lisätietoja on ohjeaiheessa [ATP-turvallisten linkkien määrittäminen](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [ATP:n turvallisten liitteiden määrittäminen](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)ja [ATP-tietojenkalastelun torjunta](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).

### <a name="sensitivity-labels"></a>Luottamuksellisuusmerkinnät

Lisätietoja herkkyystarrojen käyttämisestä on [ohjeaiheessa Herkkyystarrojen yleiskatsaus](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) sekä [herkkyysmerkintöjen](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) videon luominen ja hallinta.
