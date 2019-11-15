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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: aad21b1a-c775-469a-b89c-c5d1d59d27db
description: Tutustu Microsoft 365-yritys kartan suojaus ominaisuuksiin Intune-asetuksiin. Tilaus antaa sinulle käyttö oikeuden muokata Intune asetuksia.
ms.openlocfilehash: b7d87e9a174e942a6533ae034b4f4a551ae2159f
ms.sourcegitcommit: 9a057e70637dcfe06d4f729a96c02be989cf9e25
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/14/2019
ms.locfileid: "38633285"
---
# <a name="how-do-protection-features-in-microsoft-365-business-map-to-intune-settings"></a>Miten Microsoft 365 Businessin suojausominaisuudet vastaavat Intunen asetuksia

## <a name="android-and-ios-application-protection-settings"></a>Android- ja iOS-sovelluksen suojausasetukset

Seuraavassa taulukossa kuvataan seikkaperäisesti, miten Android- ja iOS-sovelluksen käytäntöasetukset yhdistetään Intune-asetuksiin.
  
Jos haluat löytää Intune-asetuksen, kirjaudu sisään Microsoft 365-yrityksen järjestelmänvalvojan tunniste tiedoilla ja siirry **hallinta keskuksiin**ja sitten **Intune**.
  
 > [!IMPORTANT]
 > 
 > Microsoft 365 Business-tilaus antaa sinulle oikeuden muokata kaikkia Intune asetuksia. Katso [esittely Intune päästä alkuun.](https://docs.microsoft.com/intune/introduction-intune)
  
Valitse haluamasi &mdash; käytännön nimi esimerkiksi Android &mdash; -sovellus käytännölle ja valitse sitten **käytäntö asetukset**.
  
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
|Nollaa PIN kun kirjautuminen epäonnistuu tämän monta kertaa (tämä ei ole käytössä, jos PIN ei tarvita)  <br/> |Yritysten määrä ennen PIN-koodin vaihtamista  <br/> |
|Vaadi käyttäjiä Kirjautu maan uudelleen sisään, kun Office-sovellukset ovat olleet käyttämättömänä (tämä ei ole käytössä, jos PIN-koodia ei tarvita)  <br/> | Tarkista käyttövaatimukset uudelleen näin pitkän ajan jälkeen (minuuttia)  <br/>  Tämä määrittää myös seuraavat asetukset:  <br/> **Aikakatkaisu**-asetuksena on minuutit  <br/>  Tämä on sama minuuttimäärä, jonka määritit Microsoft 365 Businessssa.  <br/> **Offline-lisäaika**-asetuksena on oletusarvoisesti 720 minuuttia  <br/> |
|Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu  <br/> |Estä hallittujen sovellusten käyttö laitteissa, joiden suojaukset on murrettu  <br/> |
|Salli käyttäjille sisällön kopiointi Office-sovelluksista henkilökohtaisiin sovelluksiin  <br/> | Leikkaa, kopioi ja liitä muiden sovellusten kanssa  <br/>  Jos Microsoft 365 Business -asetuksena on **Käytössä**, seuraavan kolmen asetuksen määrityksenä on myös **Kaikki sovellukset** Intunessa:  <br/> **Salli sovelluksen siirtää tietoja toisiin sovelluksiin** <br/> **Salli sovelluksen saada tietoja toisista sovelluksista** <br/> **Rajoita leikkaamista, kopioimista ja liittämistä muiden sovellusten kanssa** <br/>  Jos Microsoft 365 Business -asetuksena on **Käytössä**, kaikki Intune-asetukset ovat seuraavat:  <br/> **Salli sovelluksen siirtää tietoja toisiin sovelluksiin** -asetuksena on **Käytännön mukaisesti hallitut sovellukset** <br/> **Salli sovelluksen saada tietoja muista sovelluksista** -asetuksena on **Kaikki sovellukset** <br/> **Rajoita leikkaamista, kopioimista ja liittämistä muiden sovellusten kanssa** -asetuksena on **Käytännön mukaisesti hallitut sovellukset Liitä-komennon kanssa** <br/> |
|||
   
## <a name="windows-10-app-protection-settings"></a>Windows 10 -sovelluksen suojausasetukset

Seuraavassa taulukossa kuvataan seikkaperäisesti, miten Windows 10 -sovelluksen käytäntöasetukset yhdistetään Intune-asetuksiin.
  
Voit etsiä Intune-asetuksen kirjautumalla sisään Microsoft 365-yrityksen järjestelmänvalvojan tunniste tiedoilla ja siirtymällä [Azure-portaaliin](https://portal.azure.com). Valitse **Lisää palveluita**ja kirjoita Intune **suodattimeen**. Valitse **Intune App Protection** \> - **sovellus käytäntö**.
  
 > [!IMPORTANT]
 >
 >Microsoft 365 Business-tilaus antaa sinulle oikeuden muokata vain Intune-asetuksia, jotka on tehty Microsoft 365 Businessissa käytettävissä olevien asetusten mukaan. 
  
Jos haluat tutustua käytettävissä oleviin asetuksiin, valitse haluamasi käytännön nimi ja valitse vasemmasta siirtymis ruudusta **Yleiset, vara ukset**, **Sallitut sovellukset**, **vapautetut sovellukset**, **pakolliset asetukset**tai **lisä asetukset** . 
  
|**Windows 10 -sovelluksen käytäntöasetus**|**Intune-asetus**|
|:-----|:-----|
|Salaa työtiedostot  <br/> |**Lisäasetukset** \> **Tietosuoja**: Sekä **Kumoa salausavaimet rekisteröitymisen yhteydessä**- että **Kumoa pääsy suojatun tietolaitteen rekisteröitymiseen MDM:een** -kohdan asetuksena on **Käytössä**.  <br/> |
|Estä käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin.  <br/> |**Pakolliset asetukset** \> **Windowsin tietojensuojaus -tila**. Microsoft 365-yritys kartoissa: **Piilota ohitukset**, **ei käytössä** Microsoft 365 Business **-** kartoissa: **pois päältä**.  <br/> |
|Office-asiakirjojen käytön hallinta  <br/> | Jos tämän asetuksena on **Käytössä**Microsoft 365 Businessssa, silloin  <br/> **Lisäasetukset** \> **Käyttö**, **Käytä Windows Hello for Businessia kirjautumismenetelmänä Windowsiin** -asetuksena on **Käytössä** seuraavilla lisäasetuksilla:  <br/> **Määritä PIN-koodille pakollinen vähimmäismerkkimäärä** -asetuksena on **4**.  <br/> **Konfiguroi isojen kirjainten käyttö Windows Hello for Businessin PIN-koodissa** -asetuksena on **Älä salli isojen kirjainten käyttöä PIN-koodille**.  <br/> **Konfiguroi pienten kirjainten käyttö Windows Hello for Businessin PIN-koodissa** -asetuksena on **Älä salli pienten kirjainten käyttöä PIN-koodille**.  <br/> **Konfiguroi erityismerkkien käyttö Windows Hello for Businessin PIN-koodissa** -asetuksena on **Älä salli erityismerkkien käyttöä PIN-koodille**.  <br/> **Määritä ajan jakso (päivinä), jonka PIN-koodia voi käyttää, ennen kuin järjestelmä edellyttää** , että käyttäjän on muutettava arvoksi **0**.  <br/> **Määritä niiden aiempien PIN-koodien määrä, jotka voidaan liittää käyttäjätiliin, jota ei voida käyttää uudelleen** -asetuksena on **0**.  <br/> **Niiden sallittujen todennusvirheiden määrä, ennen kuin laite poistetaan** -asetuksena on sama kuin Microsoft 365 Businessssa (oletusarvoisesti 5).  <br/> **Kun laite on ollut käyttämättömänä, sallittu enimmäisaika (minuuttia), jonka jälkeen laitteen PIN-koodi tai salasana lukitaan** -asetuksena on sama kuin Microsoft 365 Businessssa.  <br/> |
|Ota käyttöön suojattujen tietojen palauttaminen  <br/> |**Lisäasetukset** \> **Tietosuoja**: **Näytä yritystietojen suojauksen kuvake**- ja **Käytä Azure RMS:ää WIP:lle** -asetuksena on **Käytössä**.  <br/> |
|Suojaa lisää yrityksen pilvipalvelusijainteja  <br/> |**Lisäasetukset** \> **Suojatut toimialueet** ja **Pilviresurssit** näyttävät toimialueet ja SharePoint-sivustot.  <br/> |
|Näiden sovellusten käyttämät tiedostot on suojattu  <br/> |Suojattujen sovellusten luettelo löytyy kohdasta **Sallitut sovellukset**.  <br/> |
|||
   
## <a name="windows-10-device-protection-settings"></a>Windows 10 -laitteen suojausasetukset

Seuraavassa taulukossa kuvataan seikkaperäisesti, miten Windows 10 -laitteen konfigurointiasetukset yhdistetään Intune-asetuksiin.
  
Voit etsiä Intune-asetuksen kirjautumalla sisään Microsoft 365-yrityksen järjestelmänvalvojan tunniste tiedoilla ja siirtymällä [Azure-portaaliin](https://portal.azure.com), valitsemalla **Lisää palveluita**ja kirjoittamalla Intunen **suodattimeen**, valitsemalla **Intune** \> - **laite määritys** \> **Profiilit**. Valitse sitten **laite käytäntö Windows 10** \> - **ominaisuuksien** \> **asetuksille**.
  
|**Windows 10 -laitteen käytäntöasetus**|**Intune-asetus**|
|:-----|:-----|
|Auta suojaamaan tietokoneita viruksilta ja muilta uhkilta käyttämällä Windows Defenderin virustentorjuntaa  <br/> |Salli reaaliaikainen valvominen = KÄYTÖSSÄ  <br/> Salli pilvipalvelun suojaus = KÄYTÖSSÄ  <br/> Pyydä käyttäjiä lähettämään näytteitä = Lähetä suojatut näytteet automaattisesti (oletuksena Ei PII:n automaattista lähetystä)  <br/> |
|Auta suojaamaan tietokoneita verkkopohjaisilta uhilta Microsoft Edgessä  <br/> |**Edge-selainasetukset**-kohdan **SmartScreen**-asetuksena on **Pakollinen**.  <br/> |
|Sammuta laitteen näyttö, kun se on ollut käyttämättömänä tämän verran (minuuttia)  <br/> |Kun näyttö on ollut käyttämättömänä, enimmäisaika minuutteina, ennen kuin näyttö lukkiutuu (minuuttia)  <br/> |
|Salli käyttäjille sovellusten lataaminen Microsoft Storesta  <br/> |Mukautettu URI-käytäntö  <br/> |
|Salli käyttäjien käyttää Cortanaa  <br/> |**Yleistä** \> **Cortana**-asetuksena on **Estä** Intunessa, kun asetuksena on **Pois käytöstä**Microsoft 365 Businessssa.  <br/> |
|Salli käyttäjille Windows-vihjeiden ja -mainosten vastaanottaminen Microsoftilta  <br/> |**Windows-tapahtumanäyttö**, kaikki estetään, jos tämän asetuksena on **Pois käytöstä**Microsoft 365 Businessssa.  <br/> |
|Pidä Windows 10 -laitteet ajan tasalla automaattisesti  <br/> | Tämä asetus on **Microsoft Intunen** \> **palvelu päivityksissä-Windows 10-päivitys renkaat**, valitse **Windows 10-laitteiden päivitys käytäntö**ja sitten **Ominaisuudet** \> - **Asetukset**.  <br/>  Kun Microsoft 365-liike toiminnan asetuksena on **käytössä**, kaikki seuraavat asetukset määritetään:  <br/> **Palveluhaara**-asetuksena on **CB** (CBB, kun se on poistettu käytöstä Microsoft 365 Businessssa).  <br/> **Microsoft-tuotepäivitykset**-asetuksena on **Salli**.  <br/> **Windows-ohjaimet**-asetuksena on **Salli**.  <br/> **Automaattinen päivityskäytäntö** -asetuksena on **Automaattinen asennus huoltoaikana**, jossa:  <br/> **Tuntia käynnistyksestä** -asetuksena on **klo 6.00**.  <br/> **Aktiivisten tuntien päättyminen** -asetuksena on **klo 22.00**.  <br/> **Laadun päivityksen jaksotusaika (päivää)** -asetuksena on **0**.  <br/> **Ominaisuuden päivityksen jaksotusaika (päivää)** -asetuksena on **0**.  <br/> **Toimituksen optimoinnin lataustila** -asetuksena on **HTTP yhdistetty samaan NAT-vertaisverkkoon**.  <br/> |
|||
   

