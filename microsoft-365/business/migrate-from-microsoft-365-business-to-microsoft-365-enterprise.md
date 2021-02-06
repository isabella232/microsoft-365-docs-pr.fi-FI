---
title: Siirtyminen Microsoft 365 Businessista Microsoft 365 E3:lle
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
description: Opi siirtämään yrityksesi Microsoft 365 Business Premiumista Microsoft 365 E3:lle.
ms.openlocfilehash: 019a422bb879389f42a32cf30f9a8094f776078a
ms.sourcegitcommit: eac5d9f759f290d3c51cafaf335a1a1c43ded927
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/06/2021
ms.locfileid: "50126197"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Siirtyminen Microsoft 365 Business Premiumista Microsoft 365 E3:lle

Microsoft 365 Business Premium sisältää kaiken, mitä tarvitset pienyritystä varten yhdistämällä luokkansa parhaat pilvipohjaiset tuottavuussovellukset yksinkertaiseen laitehallintaan ja tietoturvaan, joiden avulla työntekijät voivat tehdä parasta työtään. Joissakin tapauksissa sinun on kuitenkin ehkä siirrettävä Microsoft 365 Business Premium -tilauksesi Microsoft 365 E3:lle. 

Yrityksesi on esimerkiksi kasvanut ja tarvitsee yli 300 käyttöoikeutta (onneksi olkoon).

Yrityksesi tarvitsee myös yritysominaisuuksia, kuten Microsoft 365 -sovellukset yrityksille, Windows 10 Enterprise E3 tai Enterprise Client Access Licenses (CALs).

Päivitys on helppoa: voit käynnistää päivityksen [hallintakeskuksesta.](../commerce/subscriptions/upgrade-to-different-plan.md) Kaikki nykyisen tilauksesi tiedot ja määritykset säilytetään. Sinun ei tarvitse valmistautua siirtoon eikä tehdä mitään sen jälkeen, paitsi hyödyntää uusia ominaisuuksia.

>[!Note]
>Voit myös käyttää Microsoft 365 Business Premium -tilausta enintään 300 käyttöpaikkaa varten ja saada Microsoft 365 E3 -tilauksen, jossa on yli 300 käyttöpaikkaa. Microsoft Defender for Office 365 ei kuitenkaan sisälly Microsoft 365 E3:lle. Jatkuvan uhkien suojauksen vuoksi sinun on lisättävä Office 365 -käyttöoikeuksiin ylimääräinen Defender, jotta kaikilla Defender for Office 365 -käyttäjillä on käyttöoikeus.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Microsoft 365 Business Premiumin ja Microsoft 365 Enterprisen erot

Tässä taulukossa on esitetty Microsoft 365 Business Premiumin ja Microsoft 365 E3:n väliset erot.

| Ominaisuus    | Microsoft 365 Business Premiumin tuki    | Microsoft 365 E3:n tuki | 
|:-------|:-----|:-----|
| **Paikallinen**        | | | 
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3| 
| Office-sovellukset*    | [Microsoft 365 -sovellukset yrityksille](#office-365-business)    | Microsoft 365 -yrityssovellukset | 
| **Pilvipalvelun tuottavuussovellukset**        | | | 
| Exchange Online ja Outlook    | 50 Gigatavun tallennustilaraja postilaatikkoa kohden ja rajoittamaton Exchange Online -arkistointi    | 100 Gigatavun tallennustilaraja postilaatikkoa kohden ja rajoittamaton Exchange Online -arkistointi | 
| Teams    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| OneDrive for Business    | 1 Tt tallennustilaraja käyttäjää kohden    | Rajoittamaton | 
| Yammer, SharePoint Online, Planner, Stream    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| MileIQ    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | | 
| **Threat Protection**        | | | 
| Hyökkäyspinta-alaan pienentämisominaisuudet    | [Katso tämä luettelo](#threat-protection) | Microsoft Edgen laitteistopohjaisen eristysympäristön yrityksen hallinta | 
| Defender for Office 365 Plan 1 | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | Ei sisälly, mutta se voidaan lisätä | 
| **Käyttäjätietojen hallinta**        | | | 
| Azure Active Directory (Azure AD) -yhdistelmätilien omatoiminen salasanan palautus, Azure AD:n monimenetelmäinen todentaminen (MFA), ehdollinen käyttöoikeus, paikallisen käyttäjäryhmän salasanan palautus|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| Cloud App Discovery, Azure AD Connect Health    |     | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| Azure AD Office 365 -sovellukset Sign-On (SSO): 10 sovellusta käyttäjää kohden (Valikoima SaaS -sovellukset, kuten Salesforce)* | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| Azure AD Premium 1 SSO: ei rajoitusta (paikallinen sovellus Azure AD -sovelluksen välityspalvelimen ja muiden kuin valikoimasovellusten kautta käyttämällä Self-Service-integrointimalleja)    |     | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| **Laitteiden ja sovellusten hallinta**        | | | 
| Microsoft Intune, Windows Autopilot|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
|Virtual Desktop Access (VDA)    |  |     ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
|Windowsin virtuaalityöpöytä (WVD)    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png) |     ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
|Jaetun tietokoneen aktivointi (SCA)    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png) |     ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| Microsoftin työpöytäoptimoinnin paketti    | |     ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| **Tietojen suojaus**        | | | 
| Office 365:n tietojen menetyksen estäminen, Azure Information Protection Plan 1    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| Window Information Protection for endpoint DLP    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| **Client Access License (CAL-oikeudet)**    | | |     
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windowsin oikeuksien hallinta)| |         ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| **Yhteensopivuus**        | | | 
| Rajoittamattoman sähköpostin arkistointi    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| Yhteensopivuuden hallinta    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| eDiscovery    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| Pito- ja oikeusistuntoon pito    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
| Messaging Records Management (MRM) -säilytystunnisteet ja säilytyskäytännöt    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Mukana Microsoft 365 E3](../media/check-mark.png) | 
||||

