---
title: Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa
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
description: Opi vahvistamaan Microsoft 365 Business-sovellusten suojaus asetukset Windows 10-laitteissa.
ms.openlocfilehash: 6573519ee2fe2d1eb82545755fa98b8c018e08ff
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594991"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Sen tarkistaminen, että käyttäjät eivät voi kopioida yritystietoja yrityksen laitteiden henkilökohtaisiin tiedostoihin

Kun olet [määrittänyt sovellusten suojauskäytännöt](protection-settings-for-windows-10-devices.md), saattaa kestää muutama tunti, ennen kuin käytäntöä sovelletaan käyttäjien laitteissa. Jos olet ottanut käyttöön **Estä käyttäjiä kopioimasta yrityksen tietoja omiin tiedostoihin ja pakota heidät tallentamaan työtiedostot** yrityksen omistamien laitteiden OneDrive for Business-asetukseen, voit tarkistaa tämän käyttäjän laitteessa sen jälkeen, kun ne ovat yhteydessä Azure adiin ja kirjaudutut **sisään** . 
  
 **Yhteysasetusten tarkistaminen**
  
1. Kun olet kirjautunut sisään Microsoft 365 Business -tunnistetiedoilla ja muodostanut yhteyden Azure AD:hen [Windows-laitteiden määrittäminen Microsoft 365 Business -käyttäjille](set-up-windows-devices.md) -kohdassa kuvatun mukaisesti, siirry kohtaan **Windowsin asetukset** \> **Tilit** \> **Käytä työpaikan tai oppilaitoksen tiliä**. Valitse **Yhteys muodostettu \<vuokraajan nimi\> Azure AD:hen** ja valitse sitten **Tiedot**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. **Hallittu** \<vuokra ajan nimi\> -sivulla voit nähdä **yhteys tiedot** , jotka sisältävät **hallinta palvelimen osoitteen** , kuten seuraavassa kuvassa näkyvä. 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Sen varmistaminen, että yritys tietoja ei voi liittää hallittuun sovellukseen**
  
1. Avaa Outlook 2016, jonka on asentanut Microsoft 365 Business.
    
2. Avaa sähköpostiviesti ja kopioi siitä jotakin sisältöä.
    
    Avaa Muistio ja yritä sitten liittää sisältö siihen.
    
    Näyttöön tulee virhe sanoma, jonka mukaan sovellus ei voi käyttää sisältöä.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Voit kuitenkin liittää saman sisällön Word 2016:een.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Sen tarkistaminen, että käyttäjät eivät voi kopioida yritystietoja henkilökohtaisten laitteiden henkilökohtaisiin tiedostoihin

 **Yhteysasetusten tarkistaminen**
  
1. Windows 10-laitteessa, jossa olet kirjautuneena paikallisena käyttäjänä, siirry **Windows-asetuksiin**ja napsauta tai napauta **tilien** \> **käyttö oikeus työtä tai**koulua.
    
2. Valitse **Käytä työpaikan tai oppilaitoksen tiliä** -kohdasta **Yhdistä**.
    
3. Kirjoita Microsoft 365 Business -tunnistetietosi **Määritä työpaikan tai oppilaitoksen tili -valintaikkunaan** \> **Kirjaudu sisään**.
    
4. Valitse **Käytä työpaikan tai oppilaitoksen tiliä** -sivulla **Työpaikan tai oppilaitoksen tili** ja valitse sitten **Tiedot**.
    
    ![Napsauta tai napauta tiedot työ-tai koulu tili-ikkunassa.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. **Accessin työ-tai koulu** sivulla näet **yhteys tiedot** , jotka sisältävät **hallinta palvelimen osoitteen** , kuten seuraavassa kuvassa näkyvä, ja sisältävät sanat *KET* ja *Mam* sisällä. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Sen varmistaminen, että yritys tietoja ei voi liittää hallittuun sovellukseen**
  
1. Avaa Outlook 2016 ja lisää tarvittaessa Microsoft 365 Business -tilisi ja kirjaudu sisään Microsoft 365 Business -tunnistetiedoillasi.
    
2. Avaa sähköpostiviesti ja kopioi siitä jotakin sisältöä.
    
    Avaa Muistio ja yritä sitten liittää sisältö siihen.
    
    Näyttöön tulee virhe sanoma siitä, että sovellus ei voi käyttää sisältöä.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Voit kuitenkin liittää saman sisällön Word 2016:een.
    

