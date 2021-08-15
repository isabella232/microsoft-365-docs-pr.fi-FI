---
title: Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Vahvista Microsoft 365 Business Premium suojausasetukset Windows 10 laitteissa ja varmista, että käyttäjät eivät voi kopioida yritystietoja henkilökohtaisiin tiedostoihin tai ei-hallittuihin sovelluksiin.
ms.openlocfilehash: ab084ded5ef052a7b85839f0debb96eb1bc5bdf332230293613396825c7263f0
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53861696"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Sen tarkistaminen, että käyttäjät eivät voi kopioida yritystietoja yrityksen laitteiden henkilökohtaisiin tiedostoihin

Kun olet [määrittänyt sovellusten suojauskäytännöt](protection-settings-for-windows-10-devices.md), saattaa kestää muutama tunti, ennen kuin käytäntöä sovelletaan käyttäjien laitteissa. Jos olet ottanut **käyttöön** Estä käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin ja pakota heidät tallentamaan työtiedostot **OneDrive for Business-asetukseen** yrityksen omistamissa laitteissa, voit tarkistaa tämän käyttäjän laitteessa, kun hän on muodostanut yhteyden Azure AD:hen ja kirjautunut sisään. 
  
 **Yhteysasetusten tarkistaminen**
  
1. Kun olet Microsoft 365 Business Premium tunnistetiedoilla ja muodostanut yhteyden Azure [AD:iin](set-up-windows-devices.md)artikkelissa Windows-laitteiden määrittäminen Microsoft 365 Business Premium-käyttäjille  kuvatulla tavalla, siirry \> **Windows Asetukset-tilit,** käytä Windows Asetukset tai \> **oppilaitoksessa.** Valitse **Yhdistetty \<tenant name\> Azure AD:iin** ja valitse sitten **Tiedot**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. **Hallittu-sivulla** näet yhteyden tiedot, jotka sisältävät Management Server Address -osoitteen, kuten \<tenant name\>  seuraavassa kuvassa.  
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Yritystietojen liittämisen varmistaminen ei onnistu hallitsemassa sovelluksessa**
  
1. Avaa Outlook 2016, jonka Microsoft 365 Business Premium.
    
2. Avaa sähköpostiviesti ja kopioi siitä jotakin sisältöä.
    
    Avaa Muistio ja yritä sitten liittää sisältö siihen.
    
    Näyttöön tulee virhesanoma, jossa todetaan, että sovellus ei voi käyttää sisältöä.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Voit kuitenkin liittää saman sisällön Word 2016:een.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Sen tarkistaminen, että käyttäjät eivät voi kopioida yritystietoja henkilökohtaisten laitteiden henkilökohtaisiin tiedostoihin

 **Yhteysasetusten tarkistaminen**
  
1. Siirry henkilökohtaiseen Windows 10, johon olet kirjautunut sisään paikallisena käyttäjänä, valitse Windows Asetukset **ja** valitse  sitten Tilit, jotka ovat käytössä oppilaitoksessa tai \> **oppilaitoksessa.**
    
2. Valitse **Käytä työpaikan tai oppilaitoksen tiliä** -kohdasta **Yhdistä**.
    
3. Kirjoita Microsoft 365 Business Premium tunnistetietosi Määritä **työ- tai koulutili -valintaikkunaan** \> **Kirjaudu sisään**.
    
4. Valitse **Käytä työpaikan tai oppilaitoksen tiliä** -sivulla **Työpaikan tai oppilaitoksen tili** ja valitse sitten **Tiedot**.
    
    ![Napsauta tai napauta TiedotTyö- tai koulutili-valintaikkunassa.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Näet **Käytä työtä tai koulua** -sivulla Yhteystiedot-tiedot, jotka sisältävät  **hallintapalvelimen** osoitteen seuraavassa kuvassa esitetyllä tavalla ja sisältävät *wip-* ja *mam* within -sanat. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Yritystietojen liittämisen varmistaminen ei onnistu hallitsemassa sovelluksessa**
  
1. Avaa Outlook 2016 ja lisää Microsoft 365 Business Premium-tilisi tarvittaessa ja kirjaudu sisään Microsoft 365 Business Premium tunnistetiedoilla.
    
2. Avaa sähköpostiviesti ja kopioi siitä jotakin sisältöä.
    
    Avaa Muistio ja yritä sitten liittää sisältö siihen.
    
    Saat virheilmoituksen, jonka mukaan Sovellus ei voi käyttää sisältöä.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Voit kuitenkin liittää saman sisällön Word 2016:een.
    

