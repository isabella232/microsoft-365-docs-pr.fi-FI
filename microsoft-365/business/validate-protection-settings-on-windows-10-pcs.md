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
description: Vahvista Microsoft 365 Business Premium -sovelluksen suojausasetukset Windows 10 -laitteissa ja varmista, että käyttäjät eivät voi kopioida yritystietoja henkilökohtaisiin tiedostoihin tai ei-hallittuihin sovelluksiin.
ms.openlocfilehash: e319ffa5149f055b5de45078facc8899acffc223
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579858"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Sen tarkistaminen, että käyttäjät eivät voi kopioida yritystietoja yrityksen laitteiden henkilökohtaisiin tiedostoihin

Kun olet [määrittänyt sovellusten suojauskäytännöt](protection-settings-for-windows-10-devices.md), saattaa kestää muutama tunti, ennen kuin käytäntöä sovelletaan käyttäjien laitteissa. Jos olet **ottanut Estä** käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin ja pakotit heidät tallentamaan työtiedostot Yrityksen omistamien laitteiden **OneDrive for Business** -asetukseen, voit tarkistaa tämän käyttäjän laitteessa, kun käyttäjä on muodostanut yhteyden Azure AD:hen ja kirjautunut sisään. 
  
 **Yhteysasetusten tarkistaminen**
  
1. Kun olet kirjautunut Sisään Microsoft 365 Business Premium -tunnistetiedoilla ja muodostanut yhteyden Azure AD:seen [artikkelissa Windows-laitteiden määrittäminen Microsoft 365 Business Premium](set-up-windows-devices.md)-käyttäjille kuvatulla tavalla, siirry **Windows-asetusten** tileihin, jotka ovat käytössä töissä \>  \> **tai oppilaitoksessa.** Valitse **Yhdistetty \<tenant name\> Azure AD:en** ja valitse **sitten Tiedot.**
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. **Hallittu-sivulla** näet hallintapalvelimen osoitteen sisältävät yhteystiedot seuraavassa kuvassa \<tenant name\>  esitetyllä tavalla.  
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Varmista, että yritystietoja ei voi liittää ei-hallittavaan sovellukseen**
  
1. Avaa Microsoft 365 Business Premiumin asentama Outlook 2016.
    
2. Avaa sähköpostiviesti ja kopioi siitä jotakin sisältöä.
    
    Avaa Muistio ja yritä sitten liittää sisältö siihen.
    
    Näyttöön tulee virheilmoitus, jossa todetaan, että sovellus ei voi käyttää sisältöä.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Voit kuitenkin liittää saman sisällön Word 2016:een.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Sen tarkistaminen, että käyttäjät eivät voi kopioida yritystietoja henkilökohtaisten laitteiden henkilökohtaisiin tiedostoihin

 **Yhteysasetusten tarkistaminen**
  
1. Siirry henkilökohtaisessa Windows 10 -laitteessasi, jossa olet kirjautunut sisään paikallisena käyttäjänä, **Windows-asetukset** ja valitse **sitten Tilien** käyttö töissä \> **tai oppilaitoksessa.**
    
2. Valitse **Käytä työpaikan tai oppilaitoksen tiliä** -kohdasta **Yhdistä**.
    
3. Anna Microsoft 365 Business Premium -tunnistetietosi Määritä työ- tai koulutili **-valintaikkunaan** \> **Kirjaudu sisään.**
    
4. Valitse **Käytä työpaikan tai oppilaitoksen tiliä** -sivulla **Työpaikan tai oppilaitoksen tili** ja valitse sitten **Tiedot**.
    
    ![Napsauta tai napauta Tiedot Työ- tai koulutili -valintaikkunassa.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Accessin **työ-** tai koulusivulla  näet yhteystiedot, jotka sisältävät **hallintapalvelimen** osoitteen, kuten seuraavassa kuvassa, ja sisältää sanat *wip* and *mam* within. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Varmista, että yritystietoja ei voi liittää ei-hallittavaan sovellukseen**
  
1. Avaa Outlook 2016, lisää Tarvittaessa Microsoft 365 Business Premium -tili ja kirjaudu sisään Microsoft 365 Business Premium -tunnistetiedoillasi.
    
2. Avaa sähköpostiviesti ja kopioi siitä jotakin sisältöä.
    
    Avaa Muistio ja yritä sitten liittää sisältö siihen.
    
    Näyttöön tulee virhesanoma, jonka mukaan Sovellus ei voi käyttää sisältöä.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Voit kuitenkin liittää saman sisällön Word 2016:een.
    

