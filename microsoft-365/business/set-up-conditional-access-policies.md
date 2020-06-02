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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Lue tietoja siitä, miten voit määrittää Ehdollisen käytön käytännöt Microsoft 365 -kampanjoille, jotta voit lisätä huomattavasti lisäsuojaa.
ms.openlocfilehash: 58ee760877ee2fd7e53ef9463242657ab66a2b6e
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470643"
---
# <a name="set-up-conditional-access-policies"></a>Ehdollisen käytön käytäntöjen määrittäminen

Tämä artikkeli koskee Microsoft 365 Business Premiumia.

[Ehdollisen käytön](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) käytännöt lisäävät huomattavaa lisäsuojaa. Microsoft issa on joukko ehdollisen käytön peruskäytäntöjä, joita suositellaan kaikille asiakkaille. Perusaikataulun käytännöt ovat joukko ennalta määritettyjä käytäntöjä, jotka auttavat suojaamaan organisaatioita monilta yleisiltä hyökkäyksiltä. Näitä yleisiä hyökkäyksiä voivat olla salasanasumute, uusinta ja tietojenkalastelu.

Nämä käytännöt edellyttävät, että järjestelmänvalvojat ja käyttäjät kirjoittavat toisen todennuksen muodon (multifactor-todennuksen tai mfa-menetelmän), kun tietyt ehdot täyttyvät. Jos käyttäjä esimerkiksi kirjautuu sisään toisesta maasta, sisäänkirjautumista voidaan pitää riskialttiina ja käyttäjän on annettava lisätodennuksen muoto. 

Tällä hetkellä perusaikataulun käytännöt sisältävät seuraavat:
- **Vaadi MFA järjestelmänvalvojille** &ndash; Edellyttää monivaiheista todennusta etuoikeutetummille järjestelmänvalvojan rooleille, myös yleiselle järjestelmänvalvojalle.
- **Loppukäyttäjän suojaus** &ndash; Edellyttää monivaiheista todennusta käyttäjille vain, kun kirjautuminen on riskialtista. 
- **Estä vanha todennus** &ndash; Vanhemmat asiakassovellukset ja jotkin uudet sovellukset eivät käytä uudempia, turvallisempia todennusprotokollia. Nämä vanhemmat sovellukset voivat ohittaa ehdollisen käytön käytännöt ja käyttää ympäristöäsi luvatta. Tämä käytäntö estää pääsyn asiakkailta, jotka eivät tue ehdollista käyttöä. 
- **Vaadi MFA palvelunhallintaa** &ndash; varten Edellyttää monivaiheista todennusta hallintatyökalujen, kuten Azure-portaalin (jossa perusaikataulun käytännöt määritetään) käyttöä varten. 

Microsoft suosittelee, että otat käyttöön kaikki nämä perusaikataulun käytännöt. Kun nämä käytännöt on otettu käyttöön, järjestelmänvalvojia ja käyttäjiä pyydetään rekisteröitymään Azure Multii-Factor -todennukseen.

Lisätietoja näistä käytännöistä on kohdassa [Mitä ovat perusaikataulun käytännöt?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)


## <a name="set-up-baseline-policies"></a>Perusaikataulun käytäntöjen määrittäminen

1. Siirry [Azure-portaaliin](https://portal.azure.com)ja siirry sitten **Azure Active** \> **Directoryn ehdolliseen käyttöön**.
    
    Perusaikataulun käytännöt näkyvät sivulla. <br/> <br/>
    ![Sivu, jossa on luettelo ehdollisen käytön perusaikataulun käytännöistä.](../media/baslinepolicies.png)
1. Katso seuraavat kunkin käytännön ohjeet:

  - [Vaadi MFA järjestelmänvalvojille](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Vaadi mfa käyttäjille](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Estä vanha todennus](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Vaadi mfa palvelunhallintaa varten](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Voit määrittää useita lisäkäytäntöjä, kuten hyväksyttyjen asiakassovellusten vaatimista. Lisätietoja on [Ehdollisen käytön ohjeissa](https://docs.microsoft.com/azure/active-directory/conditional-access/).
