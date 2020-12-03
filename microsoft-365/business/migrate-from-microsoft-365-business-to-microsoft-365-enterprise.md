---
title: Siirtyminen Microsoft 365 Business-Microsoft 365 E3-tieto koneesta
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
description: Opi siirtämään yrityksesi Microsoft 365 Business Premiumista Microsoft 365 E3-tieto koneeseen.
ms.openlocfilehash: 3f1bb9591e1bd2bac49326325ce6c8c2d6778497
ms.sourcegitcommit: c1dd5be42fe0c5dcc7c05817c941edd9076febf8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/02/2020
ms.locfileid: "49558234"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Siirtäminen Microsoft 365 Business Premiumista Microsoft 365 E3-tieto koneesta

Microsoft 365 Business Premiumissa on kaikki, mitä tarvitset pien yrityksellesi, yhdistämällä huippuhuippuiset pilvipohjaiset tuottavuus sovellukset yksinkertaiseen laite hallintaan ja tieto turvaan, jotka mahdollistavat työn tekijöiden parhaan työn. Joissain tapa uksissa Microsoft 365 Business Premium-tilaus on ehkä siirrettävä Microsoft 365 E3-tila ukseen. 

Esimerkiksi yrityksesi on kasvanut ja tarvitsee enemmän kuin 300-käyttö oikeuksia (onneksi olkoon).

Tai yrityksesi tarvitsee yritys ominaisuuksia, kuten Microsoft 365-sovelluksia yritys käyttöön, Windows 10 Enterprise E3 tai Enterprise Client-käyttö oikeuksia (CALs).

Päivitys on helppoa: voit aloittaa päivityksen [hallinta keskuksesta](../commerce/subscriptions/upgrade-to-different-plan.md). Kaikki nykyisen tilauksesi tiedot ja määritykset säilytetään. Sinun ei tarvitse tehdä mitään, jos haluat valmistautua siirtoon eikä mitään jälkeenpäin, paitsi hyödyntää uusia ominaisuuksia.

>[!Note]
>Voit käyttää myös Microsoft 365 Business Premium-pakettia, jossa on enintään 300 paikkaa ja saat Microsoft 365 E3-tila uksen, jossa on yli 300 paikkaa. Microsoft Defender for Office 365 ei kuitenkaan sisälly Microsoft 365 E3-sovellukseen. Jos haluat jatkaa uhkien suojaamista, lisää Office 365-käyttö oikeuksien Defender, jotta kaikki Office 365-käytäntöjä koskevat käyttäjät saavat käyttö oikeuden.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Erot Microsoft 365 Business Premiumin ja Microsoft 365 Enterprisen välillä

Tässä taulukossa esitellään Microsoft 365 Business Premiumin ja Microsoft 365 E3-messujen erot.

| Ominaisuus    | Microsoft 365 Business Premiumin tuki    | Tuki Microsoft 365 E3-sovelluksessa | 
|:-------|:-----|:-----|
| **Paikallinen**        | | | 
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3| 
| Office-sovellukset *    | [Microsoft 365-sovellukset yrityksille](#office-365-business)    | Microsoft 365 -yrityssovellukset | 
| **Pilvi palveluiden tuottavuus sovellukset**        | | | 
| Exchange Online ja Outlook    | 50 gt tallennus tilan rajoitus posti laatikkoa kohden ja rajoittamaton Exchange Online-arkistointi    | 100 gt tallennus tilan rajoitus posti laatikkoa kohden ja rajoittamaton Exchange Online-arkistointi | 
| Teams    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| OneDrive for Business    | 1 TERATAVUN tallennus tila raja käyttäjää kohden    | Rajoittamattomat | 
| Yammer, SharePoint Online, Planner, Streamin    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| MileIQ    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | | 
| **Uhkien suojaus**        | | | 
| Hyökkäys pinnan vähennys ominaisuudet    | [Katso tämä lista](#threat-protection) | Microsoft Edgen laitteistopohjaisen eristämisen yritys hallinta | 
| Office 365-paketin 1 Defender | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | Ei sisälly, mutta se voidaan lisätä | 
| **Tunniste tietojen hallinta**        | | | 
| Omatoiminen Sala sanan palautus yhdistelmä Azure Active Directory (Azure AD)-tileillä, Azure AD Multi-Factor-todennus (MFA), ehdollinen käyttö oikeus, Sala sanan palauttaminen paikallisille identiteeteille|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| Pilvi sovellusten etsiminen, Azure AD Connect Health    |     | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| Azure AD Office 365-sovellukset yksi Sign-On (SSO): 10 sovellusta käyttäjää kohden (Galleria SaaS-sovellukset, kuten Salesforce) * | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| Azure AD Premium 1 SSO: ei rajoitusta (paikalliset sovellukset Azure AD Application Proxy-ja Non-Gallery-sovellusten kautta Self-Service sovellusten integrointi mallien avulla)    |     | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| **Laitteen ja sovellusten hallinta**        | | | 
| Microsoft Intune, Windowsin Autopilot|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
|Virtual Desktop Accessia (VDA)    |  |     ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
|Windowsin Näennäistyöpöytä (WVD)    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png) |     ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
|Jaettujen tieto koneiden Akti vointi (SCA)    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png) |     ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| Microsoftin työpöydän optimointi paketti    | |     ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| **Tieto turva**        | | | 
| Office 365 tietojen menetyksen estäminen, Azuren tieto turva sopimus 1    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| Ikkuna tieto turva pääte pisteen DLP    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| **Client Access License (CAL-käyttö oikeus)**    | | |     
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoftin pääte pisteen määritysten hallinta, Windows Rights Management)| |         ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| **Noudattamisen**        | | | 
| Rajoittamaton sähkö postin arkistointi    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| Yhteensopivuuden valvoja    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| eDiscovery    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| Pidossa oleva pito ja oikeus toimiin liittyvään pitoon    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
| Viestintä tietueiden hallinta (MRM) säilytys Tunnisteet ja säilytys käytännöt    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3-pakettiin](../media/check-mark.png) | 
||||

