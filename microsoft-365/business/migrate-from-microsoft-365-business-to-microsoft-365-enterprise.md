---
title: Siirtyminen Microsoft 365 Businessista Microsoft 365 E3:een
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
description: Lue, miten voit siirtää yrityksesi Microsoft 365 Business Premiumista Microsoft 365 E3:iin.
ms.openlocfilehash: 6a795d96ccae7e054e7e52d4fd60a4e73b3c71dd
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/27/2020
ms.locfileid: "45081809"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Siirtyminen Microsoft 365 Business Premiumista Microsoft 365 E3:een

Microsoft 365 Business Premiumissa on kaikki mitä tarvitset pienyrityksellesi, ja siinä yhdistyvät luokkansa parhaat pilvipohjaiset tuottavuussovellukset sekä yksinkertainen laitehallinta ja -suojaus, joiden avulla työntekijät voivat tehdä parhaansa. Joissakin tapauksissa microsoft 365 Business Premium -tilauksesi on kuitenkin ehkä siirrettävä Microsoft 365 E3:een. 

Esimerkiksi yrityksesi on kasvanut ja tarvitsee yli 300 lisenssiä (onnittelut muuten).

Yrityksesi tarvitsee myös yritysominaisuuksia, kuten Microsoft 365 Apps for enterprise-, Windows 10 Enterprise E3- tai Enterprise Client Access License (CALs) -käyttöoikeuksia.

Päivittäminen on helppoa: voit aloittaa päivityksen [hallintakeskuksesta](../commerce/subscriptions/upgrade-to-different-plan.md). Kaikki nykyisen tilauksesi tiedot ja määritykset säilytetään. Ei ole mitään tekemistä voit valmistautua muuttoliikkeen ja mitään tekemistä jälkeenpäin, paitsi hyödyntää uusia ominaisuuksia.

>[!Note]
>Voit myös käyttää Microsoft 365 Business Premium -tilausta enintään 300 käyttöpenkkiä varten ja saada Microsoft 365 E3 -tilauksen yli 300 käyttöpenkkiä varten. Office 365 ATP ei kuitenkaan sisälly Microsoft 365 E3:een. Jos haluat jatkaa uhkien suojausta, lisää Office 365 ATP -käyttöoikeuksia, jotta kaikki Office 365 ATP -poliisien käyttäjät ovat lisensoituja.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Microsoft 365 Business Premiumin ja Microsoft 365 Enterprisen erot

Tässä taulukossa esitetään Microsoft 365 Business Premiumin ja Microsoft 365 E3:n väliset erot.

| Ominaisuus    | Microsoft 365 Business Premiumin tuki    | Microsoft 365 E3:n tuki | 
|:-------|:-----|:-----|
| **Paikallinen**        | | | 
| Windows 10    | Windows 10 Liiketoiminta  |     Windows 10 Enterprise E3| 
| Office-sovellukset*    | [Microsoft 365 -sovellukset yrityksille](#office-365-business)    | Microsoft 365 -sovellukset yrityksille | 
| **Pilvituottavuussovellukset**        | | | 
| Exchange Online ja Outlook    | 50 Gt:n tallennustilarajoitus postilaatikkoa kohden ja rajoittamaton Exchange Online -arkistointi    | 100 Gt:n tallennustilarajoitus postilaatikkoa kohden ja rajoittamaton Exchange Online -arkistointi | 
| Joukkueet    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
| OneDrive for Business    | 1 Tt:n tallennusraja käyttäjää kohden    | Rajoittamaton | 
| Yammer, SharePoint Online, Suunnittelija, Stream    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
| Outlook-asiakaspäällikkö, MileIQ    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | | 
| **Uhkien torjunta**        | | | 
| Hyökkäyspinnan pienennysominaisuudet    | [Katso tämä luettelo](#threat-protection) | Microsoft Edgen laitteistopohjaisen eristyksen hallinta | 
| Office 365 Advanced Threat Protection (ATP) -palvelupaketti 1 | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | Ei sisälly, mutta voidaan lisätä | 
| **Identiteetin hallinta**        | | | 
| Azure Active Directory (Azure AD) -hybriditilien, Azure multi-factor-todennuksen (MFA), ehdollisen käytön, paikallisten käyttäjätietojen salasanan takaisinkutsun oletusasetusten palauttaminen|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
| Pilvisovelluksen etsintä, Azure AD Connect -terveys    |     | ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
| Azure AD Office 365 -sovellukset Kertakirjautuminen (SSO): 10 sovellusta käyttäjää kohden (Galleria SaaS -sovellukset, kuten Salesforce)* | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
| Azure AD Premium 1 SSO: ei rajoitusta (paikalliset sovellukset Azure AD Application Proxy -välityspalvelimen ja muiden kuin galleriasovellusten kautta itsepalvelusovellusten integrointimallien avulla)    |     | ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
| **Laite- ja sovellushallinta**        | | | 
| Microsoft Intune, Windowsin automaattiohjaus|     ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
|Virtuaalityöpöydän käyttö (VDA)    |  |     ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
|Windowsin virtuaalinen työpöytä (WVD)    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png) |     ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
|Jaetun tietokoneen aktivointi (SCA)    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png) |     ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
| Microsoftin työpöydän optimointipaketti    | |     ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
| **Tietojen suojaaminen**        | | | 
| Office 365:n tietojen menetyksen estäminen, Azure-tietojen suojaussuunnitelma 1    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
| Ikkunatietojen suojaus päätepisteen DLP-tekniikalle    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
| **Client Access License (CAL-käyttöoikeudet)**    | | |     
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)| |         ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
| **Noudattaminen**        | | | 
| Rajoittamaton sähköpostin arkistointi    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
| Vaatimustenmukaisuuden pisteet / Compliance Manager    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
| Ediscovery    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
| Pito ja riita-asiat    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
| Mrm(Messaging Records Management) -säilytystunnisteet ja säilytyskäytännöt    | ![Sisältyy Microsoft 365 Business Premiumiin](../media/check-mark.png)    | ![Sisältyy Microsoft 365 E3:een](../media/check-mark.png) | 
||||

