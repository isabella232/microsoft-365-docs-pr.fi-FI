---
title: Ehdollisen käytön käytäntöjen määrittäminen Microsoft 365 -kampanjoille
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
description: Lue tietoja ehdollisen käytön käytäntöjen määrittämisestä Microsoft 365 -kampanjoille, jotta voit lisätä huomattavaa lisäsuojausta.
ms.openlocfilehash: be3ca0da3d27e3ec49f1227e4482cfd7fcaae8cb
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550073"
---
# <a name="set-up-conditional-access-policies"></a>Ehdollisen käytön käytäntöjen määrittäminen

[Ehdollisen käytön](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) käytännöt lisäävät huomattavasti lisäsuojausta. Microsoft tarjoaa joukon perustason ehdollisia käyttökäytäntöjä, joita suositellaan kaikille asiakkaille. Perusaikataulun käytännöt ovat joukko ennalta määritettyjä käytäntöjä, jotka auttavat suojaamaan organisaatioita monilta yleisiltä hyökkäyksiltä. Näitä yleisiä hyökkäyksiä voivat olla salasanasuihke, uusinta ja tietojenkalastelu.

Nämä käytännöt edellyttävät, että järjestelmänvalvojat ja käyttäjät kirjoittavat toisen todennusmuodon (monivaiheinen todennus tai mfa), kun tietyt ehdot täyttyvät. Jos käyttäjä esimerkiksi kirjautuu sisään toisesta maasta, kirjautumista saatetaan pitää riskialttiina ja käyttäjän on annettava lisätodennusmuoto. 

Tällä hetkellä perustason käytäntöjä ovat seuraavat:
- **Vaadi mfa järjestelmänvalvojille** &ndash; Edellyttää monivaiheista todennusta etuoikeutetuimmille järjestelmänvalvojan rooleille, mukaan lukien yleinen järjestelmänvalvoja.
- **Loppukäyttäjän suojaus** &ndash; Edellyttää monivaiheista todennusta käyttäjille vain, kun kirjautuminen on riskialtista. 
- **Estä vanha todennus** &ndash; Vanhemmat asiakassovellukset ja jotkin uudet sovellukset eivät käytä uudempia, turvallisempia todennusprotokollia. Nämä vanhemmat sovellukset voivat ohittaa ehdollisen käytön käytännöt ja saada luvattoman pääsyn ympäristöösi. Tämä käytäntö estää pääsyn asiakkailta, jotka eivät tue ehdollista käyttöoikeutta. 
- **Vaadi mfa palvelunhallintaa** &ndash; edellyttää monivaiheista todennusta hallintatyökalujen, kuten Azure-portaalin (jossa perusaikataulun käytännöt määritetään). 

Microsoft suosittelee, että otat käyttöön kaikki nämä perusaikataulun käytännöt. Kun nämä käytännöt on otettu käyttöön, järjestelmänvalvojia ja käyttäjiä pyydetään rekisteröitymään Azure Multii-Factor -todennusta varten.

Lisätietoja näistä käytännöistä on ohjeaiheessa [Mitä ovat perustason käytännöt?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)


## <a name="set-up-baseline-policies"></a>Perusaikataulun käytäntöjen määrittäminen

1. Siirry [Azure-portaaliin](https://portal.azure.com)ja siirry sitten **Azure Active Directoryn** \> **ehdolliseen käyttöön**.
    
    Perusaikataulun käytännöt näkyvät sivulla. <br/> <br/>
    ![Sivu, jossa on luettelo ehdollisen käytön perusaikataulun käytännöistä.](../media/baslinepolicies.png)
1. Katso seuraavat tarkat ohjeet kustakin käytännöstä:

  - [Vaadi mfa ylläpitäjät](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Vaadi mfa käyttäjille](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Estä vanha todennus](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Vaadi mfa palvelunhallintaan](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Voit määrittää useita lisäkäytäntöjä, kuten edellyttää hyväksyttyjä asiakassovelluksia. Lisätietoja on [ehdollisen käytön dokumentaatiossa](https://docs.microsoft.com/azure/active-directory/conditional-access/).
