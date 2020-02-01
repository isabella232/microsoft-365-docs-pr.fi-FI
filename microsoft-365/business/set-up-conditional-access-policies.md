---
title: Ehdollisten käyttö oikeus käytäntöjen määrittäminen Microsoft 365-kampanjoille
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
search.appverid:
- BCS160
- MET150
- MOE150
description: Lue lisä tietoja ehdollisten käyttö käytäntöjen määrittämisestä Microsoft 365-kampanjoille.
ms.openlocfilehash: 335fbd7e771b1595e1846529daed76e5ddd3a8f5
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593381"
---
# <a name="set-up-conditional-access-policies"></a>Määritä ehdolliset käyttö oikeus käytännöt

[Ehdollisen käytön](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) käytännöt lisäävät huomattavasti lisä suojausta. Microsoft tarjoaa perusaikataulun ehdollisten käyttö oikeus käytäntöjen joukon, jota suositellaan kaikille asiakkaille. Perusaikataulun käytännöt ovat joukko esimääritettyjä käytäntöjä, jotka auttavat suojaamaan organisaatioita monista yleisistä hyökkäyksistä. Näitä yleisiä hyökkäyksiä voivat olla Sala sanan suihkutus, uusinta toisto ja tietojenkalastelu.

Nämä käytännöt edellyttävät, että järjestelmänvalvojat ja käyttäjät syöttäisivät toisen todennus muodon (jota kutsutaan nimellä Monivaiheinen todennus tai MFA), kun tietyt ehdot täyttyvät. Jos käyttäjä on esimerkiksi kirjauduttava sisään toisesta maasta, kirjautumista voidaan pitää riskialttiina ja käyttäjän on annettava lisä todennus muoto. 

Tällä hetkellä perusaikataulun käytäntöjä ovat seuraavat:
- **Edellytä, että järjestelmänvalvojien** &ndash; MFA edellyttää usean tekijän todennusta etuoikeutetuimpia järjestelmänvalvojan rooleja varten, mukaan lukien yleinen järjestelmänvalvoja.
- **Loppu käyttäjän suojaus** &ndash; vaatii usean tekijän todennuksen käyttäjille vain silloin, kun kirjautuminen on riskialtista. 
- **Estä vanha todennus** &ndash; vanhemmat asiakas sovellukset ja jotkin uudet sovellukset eivät käytä uudempia, turvallisempia todennus protokollia. Nämä vanhemmat sovellukset voivat ohittaa ehdolliset käyttö käytännöt ja käyttää ympäristöäsi luvattomasti. Tämä käytäntö estää pääsyn asiakkailta, jotka eivät tue ehdollista pääsyä. 
- **Vaadi MFA for Service Management** &ndash; edellyttää monivaiheista todennusta, jotta voit käyttää hallinta työkaluja, mukaan lukien Azure Portal (jossa määrität peruskäytännöt). 

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

Voit määrittää useita lisä käytäntöjä, kuten hyväksyttyjen asiakas sovellusten vaatiminen. Lisä tietoja on [ehdollisen käyttö oikeus dokumentaatiossa](https://docs.microsoft.com/azure/active-directory/conditional-access/).
