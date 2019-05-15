---
title: Tarkista suojausasetukset app Android tai iOS-laitteissa
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: 'Learn how to validate the Microsoft 365 Business app protection settings in your Android or iOS devices.  '
ms.openlocfilehash: d4ed70290b21b40ca9ecd5601954c429a27dc528
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072366"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a>Tarkista suojausasetukset app Android tai iOS-laitteissa

Tarkista suojausasetukset app Android tai iOS-laitteissa välilehdet ohjeiden mukaan.
  
## <a name="androidtab"></a>[Android](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a>Sovellusten suojausasetusten toiminnan varmistaminen käyttäjien laitteissa

Kun olet [määrittänyt Android-laitteiden sovellusasetukset](app-protection-settings-for-android-and-ios.md) sovellusten suojaamista varten, seuraavien ohjeiden avulla voit vahvistaa, että valitsemasi asetukset toimivat. 
  
Varmista ensin, että käytäntö koskee sovellusta, jossa aiot vahvistaa sen.
  
1. Siirry Microsoft 365 Businessin [hallintakeskuksessa](https://portal.office.com) kohtaan **Käytännöt** \> **Muokkaa käytäntöä**.
    
2. Valitse **Androidin sovelluskäytäntö** asennuksen aikana luomillesi asetuksille tai toinen luomasi käytäntö ja varmista, että se on käytössä esimerkiksi Outlookissa. 
    
    ![Shows all the apps for which this policy protects files.](media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a>Vahvista, että Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä

Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä** on **käytössä**.
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. Avaa Outlook käyttäjän Android-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla.
    
2. Sinua pyydetään myös antamaan PIN-koodi tai käyttämään sormenjälkeä.
    
    ![Enter a PIN on your Android device to access Office apps.](media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a>Vahvista Palauta PIN-koodi, kun on tehty tämä määrä epäonnistuneita yrityksiä

Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Palauta PIN-koodi, kun on tehty tämä määrä epäonnistuneita yrityksiä** -kohtaan on määritetty jokin luku. Oletusarvo on 5. 
  
1. Avaa Outlook käyttäjän Android-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla.
    
2. Kirjoita virheellinen PIN-koodi niin monta kertaa kuin käytäntö määrittää. Näyttöön tulee kehote, jossa ilmoitetaan **PIN-koodin syöttöyritysten rajoitus saavutettiin** ja pyydetään palauttamaan PIN-koodi. 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. Paina **Palauta PIN-koodi**. Sinua pyydetään kirjautumaan sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja määrittämään uusi PIN-koodi.
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a>Vahvista Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin

Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** on **käytössä**.
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. Avaa Outlook käyttäjän Android-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.
    
2. Avaa sähköpostiviesti, jossa on liite, ja valitse liitteen tietojen vieressä oleva alanuolikuva.
    
    ![Tap the down arrow next to an attachment to try to save it.](media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    Näytön alareunassa näkyy sanoma **Laitteeseen ei voi tallentaa**. 
    
    ![Warning text that indicates cannot save a file locally to an Android.](media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > Tallentaminen OneDrive for Businessiin ei ole käytössä Androidissa tällä hetkellä, joten näet vain, että tallentaminen paikallisesti on estetty. 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a>Vahvista Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä määritetyn ajan

Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä** -kohtaan on määritetty jokin luku. Oletusarvo on 30 minuuttia. 
  
1. Avaa Outlook käyttäjän Android-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.
    
2. Outlookin Saapuneet-kansion pitäisi nyt näkyä. Älä koske Android-laitteeseen vähintään 30 minuuttiin (tai muun käytäntöön määrittämääsi aikaa pidemmän ajan). Todennäköisesti laitteen näyttö himmenee.
    
3. Avaa Outlook uudelleen Android-laitteessa.
    
4. Sinua pyydetään antamaan PIN-koodi, ennen kuin voit käyttää Outlookia uudelleen.
    
### <a name="validate-protect-work-files-with-encryption"></a>Vahvista Suojaa työtiedostot salauksella

Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Suojaa työtiedostot salauksella** on **käytössä** ja **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** **pois käytöstä**.
  
1. Avaa Outlook käyttäjän Android-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.
    
2. Avaa sähköpostiviesti, joka sisältää muutaman kuvatiedostoliitteen.
    
3. Voit tallentaa liitteen valitsemalla sen tietojen vieressä olevan alanuolikuvakkeen.
    
    ![Tap the down arrow to save the figure file to the Android device.](media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. Näyttöön voi tulla pyyntö sallia Outlookin käyttää laitteessa olevia valokuvia, mediatiedostoja ja muita tiedostoja. Valitse **Salli**.
    
5. Valitse **Tallenna laitteeseen** näytön alareunassa ja avaa sitten **Galleria** -sovellus. 
    
6. Luettelossa pitäisi näkyä salattu valokuva (tai useita, jos tallensit useita kuvatiedostoliitteitä). Se voi näkyä Kuvat-luettelossa harmaana ruutuna, jonka keskellä on valkoisen ympyrän sisällä oleva valkoinen huutomerkki.
    
    ![An encrypted image file in the Gallery app.](media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="iostab"></a>[iOS](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a>Sovellusten suojausasetusten toiminnan varmistaminen käyttäjien laitteissa

Kun olet [määrittänyt iOS-laitteiden sovellusasetukset](app-protection-settings-for-android-and-ios.md) sovellusten suojaamista varten, seuraavien ohjeiden avulla voit vahvistaa, että valitsemasi asetukset toimivat. 
  
Varmista ensin, että käytäntö koskee sovellusta, jossa aiot vahvistaa sen.
  
1. Siirry Microsoft 365 Businessin [hallintakeskuksessa](https://portal.office.com) kohtaan **Käytännöt** \> **Muokkaa käytäntöä**.
    
2. Valitse **iOS:n sovelluskäytäntö** asennuksen aikana luomillesi asetuksille tai toinen luomasi käytäntö ja varmista, että se on käytössä esimerkiksi Outlookissa. 
    
    ![Shows all the apps for which this policy protects files.](media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a>Vahvista Office-sovellusten käyttäminen edellyttää PIN-koodia

Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä** on **käytössä**.
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. Avaa Outlook käyttäjän iOS-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla.
    
2. Sinua pyydetään myös antamaan PIN-koodi tai käyttämään sormenjälkeä.
    
    ![Enter a PIN on your IOS device to access Office apps.](media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a>Vahvista Palauta PIN-koodi, kun on tehty tämä määrä epäonnistuneita yrityksiä

Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Palauta PIN-koodi, kun on tehty tämä määrä epäonnistuneita yrityksiä** -kohtaan on määritetty jokin luku. Oletusarvo on 5. 
  
1. Avaa Outlook käyttäjän iOS-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla.
    
2. Kirjoita virheellinen PIN-koodi niin monta kertaa kuin käytäntö määrittää. Näyttöön tulee kehote, jossa ilmoitetaan **PIN-koodin syöttöyritysten rajoitus saavutettiin** ja pyydetään palauttamaan PIN-koodi. 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. Paina **OK**. Sinua pyydetään kirjautumaan sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja määrittämään uusi PIN-koodi.
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a>Vahvista Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin

Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** on **käytössä**.
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. Avaa Outlook käyttäjän iOS-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.
    
2. Avaa liitteen sisältävä sähköpostiviesti, avaa liite ja valitse **Tallenna** näytön alareunassa. 
    
    ![Tap the Save option after you open an attachment to try to save it.](media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. Näkyvissä pitäisi olla vaihtoehto vain OneDrive for Businessille. Jos näin ei ole, napauta **Lisää tili** ja valitse **OneDrive for Business** **Lisää tallennustilatili** -näytössä. Kirjaudu sisään käyttäjän Microsoft 365 Business -tiedoilla kehotettaessa. 
    
    Napauta **Tallenna** ja valitse **OneDrive for Business**.
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a>Vahvista Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä määritetyn ajan

Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä** -kohtaan on määritetty jokin luku. Oletusarvo on 30 minuuttia. 
  
1. Avaa Outlook käyttäjän iOS-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.
    
2. Outlookin Saapuneet-kansion pitäisi nyt näkyä. Älä koske iOS-laitteeseen vähintään 30 minuuttiin (tai muun käytäntöön määrittämääsi aikaa pidemmän ajan). Todennäköisesti laitteen näyttö himmenee.
    
3. Avaa Outlook uudelleen iOS-laitteessa.
    
4. Sinua pyydetään antamaan PIN-koodi, ennen kuin voit käyttää Outlookia uudelleen.
    
### <a name="validate-protect-work-files-with-encryption"></a>Vahvista Suojaa työtiedostot salauksella

Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Suojaa työtiedostot salauksella** on **käytössä** ja **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** **pois käytöstä**.
  
1. Avaa Outlook käyttäjän iOS-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.
    
2. Avaa sähköpostiviesti, joka sisältää muutaman kuvatiedostoliitteen.
    
3. Napauta liitettä ja **Tallenna**-vaihtoehtoa sen alla. 
    
4. Avaa **Valokuvat**-sovellus aloitusnäytössä. Näkyviin tulee tallennettu mutta salattu valokuva (tai useampia, jos tallensit useita kuvatiedostoliitteitä). 
    
---

