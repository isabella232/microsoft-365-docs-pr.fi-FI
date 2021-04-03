---
title: Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
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
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Opi luomaan, muokkaamaan tai poistamaan sovellusten hallintakäytäntöä ja suojaamaan työtiedostoja Android- tai iOS-laitteissa.
ms.openlocfilehash: 2e157737990c7aca6e87a676e90f62f0d40ad372
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580290"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten

Tämä artikkeli koskee Microsoft 365 Business Premiumia.

## <a name="create-an-app-management-policy"></a>Sovellustenhallintakäytännön luominen

1. Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
    
2. Valitse vasemmassa siirtymispalkin kohdassa  \> **Laitekäytännöt** \> **Lisää.**
  
3. Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle. 
    
4. Valitse **Käytäntötyyppi-kohdassa** **Androidin** sovellusten hallinta tai **iOS:n** sovellusten hallinta sen mukaan, mitkä käytännöt haluat luoda. 
    
5. Laajenna **Suojaa työtiedostot, kun laitteita katoaa tai varastetaan,** ja **hallitse, miten käyttäjät voivat käyttää Office-tiedostoja mobiililaitteissa.** Määritä asetukset, miten haluat. **Hallitse sitä, miten käyttäjät** voivat  käyttää Office-tiedostoja mobiililaitteissa, on oletusarvoisesti poissa käytöstä, mutta on suositeltavaa ottaa se **käyttöön** ja hyväksyä oletusarvot. Lisätietoja on kohdassa Käytettävissä [olevat asetukset.](#available-settings) 
    
    Voit aina palauttaa oletusasetuksen **Oletusasetusten palauttaminen** -linkin avulla. 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista  Kaikki käyttäjät -käyttöoikeusryhmää, valitse Muuta **ja** valitse käyttöoikeusryhmät, jotka saavat nämä \> **asetukset. Valitse**.
    
7. Lopuksi tallenna käytäntö valitsemalla **Valmis** ja määritä se laitteisiin. 
    
## <a name="edit-an-app-management-policy"></a>Sovellustenhallintakäytännön muokkaaminen

1. Valitse **Käytännöt-kortissa** **Muokkaa käytäntöä.**
    
2. Valitse **Muokkaa käytäntöä** -ruudussa käytäntö, jota haluat muuttaa. 
    
3. Valitse **Muokkaa** jokaisen asetuksen vieressä ja muuta käytännön arvoja. Kun muutat arvoa, se tallennetaan automaattisesti käytäntöön.
    
4. Kun olet valmis, sulje Muokkaa **käytäntöä -ruutu.** 
    
## <a name="delete-an-app-management-policy"></a>Sovellustenhallintakäytännön poistaminen

1. Valitse **Käytännöt-sivulla** käytäntö ja valitse **sitten Poista.**
    
2. Valitse Poista **käytäntö -ruudussa** **Vahvista,** jos haluat poistaa valitsemasi käytännön tai käytännöt. 
    
## <a name="available-settings"></a>Käytettävissä olevat asetukset

Seuraavissa taulukoissa annetaan yksityiskohtaisia tietoja käytettävissä olevista asetuksista työtiedostojen suojaamiseksi laitteissa sekä asetuksista, jotka ohjaavat sitä, miten käyttäjät voivat käyttää Office-tiedostoja mobiililaitteilla.
  
 Lisätietoja on kohdassa Miten [Microsoft 365 Business Premiumin suojausominaisuudet liittyvät Intune-asetuksiin.](map-protection-features-to-intune-settings.md) 
  
### <a name="settings-that-protect-work-files"></a>Työtiedostojen suojaamisasetukset

Seuraavilla asetuksilla voidaan suojata työtiedostoja, jos käyttäjän laite katoaa tai varastetaan:
  
|||
|:-----|:-----|
|Asetus  <br/> |Kuvaus  <br/> |
|Poista työtiedostot passiivisesta laitteesta näin monen päivän kuluttua  <br/> |Jos laitetta ei käytetä tässä määrittämääsi päivien lukumäärään, laitteeseen tallennetut työtiedostot poistetaan automaattisesti.  <br/> |
|Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin  <br/> |Jos tämä asetus **on Käytössä,** työtiedostojen ainoa käytettävissä oleva tallennussijainti on OneDrive for Business.  <br/> |
|Salaa työtiedostot  <br/> |Pidä tämä asetus **käytössä**, jotta työtiedostot suojataan salauksella. Vaikka laite katoaa tai varastetaan, kukaan ei voi lukea yrityksesi tietoja.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Asetukset, joilla hallitaan käyttäjien Office-tiedostojen käyttöä mobiililaitteilla

Käyttäjien Office-työtiedostojen käyttöä voidaan hallita seuraavilla asetuksilla:
  
|||
|:-----|:-----|
|Asetus  <br/> |Kuvaus  <br/> |
|Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä  <br/> |Jos tämä asetus **on käytössä,** käyttäjien on annettava toinen todennusmuoto käyttäjänimen ja salasanan lisäksi, ennen kuin he voivat käyttää Office-sovelluksia mobiililaitteissaan.<br/> |
|Palauta PIN-koodi, jos kirjautuminen epäonnistuu näin monta kertaa  <br/> |Jos haluat estää luvatonta käyttäjä arvaamasta PIN-koodia sattumalta, PIN-koodi palautetaan määrittämäsi virheellisten syöttökertojen määrän jälkeen.  <br/> |
|Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä  <br/> |Tämä asetus määrittää, kuinka kauan käyttäjä voi olla käyttämättömänä, ennen kuin häntä pyydetään kirjautumaan uudelleen sisään.  <br/> |
|Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu  <br/> |Kekseliäällä käyttäjällä voi olla laite, jonka suojaus on murrettu. Tämä tarkoittaa, että käyttäjä voi muokata käyttöjärjestelmää, minkä vuoksi laite voi altistua helpommin haittaohjelmille. Tällaiset laitteet on estetty, kun tämä asetus on **käytössä**.  <br/> |
|Älä salli käyttäjien kopioida sisältöä Office-sovelluksista henkilökohtaisiin sovelluksiin  <br/> |Oletuksena tätä ei sallita, mutta jos asetus on **käytössä**, käyttäjä voi kopioida työtiedoston tietoja henkilökohtaiseen tiedostoon. Jos asetuksena on **Ei käytössä**, käyttäjä ei voi kopioida tietoja työtilistä henkilökohtaiseen sovellukseen tai henkilökohtaisen tiliin.  <br/> |
