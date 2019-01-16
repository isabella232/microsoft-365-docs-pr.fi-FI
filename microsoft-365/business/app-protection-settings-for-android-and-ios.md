---
title: Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Opi luoda, muokata, tai poistaa app hallintakäytännön ja suojaamaan työn tiedostoja Android tai iOS-laitteissa.
ms.openlocfilehash: ed03227496120369b94bf2396974eebfd7798678
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983663"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten

## <a name="create-an-app-management-policy"></a>Sovellustenhallintakäytännön luominen

1. Kirjaudu [Microsoft 365 Businessiin](https://portal.office.com) yleisen järjestelmänvalvojan tunnistetiedoilla. 
    
2. Valitse hallintakeskuksen **Laitekäytännöt**-kortissa **Lisää käytäntö**.
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle. 
    
4. Valitse **Käytännön tyyppi** -kohdassa **Androidin sovellusten hallinta** tai **iOS:n sovellusten hallinta** sen mukaan, minkä käytäntöjoukon haluat luoda. 
    
5. Laajenna **Suojaa Työtiedostojen kun laitteita katoaa tai varastetaan** ja **miten käyttäjät voivat käyttää Office-tiedostojen mobiililaitteiden hallinta** \> miten asetukset. **Miten käyttäjät voivat käyttää mobiililaitteiden Office-tiedostojen hallinta** ei **ole käytössä** oletuksena, mutta on suositeltavaa, että **sen käyttöön** ja hyväksyä oletusarvot. Lisätietoja on kohdassa [käytettävissä olevat asetukset](app-protection-settings-for-android-and-ios.md#bkmk_availablesettings) . 
    
    Voit aina palauttaa oletusasetuksen **Oletusasetusten palauttaminen** -linkin avulla. 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja valitse käyttöoikeusryhmät, jotka saavat nämä asetukset \> **Valitse**.
    
7. Lopuksi tallenna käytäntö valitsemalla **Valmis** ja määritä se laitteisiin. 
    
## <a name="edit-an-app-management-policy"></a>Sovellustenhallintakäytännön muokkaaminen

1. **Käytännöt** kortilla Valitse **Muokkaa käytäntöä**.
    
2. Valitse **Muokkaa käytäntöä** -ruudussa käytäntö, jota haluat muuttaa. 
    
3. Valitse **Muokkaa** jokaisen asetuksen vieressä ja muuta käytännön arvoja. Kun muutat arvoa, se tallennetaan automaattisesti käytäntöön. 
    
4. Kun olet valmis, sulje **Muokkaa käytäntöä** -ruutu. 
    
## <a name="delete-an-app-management-policy"></a>Sovellustenhallintakäytännön poistaminen

1. Valitse **Käytännöt**-kortissa **Poista käytäntö**.
    
2. Poista haluamasi käytännöt valitsemalla ne **Poista käytäntö** -ruudussa \> **Valitse**, sitten **Vahvista**. 
    
## <a name="available-settings"></a>Käytettävissä olevat asetukset

Seuraavissa taulukoissa on tarkkoja tietoja käytettävissä olevista asetuksista, joilla voit suojata työtiedostoja laitteissa, sekä asetuksista, joilla voit hallita käyttäjien Office-tiedostojen käyttöä mobiililaitteissa.
  
 Katso lisätietoja artikkelista [Miten Microsoft 365 Businessin suojausominaisuudet vastaavat Intunen asetuksia](map-protection-features-to-intune-settings.md). 
  
### <a name="settings-that-protect-work-files"></a>Työtiedostojen suojaamisasetukset

Seuraavilla asetuksilla voidaan suojata työtiedostoja, jos käyttäjän laite katoaa tai varastetaan:
  
|||
|:-----|:-----|
|Asetus  <br/> |Kuvaus  <br/> |
|Poista työtiedostot passiivisesta laitteesta näin monen päivän kuluttua  <br/> |Jos laitetta ei käytetä niin moneen päivään kuin tässä määrität, laitteeseen tallennetut työtiedostot poistetaan automaattisesti.  <br/> |
|Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin  <br/> |Jos tämä asetus on **käytössä**, ainoa käytettävissä oleva työtiedostojen tallennuspaikka on OneDrive for Business.  <br/> |
|Salaa työtiedostot  <br/> |Pidä tämä asetus **käytössä**, jotta työtiedostot suojataan salauksella. Vaikka laite katoaa tai varastetaan, kukaan voi lukea yritystietojasi.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Asetukset, joilla hallitaan käyttäjien Office-tiedostojen käyttöä mobiililaitteissa

Käyttäjien Office-työtiedostojen käyttöä voidaan hallita seuraavilla asetuksilla:
  
|||
|:-----|:-----|
|Asetus  <br/> |Kuvaus  <br/> |
|Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä  <br/> |Jos tämä asetus on **käytössä**, käyttäjien on annettava toinen todennusmuoto käyttäjänimensä ja salasanansa lisäksi, ennen kuin he voivat käyttää Office-sovelluksia mobiililaitteillaan.  <br/> |
|Palauta PIN-koodi, jos kirjautuminen epäonnistuu näin monta kertaa  <br/> |Jos haluat estää luvatonta käyttäjä arvaamasta PIN-koodia sattumalta, PIN-koodi palautetaan määrittämäsi virheellisten syöttökertojen määrän jälkeen.  <br/> |
|Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä  <br/> |Tämä asetus määrittää, kuinka kauan käyttäjä voi olla toimimatta, ennen kuin häntä kehotetaan kirjautumaan sisään uudelleen.  <br/> |
|Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu  <br/> |Kekseliäällä käyttäjällä voi olla laite, jonka suojaus on murrettu. Tämä tarkoittaa, että käyttäjä voi muokata käyttöjärjestelmää, minkä vuoksi laite voi altistua helpommin haittaohjelmille. Tällaiset laitteet on estetty, kun tämä asetus on **käytössä**.  <br/> |
|Salli käyttäjille sisällön kopiointi Office-sovelluksista henkilökohtaisiin sovelluksiin  <br/> |Emme Salli oletusarvoisesti, mutta jos asetus on **käytössä**, käyttäjä voi kopioida tietoja työtiedostoa henkilökohtaisen tiedoston. Jos asetus on **poistettu käytöstä**, käyttäjä voi kopioida tiedot työn tilin oman app tai henkilökohtaisen tilin.<br/> |
   

  

