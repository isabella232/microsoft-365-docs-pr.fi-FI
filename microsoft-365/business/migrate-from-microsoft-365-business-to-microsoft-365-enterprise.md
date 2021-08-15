---
title: Siirtyminen Microsoft 365 Businessista Microsoft 365 E3
f1.keywords:
- NOCSH
ms.author: josephd
author: JoeDavies-MSFT
manager: laurawi
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Opi siirtämään yrityksesi Microsoft 365 Business Premium Microsoft 365 E3.
ms.openlocfilehash: d3030518f7f4467c7b2e16897dc7b100764d9d5a36c50169b58f1adcd7bef209
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53837629"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Siirtyminen Microsoft 365 Business Premium Microsoft 365 E3

Microsoft 365 Business Premium sisältää kaiken pienyritystäsi varten yhdistämällä luokkansa parhaat pilvipohjaiset tuottavuussovellukset yksinkertaiseen laitehallintaan ja tietoturvaan, joiden avulla työntekijät voivat tehdä parasta työtään. Joissakin tapauksissa sinun on kuitenkin ehkä siirrettävä Microsoft 365 Business Premium tilaus Microsoft 365 E3.

Yrityksesi on esimerkiksi kasvanut ja tarvitsee yli 300 käyttöoikeutta (onneksi olkoon).

Yrityksesi tarvitsee myös yrityksen ominaisuuksia, kuten Microsoft 365 -sovellukset suuryrityksille, Windows 10 Enterprise E3- tai Enterprise Client Access -käyttöoikeuksia (CALs).

Päivittäminen on helppoa: voit käynnistää [päivityksen hallintakeskuksesta.](../commerce/subscriptions/upgrade-to-different-plan.md) Kaikki nykyisen tilauksesi tiedot ja määritykset säilytetään. Sinun ei tarvitse valmistautua siirtoon eikä tehdä mitään sen jälkeen, paitsi hyödyntää uusia ominaisuuksia.

> [!NOTE]
> Voit myös käyttää Microsoft 365 Business Premium enintään 300 käyttöpaikkaa ja saada Microsoft 365 E3 tilauksen yli 300 käyttöpaikkaa varten. Microsoft Defender for Office 365 ei kuitenkaan sisälly Microsoft 365 E3. Jos haluat jatkaa uhkien suojaamista, sinun on lisättävä muita Defender for Office 365 -käyttöoikeuksia niin, että kaikille Defender for Office 365 -käyttäjille on käyttöoikeus.

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Erot Microsoft 365 Business Premium ja Microsoft 365 Enterprise

Tässä taulukossa on esitetty Microsoft 365 Business Premium ja Microsoft 365 E3.

| Ominaisuus    | Tuki Microsoft 365 Business Premium    | Tuki Microsoft 365 E3 |
|:-------|:-----|:-----|
| **Paikallinen**        | | |
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3|
| Office sovellukset*    | [Microsoft 365 -sovellukset yrityksille](#office-365-business)    | Microsoft 365 -sovellukset yrityksille |
| **Pilvitallennussovellukset**        | | |
| Exchange Online ja Outlook    | 50 Gigatavun tallennustilaraja postilaatikkoa kohden ja rajoittamaton Exchange Online arkistointi    | 100 Gigatavun tallennustilaraja postilaatikkoa kohden ja rajoittamaton Exchange Online arkistointi |
| Teams    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
| OneDrive for Business    | 1 Tt tallennustilaraja käyttäjää kohden    | Rajoittamaton |
| Yammer, SharePoint Online, Planner, Stream    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
| **Threat Protection**        | | |
| Hyökkäyspinta-alaan pienennysominaisuudet    | [Katso tämä luettelo](#threat-protection) | Laitteistoon perustuvan eristysn yrityshallinta Microsoft Edge |
| Defender for Office 365 Plan 1 | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | Ei sisälly, mutta voidaan lisätä |
| **Käyttäjätietojen hallinta**        | | |
| Omatoiminen salasanan vaihtaminen yhdistelmäympäristön Azure Active Directory (Azure AD) -tileissä, Azure AD:n monimenetelmäinen todentaminen (MFA), ehdollinen käyttöoikeus, paikallisen käyttäjätiedot salasanalla kirjoittamisen palautus|     ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
| Cloud App Discovery, Azure AD Näyttöyhteys kunto    |     | ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
| Azure AD Office 365 sovellukset Yksittäinen Sign-On (SSO): 10 sovellusta käyttäjää kohti (Valikoima saas -sovellukset, kuten Salesforce)* | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
| Azure AD Premium 1 kertakirjautuminen: ei rajoitusta (paikallinen sovellus Azure AD -sovelluksen välityspalvelimen kautta ja muut kuin valikoimasovellukset, jotka käyttävät Self-Service-integrointimalleja)    |     | ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
| **Laite- ja sovellushallinta**        | | |
| Microsoft Intune Autopilotin Windows,|     ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
|Virtual Desktop Access (VDA)    |  |     ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
|Windows Virtual Desktop (WVD)    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png) |     ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
|Jaetun tietokoneen aktivointi (SCA)    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png) |     ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
| Microsoftin työpöytäoptimoinnin paketti    | |     ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
| **Tietojen suojaus**        | | |
| Office 365 Tietojen menetyksen estäminen, Azure Information Protection Plan 1    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
| Window Information Protection for endpoint DLP    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
| **Client Access License (CAL-oikeudet)**    | | |
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows oikeuksien hallinta)| |         ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
| **Yhteensopivuus**        | | |
| Rajoittamattomasti sähköpostin arkistointia    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
| Yhteensopivuuden hallinta    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
| eDiscovery    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
| Pito ja oikeus riitautuksen pito    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
| Viestitietueiden hallinnan (MRM) säilytystunnisteet ja säilytyskäytännöt    | ![Sisältyy Microsoft 365 Business Premium](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3](../media/check-mark.png) |
||||

