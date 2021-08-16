---
title: Miten Microsoft 365 Business Premium suojausominaisuudet voidaan yhdistää Intune-asetuksiin
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
ms.date: 8/13/2018
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: aad21b1a-c775-469a-b89c-c5d1d59d27db
description: Lue, miten Microsoft 365 Business Premium suojausominaisuudet voidaan yhdistää Intune-asetuksiin. Tilauksella on käyttöoikeus Intunen asetusten muokkaamista varten.
ms.openlocfilehash: 844b83bca9483f72fd322d666803c42b90fee41d3e0047ea93b4b6b07717b0dd
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53852727"
---
# <a name="how-do-protection-features-in-microsoft-365-business-premium-map-to-intune-settings"></a>Miten Microsoft 365 Business Premium suojausominaisuudet voidaan yhdistää Intune-asetuksiin

## <a name="android-and-ios-application-protection-settings"></a>Android- ja iOS-sovelluksen suojausasetukset

Seuraavassa taulukossa kuvataan seikkaperäisesti, miten Android- ja iOS-sovelluksen käytäntöasetukset yhdistetään Intune-asetuksiin.
  
Voit etsiä Intune-asetuksen kirjautumalla sisään Microsoft 365 Business Premium tunnistetiedoilla, valitsemalla Hallintakeskukset **ja** sitten **Intune**.
  
 > [!IMPORTANT]
 > 
 > A Microsoft 365 Business Premium subscription gives you a license to modify all the Intune settings. Aloita [tutustuminen intunen esittelyssä.](/intune/introduction-intune)
  
Valitse haluamasi käytännön &mdash; nimi, esimerkiksi Androidin &mdash; sovelluskäytäntö, ja valitse sitten **Käytäntöasetukset**.
  
Kohdasta **Suojaa työtiedostoja laitteiden katoamisen tai varastamisen varalta**
  
|**Android- tai iOS-sovelluksen käytäntöasetus**|**Intune-asetus**|
|:-----|:-----|
|Poista työtiedostot passiivisesta laitteesta näin monen päivän kuluttua  <br/> |Offline-aikaväli (päivää), ennen kuin sovellustiedot poistetaan  <br/> |
|Pakota käyttäjät tallentamaan työtiedostot OneDrive for Businessiin  <br/> Huomaa, että vain OneDrive for Business on sallittu  <br/> |Valitse, mihin tallennuspalveluihin yritystiedot voidaan tallentaa  <br/> |
|||
   
Kohdasta **Hallitse käyttäjien Office-tiedostojen käyttöä mobiililaitteissa**
  
|**Android- tai iOS-sovelluksen käytäntöasetus**|**Intune-asetus**|
|:-----|:-----|
|Poista työtiedostot passiivisesta laitteesta näin monen päivän kuluttua  <br/> |Offline-aikaväli (päivää), ennen kuin sovellustiedot poistetaan  <br/> |
|Pakota käyttäjät tallentamaan työtiedostot OneDrive for Businessiin  <br/> Huomaa, että vain OneDrive for Business on sallittu  <br/> |Valitse, mihin tallennuspalveluihin yritystiedot voidaan tallentaa  <br/> |
|Salaa työtiedostot  <br/> |Salaa sovellustiedot  <br/> |
|Kohdasta **Hallitse käyttäjien Office-tiedostojen käyttöä mobiililaitteissa** <br/> ||
|Edellytä PIN-koodia tai sormenjälkeä Office-sovellusten käyttämiseksi  <br/> | Edellytä PIN-koodia sovellusten käyttämiseksi  <br/>  Tämä määrittää myös seuraavat asetukset:  <br/> **Salli yksinkertainen PIN-koodi** -asetuksena on **Kyllä** <br/> **PIN-koodin pituus** -asetuksena on 4  <br/> **Salli sormenjälki PIN-koodin sijasta** -asetuksena on **Kyllä** <br/> **Poista sovelluksen PIN-koodi käytöstä, kun PIN-koodia hallitaan** -asetuksena on **Ei** <br/> |
|Palauta PIN-koodi kirjautumisen epäonnistuessa näin monta kertaa (tämä poistetaan käytöstä, jos PIN-koodia ei tarvita)  <br/> |Yritysten määrä ennen PIN-koodin vaihtamista  <br/> |
|Vaadi käyttäjiä kirjautumaan uudelleen, kun Office on ollut käyttämättömänä (tämä on poistettu käytöstä, jos PIN-koodi ei ole pakollinen)  <br/> | Tarkista käyttövaatimukset uudelleen näin pitkän ajan jälkeen (minuuttia)  <br/>  Tämä määrittää myös seuraavat asetukset:  <br/> **Aikakatkaisu**-asetuksena on minuutit  <br/>  Tämä on sama minuuttimäärä, jonka määritit Microsoft 365 Businessssa.  <br/> **Offline-lisäaika**-asetuksena on oletusarvoisesti 720 minuuttia  <br/> |
|Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu  <br/> |Estä hallittujen sovellusten käyttö laitteissa, joiden suojaukset on murrettu  <br/> |
|Salli käyttäjille sisällön kopiointi Office-sovelluksista henkilökohtaisiin sovelluksiin  <br/> | Rajoita leikkaamista, kopioimista ja liittämistä muiden sovellusten kanssa  <br/>  Jos Microsoft 365 Business Premium -asetuksena on **Käytössä**, nämä kolme asetusta  ovat myös Kaikki sovellukset Intunessa:  <br/> **Salli sovelluksen siirtää tietoja toisiin sovelluksiin** <br/> **Salli sovelluksen saada tietoja toisista sovelluksista** <br/> **Rajoita leikkaamista, kopioimista ja liittämistä muiden sovellusten kanssa** <br/>  Jos Microsoft 365 Business -asetuksena on **Käytössä**, kaikki Intune-asetukset ovat seuraavat:  <br/> **Salli sovelluksen siirtää tietoja toisiin sovelluksiin** -asetuksena on **Käytännön mukaisesti hallitut sovellukset** <br/> **Salli sovelluksen saada tietoja muista sovelluksista** -asetuksena on **Kaikki sovellukset** <br/> **Rajoita leikkaamista, kopioimista ja liittämistä muiden sovellusten kanssa** -asetuksena on **Käytännön mukaisesti hallitut sovellukset Liitä-komennon kanssa** <br/> |
|||
   
