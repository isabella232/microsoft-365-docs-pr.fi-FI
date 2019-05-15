---
title: Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa
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
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Opettele tarkistaa Microsoft 365 Business app suojausasetukset Windows 10-laitteet.
ms.openlocfilehash: 7710accf9a3cd1db788dd5215ab6d7bbb97e48a6
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074376"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Sen tarkistaminen, että käyttäjät eivät voi kopioida yritystietoja yrityksen laitteiden henkilökohtaisiin tiedostoihin

Kun olet [määrittänyt sovellusten suojauskäytännöt](protection-settings-for-windows-10-devices.md), saattaa kestää muutama tunti, ennen kuin käytäntöä sovelletaan käyttäjien laitteissa. Jos olet ottanut **käyttöön** **Estä käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin ja pakota heidät tallentamaan työtiedostot OneDrive for Businessiin** -asetuksen yrityksen omistamille laitteille, voit valita tämän käyttäjän laitteessa, kun käyttäjä on muodostanut yhteyden Azure AD:hen ja kirjautunut sisään. 
  
 **Yhteysasetusten tarkistaminen**
  
1. Kun olet kirjautunut sisään Microsoft 365 Business -tunnistetiedoilla ja muodostanut yhteyden Azure AD:hen [Windows-laitteiden määrittäminen Microsoft 365 Business -käyttäjille](set-up-windows-devices.md) -kohdassa kuvatun mukaisesti, siirry kohtaan **Windowsin asetukset** \> **Tilit** \> **Käytä työpaikan tai oppilaitoksen tiliä**. Valitse **Yhteys muodostettu \<vuokraajan nimi\> Azure AD:hen** ja valitse sitten **Tiedot**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. Voit nähdä **Hallinnoija** \<vuokraajan nimi\> -sivulla **yhteystiedot**, jotka sisältävät **hallintapalvelimen osoitteen** seuraavassa kuvassa näytetyn mukaisesti. 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Sen tarkistaminen, ettet voi liittää yritystietoja hallinnoimattomaan sovellukseen**
  
1. Avaa Outlook 2016, jonka on asentanut Microsoft 365 Business.
    
2. Avaa sähköpostiviesti ja kopioi siitä jotakin sisältöä.
    
    Avaa Muistio ja yritä sitten liittää sisältö siihen.
    
    Saat virheilmoituksen, jonka mukaan sovellus ei voi näyttää sisältöä.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Voit kuitenkin liittää saman sisällön Word 2016:een.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Sen tarkistaminen, että käyttäjät eivät voi kopioida yritystietoja henkilökohtaisten laitteiden henkilökohtaisiin tiedostoihin

 **Yhteysasetusten tarkistaminen**
  
1. Siirry henkilökohtaisessa Windows 10 -laitteessa, johon olet kirjautunut sisään paikallisena käyttäjänä, **Windowsin asetukset** -kohtaan, ja napsauta tai napauta **Tilit** \> **Käytä työpaikan tai oppilaitoksen tiliä**.
    
2. Valitse **Käytä työpaikan tai oppilaitoksen tiliä** -kohdasta **Yhdistä**.
    
3. Kirjoita Microsoft 365 Business -tunnistetietosi **Määritä työpaikan tai oppilaitoksen tili -valintaikkunaan** \> **Kirjaudu sisään**.
    
4. Valitse **Käytä työpaikan tai oppilaitoksen tiliä** -sivulla **Työpaikan tai oppilaitoksen tili** ja valitse sitten **Tiedot**.
    
    ![Click or tap Info on the Work or school account dalog.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Voit nähdä **Käytä työpaikan tai oppilaitoksen tiliä** -sivulla **yhteystiedot**, jotka sisältävät **hallintapalvelimen osoitteen** seuraavassa kuvassa näytetyn mukaisesti sekä  *wip*  - ja  *mam*  -sanat. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Sen tarkistaminen, ettet voi liittää yritystietoja hallinnoimattomaan sovellukseen**
  
1. Avaa Outlook 2016 ja lisää tarvittaessa Microsoft 365 Business -tilisi ja kirjaudu sisään Microsoft 365 Business -tunnistetiedoillasi.
    
2. Avaa sähköpostiviesti ja kopioi siitä jotakin sisältöä.
    
    Avaa Muistio ja yritä sitten liittää sisältö siihen.
    
    Saat virheilmoituksen, jonka mukaan sovellus ei voi näyttää sisältöä.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Voit kuitenkin liittää saman sisällön Word 2016:een.
    