\*Käyttäjät, joille on määritetty SaaS-sovellusten käyttöoikeus, voivat käyttää enintään 10 sovellusta. Järjestelmänvalvojat voivat määrittää kertakirjautumisen ja muuttaa eri SaaS-sovellusten käyttöoikeuksia, mutta SSO-käyttö on sallittu vain 10 sovellukselle käyttäjää kohti kerrallaan. Kaikki Office 365 -sovellukset lasketaan yhdeksi sovellukseksi.

## <a name="migration"></a>Siirron

Voit siirtää microsoft 365 Business Premium -tilauksen ja -käyttöoikeudet sopivalle Microsoft 365 E3 -tilaukselle käyttöoikeuksiensa avulla kumppanisi kanssa.

Seuraavissa osissa kuvataan, mitä muutoksia sinun on tehtävä, jos sellaisia on ja mitä voit tehdä siirron jälkeen.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Microsoft 365 -tilauksen määritys ja tiedot

Sinun ei tarvitse tehdä muutoksia nykyiseen tilaukseesi tai tietoihin ennen siirtämistä, joka sisältää:

- Tilauksen määritykset, kuten DNS-toimialuenimet.
- Käyttäjä- ja ryhmätilit ja todennusasetukset, kuten monivaiheinen todennus tai ehdollisen käytön käytännöt.
- Tuottavuuspalvelun määritykset ja niiden tiedot, kuten Teams, Exchange Online -postilaatikot, SharePoint Online -sivustot, OneDrive for Business -kansiot ja OneNote-muistikirjat.

Käyttäjät voivat nyt nauttia rajoittamattomasta tallennustilasta Exchange Online -postilaatikoissa ja OneDrive for Business -kansioissa.

Voit aloittaa Cloud App Discoveryn, Azure AD Connect Healthin ja SSO:n käytön yli 10 sovelluksessa.

>[!Note]
>Microsoft 365 E3:een siirretyt käyttäjät eivät voi enää käyttää Outlook Customer Manageria ja MileIQ:ta.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Uhkien torjunta

Windows 10 Business sisältää seuraavat suojaukset:

- Eheyden valvonta käyttöjärjestelmän käynnistysprosessi
- Arkaluonteisten käyttökomponenttien eheyden valvonta
- Edistyneiden haavoittuvuuksien ja nollapäivän hyväksikäytön lieventämiset
- Microsoft Edgen, Internet Explorerin ja Chromen mainepohjainen verkkosuojaus
- Isäntäpohjainen palomuuri
- Ransomware lieventäminen
- Laitteistopohjainen eristäminen Microsoft Edgelle
- Älykäs suojauskaavion tarjoama sovellusten hallinta
- Laitteen ohjaus (USB)
- Verkkosuojaus verkkopohjaisille uhkille
- Isännän tunkeutumisen ehkäisyä koskevat säännöt

Windows 10 Enterprise E3 sisältää myös microsoft Edgen laitteistopohjaisen eristyksen yrityshallinnan.

>[!Note]
>Microsoft 365 E3:een siirretyt käyttäjät tarvitsevat kumpikin Office 365 ATP -käyttöoikeuden jatkuvaa uhkien suojausta varten. Muista ostaa lisää Office 365 ATP -käyttöoikeuksia, jotta kaikki Office 365 ATP -poliisien piiriin kuuluvat käyttäjät ovat lisensoituja. 
>

### <a name="device-management-with-intune"></a>Laitteen hallinta Intunen avulla

Sinun ei tarvitse tehdä muutoksia nykyiseen Intune-kokoonpanoosi ennen muuttoa, joka sisältää rekisteröityneet laitteet sekä laite- ja sovellusasetukset.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium sisältää Windows 10 Businessin, jonka voit asentaa Windowsin automaattiohjauksella. Kun siirryt Microsoft 365 E3:een, jokainen käyttöoikeus sisältää Windows 10 Enterprise E3:n, jonka voit asentaa myös Windowsin automaattiohjauksella.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365 -sovellukset yrityksille

Laitteisiin asennetut Microsoft 365 -yrityssovellukset alkavat automaattisesti käyttää Microsoft 365 Apps for enterprise -sovelluksen ominaisuuksia. Siirron jälkeen voit nyt käyttää:

 - Volyymiaktivointi ryhmäkäytännön avulla
 - Sovelluksen telemetria
 - Päivitä ohjausobjektit
 - Laskentataulukon vertailu ja kysely
 - Liiketoimintatieto

