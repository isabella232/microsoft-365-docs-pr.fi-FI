---
title: Ehdollisten käyttö oikeus käytäntöjen määrittäminen Microsoft 365-kampanjoille
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
search.appverid:
- BCS160
- MET150
- MOE150
description: Lue lisä tietoja ehdollisten käyttö käytäntöjen määrittämisestä Microsoft 365-kampanjoille.
ms.openlocfilehash: 3772aa0d505ef54a0587423e890ede519d571e0c
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/07/2019
ms.locfileid: "38031391"
---
# <a name="set-up-conditional-access-policies"></a>Määritä ehdolliset käyttö oikeus käytännöt

[Ehdollisen käytön käytännöt lisäävät aineeksi](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) lisä suojausta. Microsoft tarjoaa perusaikataulun ehdollisten käyttö oikeus käytäntöjen joukon, jota suositellaan kaikille asiakkaille. Perusaikataulun käytännöt ovat joukko esimääritettyjä käytäntöjä, jotka auttavat suojaamaan organisaatioita monista yleisistä hyökkäyksistä. Näitä yleisiä hyökkäyksiä voivat olla Sala sanan suihkutus, uusinta toisto ja tietojenkalastelu.

Nämä käytännöt edellyttävät, että järjestelmänvalvojat ja käyttäjät syöttäisivät toisen todennus muodon (jota kutsutaan nimellä Monivaiheinen todennus tai MFA), kun tietyt ehdot täyttyvät. Jos käyttäjä on esimerkiksi kirjauduttava sisään toisesta maasta, kirjautumista voidaan pitää riskialttiina ja käyttäjän on annettava lisä todennus muoto. 

Tällä hetkellä perusaikataulun käytäntöjä ovat seuraavat:
- **Vaadi järjestelmänvalvojien makrotaloudellinen** tuki – vaatii usean tekijän todennuksen suosituimmille järjestelmänvalvojan rooleille, mukaan lukien yleinen järjestelmänvalvoja.
- **Loppu käyttäjän suojaus** – vaatii usean tekijän todennuksen käyttäjille vain silloin, kun kirjautuminen on riskialtista. 
- **Estä aiempi todennus** – vanhemmat asiakas sovellukset ja jotkin uudet sovellukset eivät käytä uudempia, turvallisempia todennus protokollia. Nämä vanhemmat sovellukset voivat ohittaa ehdolliset käyttö käytännöt ja käyttää ympäristöäsi luvattomasti. Tämä käytäntö estää pääsyn asiakkailta, jotka eivät tue ehdollista pääsyä. 
- **Vaadi palvelun hallinnan MFA-tuki** – vaatii monivaiheisen todennuksen hallinta työkalujen, kuten Azure-portaalin, käyttöä varten (Jos määrität peruskäytännöt). 

Microsoft suosittelee, että otat kaikki nämä perusaikataulun käytännöt käyttöön. Kun nämä käytännöt on otettu käyttöön, ylläpitäjiä ja käyttäjiä kehotetaan rekisteröitymään Azure Multii-Factor-todennukseen.

Lisä tietoja näistä käytännöistä on Ohje aiheessa [Mitä ovat perusaikataulun käytännöt](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Määritä perusaikataulun käytännöt

1. Siirry [Azure-portaaliin](https://portal.azure.com)ja siirry sitten **Azure Active Directoryn** \> **ehdolliseen pääsyyn**.
    
    Perusaikataulun käytännöt on lueteltu sivulla. <br/> <br/>
    ![Sivu, joka sisältää ehdollisen käytön peruskäytännöt.](media/baslinepolicies.png)
1. Katso seuraavat erityiset ohjeet kutakin käytäntöä varten:

  - [Vaadi järjestelmänvalvojien MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Vaadi MFA-käyttäjille](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Estä aiempi todennus](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Vaadi MFA palvelun hallintaa varten](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Voit määrittää useita lisä käytäntöjä, kuten hyväksyttyjen asiakas sovellusten vaatiminen. Lisä tietoja on [ehdollisen käytön ohjeissa](https://docs.microsoft.com/azure/active-directory/conditional-access/) .