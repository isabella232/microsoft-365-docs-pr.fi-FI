---
title: Miten Microsoft 365 Businessin suojausominaisuudet vastaavat Intunen asetuksia
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: aad21b1a-c775-469a-b89c-c5d1d59d27db
description: Lue kuinka suojausominaisuudet 365 Microsoft Business yhdistetään Intune asetukset. Tilaus sisältää käyttöoikeuden Intune-asetusten muuttamista.
ms.openlocfilehash: a6aaf6cc06c31b870eb85582f5aa47699919d75d
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074256"
---
# <a name="how-do-protection-features-in-microsoft-365-business-map-to-intune-settings"></a>Miten Microsoft 365 Businessin suojausominaisuudet vastaavat Intunen asetuksia

## <a name="android-and-ios-application-protection-settings"></a>Android- ja iOS-sovelluksen suojausasetukset

Seuraavassa taulukossa kuvataan seikkaperäisesti, miten Android- ja iOS-sovelluksen käytäntöasetukset yhdistetään Intune-asetuksiin.
  
Löydät Intune-asetuksen, kun olet kirjautuneena Microsoft 365 Business -järjestelmänvalvojana, valitsemalla ensin **Hallintakeskukset** ja sitten **Intune**.
  
 **Tärkeää:** Microsoft 365 Business-tilaus sisältää käyttöoikeuden Intune asetusten muuttamiseen. Katso [esittely Intune aloittamiseen.](https://docs.microsoft.com/intune/introduction-intune)
  
Napsauta sen käytännön nimeä, jonka haluat valita, esimerkiksi Androidin sovelluskäytäntö. Valitse sitten **Käytäntöasetukset**.
  
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
|Vaihda PIN-koodi, kun sisäänkirjautuminen epäonnistuu näin monta kertaa (tämä poistetaan käytöstä, jos PIN-koodi ei ole pakollinen)  <br/> |Yritysten määrä ennen PIN-koodin vaihtamista  <br/> |
|Vaadi käyttäjiä kirjautumaan sisään uudestaan, kun Office-sovelluksia ei ole käytetty näin pitkään aikaan (tämä poistetaan käytöstä, jos PIN-koodi ei ole pakollinen)  <br/> | Tarkista käyttövaatimukset uudelleen näin pitkän ajan jälkeen (minuuttia)  <br/>  Tämä määrittää myös seuraavat asetukset:  <br/> **Aikakatkaisu**-asetuksena on minuutit  <br/>  Tämä on sama minuuttimäärä, jonka määritit Microsoft 365 Businessssa.  <br/> **Offline-lisäaika**-asetuksena on oletusarvoisesti 720 minuuttia  <br/> |
|Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu  <br/> |Estä hallittujen sovellusten käyttö laitteissa, joiden suojaukset on murrettu  <br/> |
|Salli käyttäjille sisällön kopiointi Office-sovelluksista henkilökohtaisiin sovelluksiin  <br/> | Rajoita leikkaamista, kopioimista ja liittämistä muiden sovellusten kanssa  <br/>  Jos Microsoft 365 Business -asetuksena on **Käytössä**, seuraavan kolmen asetuksen määrityksenä on myös **Kaikki sovellukset** Intunessa:  <br/> **Salli sovelluksen siirtää tietoja toisiin sovelluksiin** <br/> **Salli sovelluksen saada tietoja toisista sovelluksista** <br/> **Rajoita leikkaamista, kopioimista ja liittämistä muiden sovellusten kanssa** <br/>  Jos Microsoft 365 Business -asetuksena on **Käytössä**, kaikki Intune-asetukset ovat seuraavat:  <br/> **Salli sovelluksen siirtää tietoja toisiin sovelluksiin** -asetuksena on **Käytännön mukaisesti hallitut sovellukset** <br/> **Salli sovelluksen saada tietoja muista sovelluksista** -asetuksena on **Kaikki sovellukset** <br/> **Rajoita leikkaamista, kopioimista ja liittämistä muiden sovellusten kanssa** -asetuksena on **Käytännön mukaisesti hallitut sovellukset Liitä-komennon kanssa** <br/> |
|||
   
## <a name="windows-10-app-protection-settings"></a>Windows 10 -sovelluksen suojausasetukset

Seuraavassa taulukossa kuvataan seikkaperäisesti, miten Windows 10 -sovelluksen käytäntöasetukset yhdistetään Intune-asetuksiin.
  
Etsi Intune asetus, kun kirjautunut sisään Microsoft 365 Business järjestelmänvalvojan tunnistetiedot, siirry [Azure portal](https://portal.azure.com)ja valitse Valitse **useita palveluja**ja Intune **suodattimen**tyyppi **Intune App suojaa** \> ** App käytännön**.
  
 **Tärkeää**: Microsoft 365 Business -tilaus antaa sinulle lisenssin, jolla voit muokata vain niitä Intune-asetuksia, jotka on yhdistetty Microsoft 365 Businessissa käytettävissä oleviin asetuksiin. 
  
Napsauta sen käytännön nimeä, jonka haluat valita, ja tarkastele sitten käytettävissä olevia asetuksia valitsemalla **Yleistä, tehtävät**, **Sallitut sovellukset**, **Vapautetut sovellukset**, **Pakolliset asetukset** tai **Lisäasetukset** vasemmasta siirtymispalkista. 
  
|**Windows 10 -sovelluksen käytäntöasetus**|**Intune-asetus**|
|:-----|:-----|
|Salaa työtiedostot  <br/> |**Lisäasetukset** \> **Tietosuoja**: Sekä **Kumoa salausavaimet rekisteröitymisen yhteydessä**- että **Kumoa pääsy suojatun tietolaitteen rekisteröitymiseen MDM:een** -kohdan asetuksena on **Käytössä**.  <br/> |
|Estä käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin.  <br/> |**Pakolliset asetukset** \> **Windowsin tietojensuojaus -tila**. **Käytössä**Microsoft 365 Businessssa yhdistää seuraavaan: **Piilota ohitukset**, **Pois käytöstä**Microsoft 365 Businessssa yhdistää seuraavaan: **Pois käytöstä**.  <br/> |
|Office-asiakirjojen käytön hallinta  <br/> | Jos tämän asetuksena on **Käytössä**Microsoft 365 Businessssa, silloin  <br/> **Lisäasetukset** \> **Käyttö**, **Käytä Windows Hello for Businessia kirjautumismenetelmänä Windowsiin** -asetuksena on **Käytössä** seuraavilla lisäasetuksilla:  <br/> **Määritä PIN-koodille pakollinen vähimmäismerkkimäärä** -asetuksena on **4**.  <br/> **Konfiguroi isojen kirjainten käyttö Windows Hello for Businessin PIN-koodissa** -asetuksena on **Älä salli isojen kirjainten käyttöä PIN-koodille**.  <br/> **Konfiguroi pienten kirjainten käyttö Windows Hello for Businessin PIN-koodissa** -asetuksena on **Älä salli pienten kirjainten käyttöä PIN-koodille**.  <br/> **Konfiguroi erityismerkkien käyttö Windows Hello for Businessin PIN-koodissa** -asetuksena on **Älä salli erityismerkkien käyttöä PIN-koodille**.  <br/> **Määritä ajanjakso (päivää), jolloin PIN-koodia voidaan käyttää, ennen kuin järjestelmä vaatii käyttäjää muuttamaan** sen asetukseksi **0**.  <br/> **Määritä niiden aiempien PIN-koodien määrä, jotka voidaan liittää käyttäjätiliin, jota ei voida käyttää uudelleen** -asetuksena on **0**.  <br/> **Niiden sallittujen todennusvirheiden määrä, ennen kuin laite poistetaan** -asetuksena on sama kuin Microsoft 365 Businessssa (oletusarvoisesti 5).  <br/> **Kun laite on ollut käyttämättömänä, sallittu enimmäisaika (minuuttia), jonka jälkeen laitteen PIN-koodi tai salasana lukitaan** -asetuksena on sama kuin Microsoft 365 Businessssa.  <br/> |
|Ota käyttöön suojattujen tietojen palauttaminen  <br/> |**Lisäasetukset** \> **Tietosuoja**: **Näytä yritystietojen suojauksen kuvake**- ja **Käytä Azure RMS:ää WIP:lle** -asetuksena on **Käytössä**.  <br/> |
|Suojaa lisää yrityksen pilvipalvelusijainteja  <br/> |**Lisäasetukset** \> **Suojatut toimialueet** ja **Pilviresurssit** näyttävät toimialueet ja SharePoint-sivustot.  <br/> |
|Näiden sovellusten käyttämät tiedostot on suojattu  <br/> |Suojattujen sovellusten luettelo löytyy kohdasta **Sallitut sovellukset**.  <br/> |
|||
   
## <a name="windows-10-device-protection-settings"></a>Windows 10 -laitteen suojausasetukset

Seuraavassa taulukossa kuvataan seikkaperäisesti, miten Windows 10 -laitteen konfigurointiasetukset yhdistetään Intune-asetuksiin.
  
Etsi Intune asetus, kun kirjautunut sisään Microsoft 365 Business järjestelmänvalvojan tunnistetiedot, siirry [Azure portal](https://portal.azure.com)ja valitse Valitse **useita palveluja**ja Intune **suodattimen**tyyppi **Intune** \> laitteen ** kokoonpanon** \> **profiilit**. Valitse **laite-käytännön Windows 10** \> **Ominaisuudet** \> **asetukset**.
  
|**Windows 10 -laitteen käytäntöasetus**|**Intune-asetus**|
|:-----|:-----|
|Auta suojaamaan tietokoneita viruksilta ja muilta uhkilta käyttämällä Windows Defenderin virustentorjuntaa  <br/> |Salli reaaliaikainen valvominen = KÄYTÖSSÄ  <br/> Salli pilvipalvelun suojaus = KÄYTÖSSÄ  <br/> Pyydä käyttäjiä lähettämään näytteitä = Lähetä suojatut näytteet automaattisesti (oletuksena Ei PII:n automaattista lähetystä)  <br/> |
|Auta suojaamaan tietokoneita verkkopohjaisilta uhilta Microsoft Edgessä  <br/> |**Edge-selainasetukset**-kohdan **SmartScreen**-asetuksena on **Pakollinen**.  <br/> |
|Sammuta laitteen näyttö, kun se on ollut käyttämättömänä tämän verran (minuuttia)  <br/> |Kun näyttö on ollut käyttämättömänä, enimmäisaika minuutteina, ennen kuin näyttö lukkiutuu (minuuttia)  <br/> |
|Salli käyttäjille sovellusten lataaminen Microsoft Storesta  <br/> |Mukautettu URI-käytäntö  <br/> |
|Salli käyttäjien käyttää Cortanaa  <br/> |**Yleistä** \> **Cortana**-asetuksena on **Estä** Intunessa, kun asetuksena on **Pois käytöstä**Microsoft 365 Businessssa.  <br/> |
|Salli käyttäjille Windows-vihjeiden ja -mainosten vastaanottaminen Microsoftilta  <br/> |**Windows-tapahtumanäyttö**, kaikki estetään, jos tämän asetuksena on **Pois käytöstä**Microsoft 365 Businessssa.  <br/> |
|Pidä Windows 10 -laitteet ajan tasalla automaattisesti  <br/> | Tämä asetus on kohdassa **Microsoft Intune** \> **Palvelupäivitykset - Windows 10 -päivityskierrokset**. Valitse **Windows 10 -laitteiden päivityskäytäntö** ja sitten **Ominaisuudet** \> **Asetukset**.      <br/>  Kun Microsoft 365 Business -asetuksena on **Pois käytöstä**, kaikki seuraavat asetukset on määritetty:  <br/> **Palveluhaara**-asetuksena on **CB** (CBB, kun se on poistettu käytöstä Microsoft 365 Businessssa).  <br/> **Microsoft-tuotepäivitykset**-asetuksena on **Salli**.  <br/> **Windows-ohjaimet**-asetuksena on **Salli**.  <br/> **Automaattinen päivityskäytäntö** -asetuksena on **Automaattinen asennus huoltoaikana**, jossa:  <br/> **Tuntia käynnistyksestä** -asetuksena on **klo 6.00**.  <br/> **Aktiivisten tuntien päättyminen** -asetuksena on **klo 22.00**.  <br/> **Laadun päivityksen jaksotusaika (päivää)** -asetuksena on **0**.  <br/> **Ominaisuuden päivityksen jaksotusaika (päivää)** -asetuksena on **0**.  <br/> **Toimituksen optimoinnin lataustila** -asetuksena on **HTTP yhdistetty samaan NAT-vertaisverkkoon**.  <br/> |
|||
   