\* Käyttäjät, joille on määritetty SaaS-sovellusten käyttö oikeus, voivat hankkia KERTAKIRJAUTUMISEN jopa 10 sovellukseen. Järjestelmänvalvojat voivat määrittää KERTAKIRJAUTUMISEN ja vaihtaa käyttö oikeuksia eri SaaS-sovelluksille, mutta kertakäyttöinen käyttö oikeus on sallittu vain 10: lle sovelluksen käyttäjää kohden kerrallaan. Kaikki Office 365-sovellukset lasketaan yhdeksi sovellukseksi.

## <a name="migration"></a>Siirto

Jos haluat siirtää Microsoft 365 Business Premium-tila uksen ja käyttö oikeudet sopivan Microsoft 365 E3-tila ukseen, sinun on työskenneltävä yhdessä kumppanien kanssa.

Seuraavissa osissa kerrotaan, mitä muutoksia sinun on tehtävä ja mitä voit tehdä siirron jälkeen.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Microsoft 365-tila uksen määritykset ja tiedot

Sinun ei tarvitse tehdä muutoksia nykyiseen tilaukseesi tai tiedoihisi ennen siirtoa, joka sisältää seuraavat tiedot:

- Tila uksen määritykset, kuten DNS-toimi alue nimet.
- Käyttäjä-ja ryhmä tunnukset sekä todennus asetukset, kuten usean tekijän todentaminen tai ehdolliset käyttö oikeus käytännöt.
- Tuottavuus palvelu määritykset ja niiden tiedot, kuten tiimit, Exchange Online-posti laatikot, SharePoint Online-sivustot, OneDrive for Business-kansiot ja OneNote-muisti kirjat.

Käyttäjät voivat nyt nauttia rajoittamattomasta tallennus tilasta Exchange Online-posti laatikoissa ja OneDrive for Business-kansioissa.

Voit aloittaa pilvi sovellusten etsimisen, Azure AD Connect Healthin ja SKERTA:N käytön yli 10 sovellukselle.

>[!Note]
>Käyttäjät, jotka on siirretty Microsoft 365 E3-käyttö kohteeseen, eivät voi enää käyttää MileIQ-valmistetta
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Uhkien suojaus

Windows 10 Business sisältää seuraavat suoja ukset:

- Käyttö järjestelmän käynnistys prosessin eheys valvonta
- Arkaluonteisten käyttö komponenttien eheys valvonta
- Kehittynyt haavoittuvuus ja nolla päivän heikkoutta hyödyntävät lieventävät tekijät
- Maine-pohjainen verkon suojaus Microsoft Edgessä, Internet Explorerissa ja Chromessa
- Isäntäpohjainen palo muuri
- Kiristys ohjelmien lieventämis prosessit
- Laitteistopohjainen eristys Microsoft Edgessä
- Älykkään tieto turva graafin tarjoama sovellus ohjaus objekti
- Device Control (USB)
- Verkko suojaus verkkopohjaisia uhkia varten
- Isännän luvattoman käytön estämistä koskevat säännöt

Windows 10 Enterprise E3 sisältää myös Microsoft Edgeen laitepohjaisen eristämisen yritys hallinnan.

>[!Note]
>Käyttäjät, jotka on siirretty Microsoft 365 E3-käyttö oikeuteen, vaativat Microsoft Defender for Office 365-lisenssin jatkuvan uhkien suojaamiseksi. Varmista, että ostat lisää Office 365-käyttö oikeuksien Defender-ohjelman, jotta kaikki Office 365-käytäntöjä koskevat käyttäjät saavat käyttö oikeuden. 
>

### <a name="device-management-with-intune"></a>Laite hallinta Intune-palvelulla

Sinun ei tarvitse tehdä muutoksia nykyiseen Intune-määritykseen ennen siirtoa, joka sisältää myös rekisteröityneet laitteet sekä laitteiden ja sovellusten asetukset.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium sisältää Windows 10 Business-palvelu paketit, jotka voit asentaa Windows AutoPilot-asennuksen avulla. Kun siirryt Microsoft 365 E3-käyttö järjestelmään, jokaiseen käyttäjän käyttö oikeuteen sisältyy Windows 10 Enterprise E3, jonka voit asentaa myös Windows Autopilot-ohjelmiston avulla.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365-sovellukset yrityksille

Laitteisiisi asennettu Microsoft 365-sovellusten yritys sovellus alkaa automaattisesti käyttää Microsoft 365-sovellusten ominaisuuksia yrityksessä. Siirron jälkeen voit nyt käyttää:

 - Määrä Akti vointi ryhmä käytännöllä
 - Sovellustelemetria
 - Päivitä komponentit
 - Laskenta taulukon vertailu ja kysely
 - Liiketoiminta tiedot