\* Käyttäjät, joilla on saas-sovellusten käyttöoikeus, voivat saada SSO-käyttöomme jopa 10 sovellusta. Järjestelmänvalvojat voivat määrittää kertakirjautumisen ja muuttaa eri SaaS-sovellusten käytön, mutta kertakirjautumiskäyttö sallitaan vain 10 käyttäjälle kerrallaan. Kaikki Office 365-sovellukset lasketaan yhteen sovellukseen.

## <a name="migration"></a>Siirto

Jos haluat siirtää tilauksesi ja käyttöoikeutesi Microsoft 365 Business Premium kumppanisi kanssa, siirrä ne Microsoft 365 E3 tilaukseen, joka sisältää sen käyttöoikeudet.

Seuraavissa osissa kerrotaan, mitä muutoksia on tehtävä (jos niitä on) ja mitä voit tehdä siirron jälkeen.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Microsoft 365 määrittäminen ja tiedot

Sinun ei tarvitse tehdä muutoksia nykyiseen tilaukseesi tai tietoihin ennen sen muutosta, joka sisältää seuraavat:

- Tilausmääritykset, kuten DNS-toimialuenimet.
- Käyttäjä- ja ryhmätilit ja todentamisasetukset, kuten monimenetelmäinen todentaminen tai ehdolliset käyttöoikeuskäytännöt.
- Tuottavuuspalvelun määritykset ja niiden tiedot, kuten Teams, Exchange Online postilaatikot, SharePoint online-sivustot, OneDrive for Business kansiot OneNote muistikirjat.

Käyttäjät voivat nyt nauttia rajoittamattomasta tallennustilasta Exchange Online postilaatikoissa ja OneDrive for Business kansioissa.

Voit aloittaa Cloud App Discoveryn, Azure AD Näyttöyhteys Healthin ja SSO:n käytön yli 10 sovelluksessa.

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Uhkien suojaus

Windows 10 Business sisältää seuraavat suojaukset:

- Käyttöjärjestelmän käynnistysprosessin eheyden pakotus
- Arkaluonteisten käyttökomponenttien eheyden pakotus
- Kehittynyt haavoittuvuus ja nollapäiväinen riskien lieventäminen
- Maineen pohjainen verkon suojaus Microsoft Edge, Internet Explorerille ja Chromelle
- Isäntäpohjainen palomuuri
- Kiristysohjelmien riskien lieventäminen
- Laitteistopohjainen eristys Microsoft Edge
- Älykkään suojausjärjestelmän sovellushallinta Graph
- Laiteohjaus (USB)
- Verkkosuojaus verkkopohjaisia uhkia varten
- Isännän tunkeilun estämissäännöt

Windows 10 Enterprise E3 sisältää myös laitteistopohjaisen eristämisen yrityshallinnan Microsoft Edge.

> [!NOTE]
> Käyttäjät, jotka siirretään Microsoft 365 E3 edellyttävät Microsoft Defenderiä, jotta Office 365 uhkien jatkuvalle suojalle. Muista ostaa lisää Defender for Office 365 käyttöoikeuksia, jotta kaikilla Defender for Office 365 -käyttöoikeuksilla on käyttöoikeus.

### <a name="device-management-with-intune"></a>Laitehallinta Intunen avulla

Sinun ei tarvitse tehdä muutoksia nykyiseen Intune-määritykseen ennen muutosta, joka sisältää rekisteröidyt laitteet ja laite- ja sovellusasetukset.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium sisältää Windows 10 Business, jotka voit asentaa Windows AutoPilotin avulla. Kun siirryt Microsoft 365 E3, jokainen käyttöoikeus sisältää Windows 10 Enterprise E3:n, jonka voit asentaa myös Windows Autopilotilla.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365 -sovellukset yrityksille

Tietokoneeseen Microsoft 365 -sovellukset yrityksille asiakasohjelma alkaa automaattisesti käyttää Microsoft 365 -sovellukset suuryrityksille. Siirron jälkeen voit nyt käyttää:

- Ryhmäkäytännön tuki
- Spreadsheet compare and inquire
- Liiketoimintatiedot
