---
title: Ehdollisten käyttökäytäntöjen määrittäminen Microsoft 365 -kampanjoille
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Lue, miten voit määrittää Microsoft 365 -kampanjoiden ehdollisen käytön käytännöt, jotka lisäävät huomattavaa lisäsuojausta.
ms.openlocfilehash: d7c9cfee2ef00e4ebe231a28ccca185c10f53c6b
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403014"
---
# <a name="set-up-conditional-access-policies"></a>Ehdollisen käytön käytäntöjen määrittäminen

[Ehdollisen käytön](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) käytännöt lisäävät huomattavasti lisäsuojausta. Microsoft sisältää joukon perusaikataulun ehdollisia käyttökäytäntöjä, joita suositellaan kaikille asiakkaille. Perusaikataulun käytännöt ovat joukko ennalta määritettyjä käytäntöjä, jotka auttavat suojaamaan organisaatioita useilta yleisiltä hyökkäyksiltä. Näitä yleisiä hyökkäyksiä voivat olla salasanasumutteet, toisto ja tietojenkalastelu.

Nämä käytännöt edellyttävät, että järjestelmänvalvojat ja käyttäjät kirjoittavat toisen todennusmuodon (monivaiheinen todennus tai mfa), kun tietyt ehdot täyttyvät. Jos käyttäjä esimerkiksi kirjautuu sisään toisesta maasta, kirjautumista voidaan pitää riskialttiina ja käyttäjän on annettava lisätodennusmuoto. 

Tällä hetkellä perusaikataulun käytännöt sisältävät seuraavat:
- **Vaadi mfa ylläpitäjät** &ndash; Edellyttää monivaiheista todennusta etuoikeutetuimmille järjestelmänvalvojan rooleille, mukaan lukien yleinen järjestelmänvalvoja.
- **Loppukäyttäjän suojaus** &ndash; Edellyttää monivaiheista todennusta käyttäjille vain, kun kirjautuminen on riskialtista. 
- **Estä vanha todennus** &ndash; Vanhemmat asiakassovellukset ja jotkin uudet sovellukset eivät käytä uudempia, turvallisempia todennusprotokollia. Nämä vanhemmat sovellukset voivat ohittaa ehdollisen pääsyn käytännöt ja saada luvattoman pääsyn ympäristöön. Tämä käytäntö estää sellaisten asiakkaiden käytön, jotka eivät tue ehdollista käyttöä. 
- **Vaadi mfa palvelunhallintaa** &ndash; varten Edellyttää monivaiheista todennusta hallintatyökalujen, kuten Azure-portaalin (jossa perusaikataulukäytännöt määritetään) käyttöä varten. 

Microsoft suosittelee, että otat käyttöön kaikki nämä perusaikataulukäytännöt. Kun nämä käytännöt on otettu käyttöön, järjestelmänvalvojia ja käyttäjiä pyydetään rekisteröitymään Azure Multii-Factor -todennukseen.

Lisätietoja näistä käytännöistä on ohjeaiheessa [Mitä ovat peruskäytännöt](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Perusaikataulun käytäntöjen määrittäminen

1. Siirry [Azure-portaaliin](https://portal.azure.com)ja siirry sitten **Azure Active** \> **Directoryn ehdolliseen käyttöön**.
    
    Perusaikataulun käytännöt näkyvät sivulla. <br/> <br/>
    ![Sivu, jossa on luettelo ehdollisen käytön peruskäytäntöjen käyttämisestä.](../media/baslinepolicies.png)
1. Katso seuraavat kunkin käytännön erityisohjeet:

  - [Vaadi mfa ylläpitäjät](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Vaadi mfa käyttäjille](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Estä vanha todennus](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Vaadi mfa palvelun hallintaa varten](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Voit määrittää useita lisäkäytäntöjä, kuten vaatia hyväksyttyjä asiakassovelluksia. Lisätietoja on [Ehdollisen käytön ohjeissa](https://docs.microsoft.com/azure/active-directory/conditional-access/).
