---
title: Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Opi app hallintakäytännön luominen ja suojaamaan työn tiedostoja Windows 10-laitteissa.
ms.openlocfilehash: acf19a72d994185a35b2e425f8334a73a121ee10
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982823"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a>Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille

## <a name="create-an-app-management-policy-for-windows-10"></a>Windows 10:n sovellustenhallintakäytännön luominen

Jos käyttäjillä on henkilökohtaisia Windows 10 -laitteita, joissa he tekevät työtehtäviä, voit suojata tiedot myös kyseisissä laitteissa.
  
1. Kirjaudu [Microsoft 365 Businessiin](https://portal.office.com) yleisen järjestelmänvalvojan tunnistetiedoilla. Siirry hallintakeskukseen valitsemalla **Järjestelmänvalvoja** -ruutu. 
    
2. Valitse hallintaportaalin **Laitekäytännöt**-kortissa **Lisää käytäntö**.
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle. 
    
4. Valitse **Käytännön tyyppi** -kohdassa **Windows 10:n sovellusten hallinta**.
    
5. Valitse ** laitetyyppi **, **henkilökohtaisia** tai **Yrityksen omistuksessa**.
    
6. **Salaa työtiedostot** otetaan automaattisesti käyttöön. 
    
7. Määritä **Estä käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin ja pakota heidät tallentamaan työtiedostot OneDrive for Businessiin** **käyttöön**, jos et halua käyttäjien tallentavan työtiedostoja tietokoneeseensa. 
    
8. Laajenna **hallita, miten käyttäjät voivat käyttää Office-tiedostojen, laitteiden** \> miten asetukset. **Miten käyttäjät voivat käyttää Office-laitteita mobiililaitteiden hallinta** ei **ole käytössä** oletusarvoisesti, mutta voit ottaa sen **käyttöön** ja hyväksyä oletusarvot on suositeltavaa. Lisätietoja on kohdassa [käytettävissä olevat asetukset](protection-settings-for-windows-10-devices.md#bkmk_settings) . 
    
    Voit aina palauttaa oletusasetuksen **Oletusasetusten palauttaminen** -linkin avulla. 
    
9. Laajenna **Palauta tietoja Windows-laitteissa**. On suositeltavaa ottaa se **käyttöön**.
    
    Ennen kuin voit etsiä Tietojenpalautusagentti-varmenteen, sinun on ensin luotava se. Ohjeita on artikkelissa [EFS-tiedostojärjestelmän Tietojenpalautusagentti-varmenteen luominen ja vahvistaminen](https://go.microsoft.com/fwlink/p/?linkid=853700).
    
    Työtiedostot on oletusarvoisesti salattu salaisella avaimella, joka on tallennettu laitteeseen ja liitetty käyttäjän profiiliin. Vain käyttäjä itse voi avata tiedoston ja purkaa sen salauksen. Jos laite häviää tai jos käyttäjä poistetaan, tiedosto voi jäädä salattuun tilaan. Järjestelmänvalvoja voi purkaa tiedoston salauksen Tietojenpalautusagentti-varmenteen (Data Recovery Agent, DRA) avulla.
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Laajenna **Suojaa muita verkko- ja pilvisijainteja**, jos haluat lisätä muita toimialueita tai SharePoint Online -sijainteja ja varmistaa, että kaikkien ilmoitettujen sovellusten tiedostot suojataan. Jos sinun on annettava jompaankumpaan kenttään useita kohteita, lisää kohteiden väliin puolipiste (;). 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja valitse käyttöoikeusryhmät, jotka saavat nämä asetukset \> **Valitse**.
    
12. Lopuksi tallenna käytäntö valitsemalla **Lisää** ja määritä se laitteisiin. 
    
## <a name="available-settings"></a>Käytettävissä olevat asetukset

Käyttäjien Office-työtiedostojen käyttöä voidaan hallita seuraavilla asetuksilla:
  
Katso lisätietoja artikkelista [Miten Microsoft 365 Businessin suojausominaisuudet vastaavat Intunen asetuksia](map-protection-features-to-intune-settings.md).
  
|**Asetus**|**Kuvaus**|
|:-----|:-----|
|Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä  <br/> |Jos tämä asetus on **käytössä**, käyttäjien on annettava toinen todennusmuoto käyttäjänimensä ja salasanansa lisäksi, ennen kuin he voivat käyttää Office-sovelluksia mobiililaitteillaan.  <br/> |
|Palauta PIN-koodi, jos kirjautuminen epäonnistuu näin monta kertaa  <br/> |Jos haluat estää luvatonta käyttäjä arvaamasta PIN-koodia sattumalta, PIN-koodi palautetaan määrittämäsi virheellisten syöttökertojen määrän jälkeen.  <br/> |
|Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä  <br/> |Tämä asetus määrittää, kuinka kauan käyttäjä voi olla toimimatta, ennen kuin häntä kehotetaan kirjautumaan sisään uudelleen.  <br/> |
   