## <a name="windows-10-app-protection-settings"></a>Windows 10 -sovelluksen suojausasetukset

Seuraavassa taulukossa kuvataan seikkaperäisesti, miten Windows 10 -sovelluksen käytäntöasetukset yhdistetään Intune-asetuksiin.
  
Voit etsiä Intune-asetuksen kirjautumalla sisään Microsoft 365 Business Premium tunnistetiedoilla ja valitsemalla [Azure-portaalin.](https://portal.azure.com) Valitse **Lisää palveluita** ja kirjoita Intune **Suodatin-ruutuun.** Valitse **Intune-sovelluksen** \> **suojaussovelluksen käytäntö**.
  
 > [!IMPORTANT]
 >
 >A Microsoft 365 Business Premium subscription gives you a license to modify only the Intune settings that map to the settings available to the settings available in Microsoft 365 Business Premium. 
  
Voit tarkastella käytettävissä olevia asetuksia valitsemalla haluamasi käytännön nimen ja valitsemalla sitten vasemman siirtymisruudun  **Yleiset,** Tehtävät **,** Sallitut sovellukset **,** Vapautetut sovellukset **,** Pakolliset asetukset tai Lisäasetukset. 
  
|**Windows 10 -sovelluksen käytäntöasetus**|**Intune-asetus**|
|:-----|:-----|
|Salaa työtiedostot  <br/> |**Lisäasetukset** \> **Tietosuoja**: Sekä **Kumoa salausavaimet rekisteröitymisen yhteydessä**- että **Kumoa pääsy suojatun tietolaitteen rekisteröitymiseen MDM:een** -kohdan asetuksena on **Käytössä**.  <br/> |
|Estä käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin.  <br/> |**Pakolliset asetukset** \> **Windowsin tietojensuojaus -tila**. **Käytössä** Microsoft 365 Business Premium: Piilota **ohitukset** **,** Ei käytössä Microsoft 365 Business Premium kartat: **Ei käytössä**.  <br/> |
|Office-asiakirjojen käytön hallinta  <br/> | Jos tämän asetuksena **on Käytössä** Microsoft 365 Business Premium,  <br/> **Lisäasetukset** \> **Käyttö**, **Käytä Windows Hello for Businessia kirjautumismenetelmänä Windowsiin** -asetuksena on **Käytössä** seuraavilla lisäasetuksilla:  <br/> **Määritä PIN-koodille pakollinen vähimmäismerkkimäärä** -asetuksena on **4**.  <br/> **Konfiguroi isojen kirjainten käyttö Windows Hello for Businessin PIN-koodissa** -asetuksena on **Älä salli isojen kirjainten käyttöä PIN-koodille**.  <br/> **Konfiguroi pienten kirjainten käyttö Windows Hello for Businessin PIN-koodissa** -asetuksena on **Älä salli pienten kirjainten käyttöä PIN-koodille**.  <br/> **Konfiguroi erityismerkkien käyttö Windows Hello for Businessin PIN-koodissa** -asetuksena on **Älä salli erityismerkkien käyttöä PIN-koodille**.  <br/> **Määritä, kuinka kauan (päivinä)** PIN-koodia voidaan käyttää, ennen kuin järjestelmä edellyttää käyttäjän vaihtamista arvoksi **0.**  <br/> **Määritä niiden aiempien PIN-koodien määrä, jotka voidaan liittää käyttäjätiliin, jota ei voida käyttää uudelleen** -asetuksena on **0**.  <br/> **Niiden sallittujen todennusvirheiden määrä, ennen kuin laite poistetaan** -asetuksena on sama kuin Microsoft 365 Businessssa (oletusarvoisesti 5).  <br/> **Kun laite on ollut käyttämättömänä, sallittu enimmäisaika (minuuttia), jonka jälkeen laitteen PIN-koodi tai salasana lukitaan** -asetuksena on sama kuin Microsoft 365 Businessssa.  <br/> |
|Ota käyttöön suojattujen tietojen palauttaminen  <br/> |**Lisäasetukset** \> **Tietosuoja**: **Näytä yritystietojen suojauksen kuvake**- ja **Käytä Azure RMS:ää WIP:lle** -asetuksena on **Käytössä**.  <br/> |
|Suojaa lisää yrityksen pilvipalvelusijainteja  <br/> |**Lisäasetukset** \> **Suojatut toimialueet** ja **Pilviresurssit** näyttävät toimialueet ja SharePoint-sivustot.  <br/> |
|Näiden sovellusten käyttämät tiedostot on suojattu  <br/> |Suojattujen sovellusten luettelo löytyy kohdasta **Sallitut sovellukset**.  <br/> |
|||
   
## <a name="windows-10-device-protection-settings"></a>Windows 10 -laitteen suojausasetukset

Seuraavassa taulukossa kuvataan seikkaperäisesti, miten Windows 10 -laitteen konfigurointiasetukset yhdistetään Intune-asetuksiin.
  
Jos haluat etsiä Intune-asetuksen, kirjaudu sisään Microsoft 365 Business Premium-järjestelmänvalvojan tunnistetiedoilla, siirry Azure-portaaliin, valitse Lisää **palveluita** ja kirjoita Intune Suodatin -ruutuun **ja** valitse [](https://portal.azure.com)  Intune-laitemääritysprofiilit \>  \> . Valitse sitten **Laitekäytäntö kohdassa Windows 10** \>  \> **ominaisuudet Asetukset.**
  
|**Windows 10 -laitteen käytäntöasetus**|**Intune-asetus**|
|:-----|:-----|
|Auta suojaamaan tietokoneita viruksilta ja muilta uhkilta käyttämällä Windows Defenderin virustentorjuntaa  <br/> |Salli reaaliaikainen valvominen = KÄYTÖSSÄ  <br/> Salli pilvipalvelun suojaus = KÄYTÖSSÄ  <br/> Pyydä käyttäjiä lähettämään näytteitä = Lähetä suojatut näytteet automaattisesti (oletuksena Ei PII:n automaattista lähetystä)  <br/> |
|Auta suojaamaan tietokoneita verkkopohjaisilta uhilta Microsoft Edgessä  <br/> |**Edge-selainasetukset**-kohdan **SmartScreen**-asetuksena on **Pakollinen**.  <br/> |
|Sammuta laitteen näyttö, kun se on ollut käyttämättömänä tämän verran (minuuttia)  <br/> |Kun näyttö on ollut käyttämättömänä, enimmäisaika minuutteina, ennen kuin näyttö lukkiutuu (minuuttia)  <br/> |
|Salli käyttäjille sovellusten lataaminen Microsoft Storesta  <br/> |Mukautettu URI-käytäntö  <br/> |
|Salli käyttäjien käyttää Cortanaa  <br/> |**Yleiset** \> **Cortana** on määritetty **estämaan** Intunessa, kun asetus **on poissa käytöstä** Microsoft 365 Business Premium.  <br/> |
|Salli käyttäjille Windows-vihjeiden ja -mainosten vastaanottaminen Microsoftilta  <br/> |**Windows esittelyssä**, kaikki estetään, jos asetuksena **on Ei käytössä** Microsoft 365 Business Premium.  <br/> |
|Pidä Windows 10 -laitteet ajan tasalla automaattisesti  <br/> | Tämä asetus on **kohdassa Microsoft Intune** palvelupäivitykset – Windows 10 päivitys rings , valitse \>  **päivityskäytäntö Windows 10 -laitteille** ja valitse **sitten** \> **Ominaisuudet Asetukset**.  <br/>  Kun Microsoft 365 Business Premium asetukseksi **on määritetty Käytössä,** kaikki seuraavat asetukset on määritetty:  <br/> **Palveluhaara-asetuksena** **on CB** (CBB, kun tämä asetus on poistettu käytöstä Microsoft 365 Business Premium).  <br/> **Microsoft-tuotepäivitykset**-asetuksena on **Salli**.  <br/> **Windows-ohjaimet**-asetuksena on **Salli**.  <br/> **Automaattinen päivityskäytäntö** -asetuksena on **Automaattinen asennus huoltoaikana**, jossa:  <br/> **Tuntia käynnistyksestä** -asetuksena on **klo 6.00**.  <br/> **Aktiivisten tuntien päättyminen** -asetuksena on **klo 22.00**.  <br/> **Laadun päivityksen jaksotusaika (päivää)** -asetuksena on **0**.  <br/> **Ominaisuuden päivityksen jaksotusaika (päivää)** -asetuksena on **0**.  <br/> **Toimituksen optimoinnin lataustila** -asetuksena on **HTTP yhdistetty samaan NAT-vertaisverkkoon**.  <br/> |
|||
