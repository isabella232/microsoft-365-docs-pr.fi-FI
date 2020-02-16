---
title: Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Lue, miten voit luoda, muokata tai poistaa sovelluksen hallintakäytännön ja suojata työtiedostoja Android- tai iOS-laitteissa.
ms.openlocfilehash: f4366230805c50fe82183431e3bd2bdfa9fddd68
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2020
ms.locfileid: "42068639"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten

![Banner, joka https://aka.ms/aboutM365previewosoittaa .](../media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a>Sovellustenhallintakäytännön luominen

1. Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. 
    
2. Valitse vasemmasta siirtymisruudusta \> **Laitekäytännöt** \> **Lisää**. ****
  
3. Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle. 
    
4. Valitse **Käytäntötyyppi -kohdassa** **Sovellusten hallinta Androidille** tai Sovellusten hallinta **iOS:lle**sen mukaan, mitkä käytännöt haluat luoda. 
    
5. Laajenna **Suojaa työtiedostot, kun laitteita katoaa tai varastetaan,** ja **Hallitse, miten käyttäjät käyttävät Office-tiedostoja mobiililaitteissa**. Määritä asetukset niin kuin haluat. **Hallitse, miten käyttäjät käyttävät Office-tiedostoja mobiililaitteissa** on oletusarvoisesti **poissa käytöstä,** mutta suosittelemme, että otat sen **käyttöön** ja hyväksyt oletusarvot. Lisätietoja on kohdassa [Käytettävissä olevat asetukset](#available-settings). 
    
    Voit aina palauttaa oletusasetuksen **Oletusasetusten palauttaminen** -linkin avulla. 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää Kaikki **käyttäjät** -oletussuojausryhmää, valitse **Muuta**, valitse \> suojausryhmät, jotka saavat nämä asetukset **Valitse**.
    
7. Lopuksi tallenna käytäntö valitsemalla **Valmis** ja määritä se laitteisiin. 
    
## <a name="edit-an-app-management-policy"></a>Sovellustenhallintakäytännön muokkaaminen

1. Valitse **Käytännöt-kortissa** **Muokkaa käytäntöä**.
    
2. Valitse **Muokkaa käytäntöä** -ruudussa käytäntö, jota haluat muuttaa. 
    
3. Valitse **Muokkaa** jokaisen asetuksen vieressä ja muuta käytännön arvoja. Kun muutat arvoa, se tallennetaan automaattisesti käytäntöön.
    
4. Kun olet valmis, sulje **Muokkaa käytäntöä -ruutu.** 
    
## <a name="delete-an-app-management-policy"></a>Sovellustenhallintakäytännön poistaminen

1. Valitse **Käytännöt-sivulla** käytäntö ja valitse sitten **Poista**.
    
2. Poista **valitsemasi** käytäntö tai käytännöt valitsemalla Poista käytäntö -ruudussa **Vahvista.** 
    
## <a name="available-settings"></a>Käytettävissä olevat asetukset

Seuraavissa taulukoissa on yksityiskohtaisia tietoja laitteiden työtiedostojen suojaamiseen käytettävissä olevista asetuksista ja asetuksista, jotka määrittävät, miten käyttäjät käyttävät Office-tiedostoja mobiililaitteistaan.
  
 Katso lisätietoja artikkelista [Miten Microsoft 365 Businessin suojausominaisuudet vastaavat Intunen asetuksia](map-protection-features-to-intune-settings.md). 
  
### <a name="settings-that-protect-work-files"></a>Työtiedostojen suojaamisasetukset

Seuraavilla asetuksilla voidaan suojata työtiedostoja, jos käyttäjän laite katoaa tai varastetaan:
  
|||
|:-----|:-----|
|Asetus  <br/> |Kuvaus  <br/> |
|Poista työtiedostot passiivisesta laitteesta näin monen päivän kuluttua  <br/> |Jos laitetta ei käytetä tässä määritettyjen päivien lukumäärään, laitteeseen tallennetut työtiedostot poistetaan automaattisesti.  <br/> |
|Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin  <br/> |Jos tämä asetus on **Käytössä**, työtiedostojen ainoa käytettävissä oleva tallennussijainti on OneDrive for Business.  <br/> |
|Salaa työtiedostot  <br/> |Pidä tämä asetus **käytössä**, jotta työtiedostot suojataan salauksella. Vaikka laite katoaa tai varastettaisiin, kukaan ei voi lukea yrityksen tietoja.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Asetukset, joilla hallitaan käyttäjien Office-tiedostojen käyttöä mobiililaitteilla

Käyttäjien Office-työtiedostojen käyttöä voidaan hallita seuraavilla asetuksilla:
  
|||
|:-----|:-----|
|Asetus  <br/> |Kuvaus  <br/> |
|Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä  <br/> |Jos tämä asetus on **Käytössä,** käyttäjien on tarjottava toinen todennusmuoto käyttäjänimen ja salasanan lisäksi, ennen kuin he voivat käyttää Office-sovelluksia mobiililaitteissaan.<br/> |
|Palauta PIN-koodi, jos kirjautuminen epäonnistuu näin monta kertaa  <br/> |Jos haluat estää luvatonta käyttäjä arvaamasta PIN-koodia sattumalta, PIN-koodi palautetaan määrittämäsi virheellisten syöttökertojen määrän jälkeen.  <br/> |
|Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä  <br/> |Tämä asetus määrittää, kuinka kauan käyttäjä voi olla käyttämättömänä, ennen kuin häntä kehotetaan kirjautumaan uudelleen sisään.  <br/> |
|Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu  <br/> |Kekseliäällä käyttäjällä voi olla laite, jonka suojaus on murrettu. Tämä tarkoittaa, että käyttäjä voi muokata käyttöjärjestelmää, minkä vuoksi laite voi altistua helpommin haittaohjelmille. Tällaiset laitteet on estetty, kun tämä asetus on **käytössä**.  <br/> |
|Salli käyttäjille sisällön kopiointi Office-sovelluksista henkilökohtaisiin sovelluksiin  <br/> |Oletuksena tätä ei sallita, mutta jos asetus on **käytössä**, käyttäjä voi kopioida työtiedoston tietoja henkilökohtaiseen tiedostoon. Jos asetuksena on **Ei käytössä**, käyttäjä ei voi kopioida tietoja työtilistä henkilökohtaiseen sovellukseen tai henkilökohtaisen tiliin.  <br/> |