\* Käyttäjät, joilla on SaaS-sovellusten käyttöoikeus, voivat käyttää SSO-käyttöomme jopa 10 sovellusta. Järjestelmänvalvojat voivat määrittää kertakirjautumisen ja muuttaa eri SaaS-sovellusten käyttöoheuksia, mutta kertakirjautumisen käyttö sallitaan vain 10 käyttäjälle kerrallaan. Kaikki Office 365 -sovellukset lasketaan yhteen sovellukseen.

## <a name="migration"></a>Siirto

Siirrä Microsoft 365 Business Premium -tilauksesi ja -käyttöoikeutesi sopivaan Microsoft 365 E3 -tilaukseen, jonka käyttöoikeudet sinulla on, työskentele yhdessä kumppanisi kanssa.

Seuraavissa osissa kerrotaan, mitä muutoksia on tehtävä ja mitä voit tehdä siirron jälkeen.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Microsoft 365 -tilauksen määritykset ja tiedot

Sinun ei tarvitse tehdä muutoksia nykyiseen tilaukseesi tai tietoihin ennen sen muutosta, joka sisältää seuraavat:

- Tilausmääritykset, kuten DNS-toimialuenimet.
- Käyttäjä- ja ryhmätilit ja todennusasetukset, kuten monimenetelmäinen todentaminen tai ehdollisten käyttöoikeuksien käytännöt.
- Tuottavuuspalvelun määritykset ja niiden tiedot, kuten Teams, Exchange Online -postilaatikot, SharePoint Online -sivustot, OneDrive for Business -kansiot ja OneNote-muistikirjat.

Käyttäjät voivat nyt nauttia rajoittamattomasta tallennustilasta Exchange Online -postilaatikoissa ja OneDrive for Business -kansioissa.

Voit aloittaa Cloud App Discoveryn, Azure AD Connect Healthin ja SSO:n käytön yli 10 sovellukselle.

>[!Note]
>Microsoft 365 E3:lle siirretyt käyttäjät eivät voi enää käyttää MileIQ:a.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Uhkien torjunta

Windows 10 Business sisältää seuraavat suojaukset:

- Käyttöjärjestelmän käynnistysprosessin eheyden pakotus
- Arkaluonteisten käyttökomponenttien eheyden pakotus
- Kehittynyt haavoittuvuus ja nollapäiväinen haun riskien lieventäminen
- Microsoft Edgen, Internet Explorerin ja Chromen mainepohjainen verkon suojaus
- Isäntäpohjainen palomuuri
- Kiristysohjelmien riskien lieventäminen
- Microsoft Edgen laitteistopohjainen eristys
- Älykkään suojauskaavion sovellusohjausobjekti
- Laiteohjaus (USB)
- Verkkosuojaus verkkopohjaisia uhkia varten
- Isännän tunkeilun estämissäännöt

Windows 10 Enterprise E3 sisältää myös laitteistopohjaisen eristysympäristön hallinnan Microsoft Edgessä.

>[!Note]
>Microsoft 365 E3:lle siirretyt käyttäjät edellyttävät microsoft Defender for Office 365 -käyttöoikeutta, jotta he voivat jatkaa uhkientorjuntaa. Muista ostaa lisää Defender for Office 365 -käyttöoikeuksia, jotta kaikilla Defender for Office 365 -käyttäjillä on käyttöoikeus. 
>

### <a name="device-management-with-intune"></a>Laitehallinta Intunen avulla

Sinun ei tarvitse tehdä muutoksia nykyiseen Intune-määritykseesi ennen sen muutosta, joka sisältää rekisteröidyt laitteet sekä laite- ja sovellusasetukset.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium sisältää Windows 10 Businessin, jonka voit asentaa Windows AutoPilotilla. Kun siirryt Microsoft 365 E3:lle, jokainen käyttöoikeus sisältää Windows 10 Enterprise E3:n, jonka voit asentaa myös Windows Autopilotilla.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365 -sovellukset yrityksille

Laitteisiisi asennetut Microsoft 365 Apps for Business -sovellukset alkavat automaattisesti käyttää Microsoft 365 Apps for Enterprisen ominaisuuksia. Siirron jälkeen voit nyt käyttää:

 - Ryhmäkäytäntöjen tuki
 - Spreadsheet Compare ja inquire
 - Liiketoimintatiedot

