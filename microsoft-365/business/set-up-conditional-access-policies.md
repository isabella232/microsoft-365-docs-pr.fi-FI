---
title: Ehdollisen käyttöoikeuden Microsoft 365 kampanjoiden käytäntöjen määrittäminen
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
search.appverid:
- BCS160
- MET150
- MOE150
description: Tietoja ehdollisen käyttöoikeuden käytäntöjen määrittäminen Microsoft 365 kampanjoita.
ms.openlocfilehash: 7d8e1f16019d151478aae57b1593b0e0758e5b19
ms.sourcegitcommit: 7e46db0b35c188ee6a7b40ab3eb2d76ff6c101c5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/19/2019
ms.locfileid: "35086321"
---
# <a name="set-up-conditional-access-policies"></a>Ehdollisen käyttöoikeuden käytäntöjen määrittäminen

[Ehdollisen käyttöoikeuden](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) käytäntöjä lisätä substancial suojausta. Microsoft tarjoaa joukon perusaikataulun ehdollisen käyttöoikeuden käytäntöjä, joita suositellaan kaikille asiakkaille. Perusaikataulun käytännöt ovat valmiita käytäntöjä, jotka suojaavat hyökkäyksiltä monia yhteisiä organisaatioita. Yleisiä nämä hyökkäykset voivat olla salasana ruiskun, replay ja phishing.

Nämä käytännöt edellyttävät Järjestelmänvalvojat ja käyttäjät voivat syöttää toisen lomakkeen todennusta (jota kutsutaan useaan tekijään perustuvan todennuksen tai MFA) kun tietyt ehdot täyttyvät. Esimerkiksi jos käyttäjä sisään eri maasta, kirjautumissivulta voidaan harkita riskialtis ja käyttäjän on annettava todennusta uuden lomakkeen. 

Perusaikataulun käytännöt ovat tällä hetkellä seuraavat:
- **MFA edellyttävät järjestelmänvalvojat** – edellyttää monitasoisen todennuksen ensisijaisessa järjestelmänvalvoja-roolien mukaan lukien Yleinen järjestelmänvalvoja.
- **Käyttäjän suojaus** — vaatii monitasoisen todennuksen käyttäjille vain, kun jokin merkki on riskialtista. 
- **Vanhan mallin mukainen todennus estää** — vanhemmat asiakassovellukset ja joitakin uusia apps et käytä uudempia, turvallisempia, todennusprotokollia. Nämä vanhat apps voit ohittaa ehdollisen käyttöoikeuden käytäntöjä ja ympäristön yrityksiin hankkia luvaton pääsy. Tämä käytäntö estää käytön asiakkailta, jotka eivät tue ehdollisen käyttöoikeuden. 
- **Huoltohallinnan edellyttävät MFA** — monitasoisen todennuksen vaatii pääsyä hallintatyökaluihin, mukaan lukien Azure portal (jossa voit määrittää perusaikataulun käytännöt). 

Microsoft suosittelee, että otat kaikki nämä käytännöt perusaikataulun. Kun nämä käytännöt on otettu käyttöön, järjestelmänvalvojat- ja käyttäjät pyydetään rekisteröitymään Multii Azure-tekijä authentication.

Lisätietoja näistä käytännöistä Katso [mitä perusaikataulun käytännöt ovat](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Perusaikataulun käytäntöjen määrittäminen

1. Siirry [Azure portal](https://portal.azure.com)ja siirry **Azure Active Directory** \> **Ehdollisen käyttöoikeuden**.
    
    Perusaikataulun käytännöt on lueteltu sivulla. <br/> <br/>
    ![Ehdollisen käyttöoikeuden käytäntöjä perusaikataulun sisältävällä sivulla.](media/baslinepolicies.png)
1. Lisätietoja käytäntöjen seuraavat ohjeet:

  - [MFA edellyttävät Järjestelmänvalvojat](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Reequire MFA-käyttäjille](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Estä vanhan mallin mukainen todennus](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Vaadi MFA hallinta](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Voit määrittää useita muita käytäntöjä esimerkiksi asiakkaan hyväksytyn apps. Katso lisätietoja [Ehdollinen Access in ohjeista](https://docs.microsoft.com/azure/active-directory/conditional-access/) .