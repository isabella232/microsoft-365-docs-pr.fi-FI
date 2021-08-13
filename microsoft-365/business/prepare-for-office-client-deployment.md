---
title: Office käyttöönottoon valmistautuminen Microsoft 365 yrityskäyttöön
f1.keywords:
- CSH
ms.author: efrene
author: efrene
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Opi asentamaan 32-bittiset Office automaattisesti Windows 10 ja pitämään ne ajan tasalla.
ms.openlocfilehash: 134d5f2918e3f28c2025b282b9ae0325b64fe0474ae8123d0637bb43c4730c55
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53803552"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Office käyttöönottoon valmistautuminen Microsoft 365 yrityskäyttöön

Tämä artikkeli koskee Microsoft 365 Business Premium.

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Valmistaudu Office-sovellusten automaattiseen asentamiseen asiakastietokoneisiin.

Voit Microsoft 365 Business Premium 32-bittiset Office-sovellukset Windows 10 tietokoneisiin ja pitää ne ajan tasalla päivityksillä.
  
Automaattinen asennus toimii parhaiten, jos käyttäjän tietokone on Windows 10 Business:
  
- Ei ole olemassa olevia Office-työpöytäsovelluksia (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ja OneDrive).
    
    tai
    
- Tietokoneeseen on asennettu Officen pika-asennusversio.
    
Voit selvittää, onko käytössäsi Officen pika-asennusversio, valitsemalla missä tahansa Office-sovelluksessa **Tiedosto** \> **Tili** (Outlookissa **Office-tili**). Jos näet **Office päivitykset** seuraavassa kuvassa esitetyllä tavalla, asennus on tehty click-to-run-asennuksella. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Ken tämän ominaisuuden edut**
  
Käyttäjä, jonka PC-tietokoneessa on seuraavat ominaisuudet:
  
- **Sisältää** Windows 10 Business käyttöoikeuden, aktiivisen Microsoft 365 for Business -käyttöoikeuden Windows 10 Creators -päivitys ja se on Azure Active Directory. 
    
- **Siinä ei ole** 64-bittisiä Office sovelluksia (esimerkki: Word, Excel, PowerPoint). Jos tarvitaan 64-bittisiä Office-sovelluksia, tämä toiminto ei sovi hyvin, koska Office:n 64-bittisen 2016-Microsoft 365-version käynnistäminen Microsoft 365 for Business -hallintakonsolista ei tue. 
    
- **Tietokoneessa ei ole** mitään 2016 Windows Installer (MSI) -erillissovelluksia (esimerkiksi Visiota tai Projectia). Microsoft 365 for Business Office Office 2016:n Office MSI -erillissovellusten kanssa. 
    
Seuraavassa taulukossa on esitetty, mitä toimia loppukäyttäjien ja järjestelmänvalvojien on ehkä suoritettava, jotta Office:n 32-bittisen Office-version käyttöönotto Microsoft 365 for Business -hallintakonsolissa onnistuu.<br/>


|Office-asennuksen aloittamistila|Toimet, jotka on Microsoft 365 for Businessin Office asentamista|Lopputila|
|:-----|:-----|:-----|
|Ei asennettua Office-ohjelmistopakettia  <br/> |Ei mitään  <br/> |Office 2016:n 32-bittinen versio asennetaan office 32 -asennuksena  <br/> |
|Olemassa oleva 32-bittisen Officen (2016 tai aiempi versio) pika-asennusversio, mutta ei erillissovelluksia  <br/> |Ei mitään  <br/> |Päivitetty uusimpaan 32-bittiseen Office 2016 -pika-asennusversioon tarpeen mukaisesti **\*** <br/> |
|Olemassa oleva 32-bittisen 32-bittisen Office-ja 32-bittisen tai 64-bittisen erillisversion Office-versio (esimerkiksi Visio, Project)  <br/> |Ei mitään  <br/> |Tämä ei vaikuta erillissovelluksiin. Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon  <br/> |
|Olemassa oleva 32-bittisen Officen pika-asennusversio ja mitkä tahansa 32- tai 64-bittiset (paitsi 2016) Office MSI -erillissovellukset  <br/> |Ei mitään  <br/> |Tämä ei vaikuta erillissovelluksiin. Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon  <br/> |
|Mikä tahansa 64-bittisen Officen pika-asennusversio  <br/> |64-bittisen Office-sovellusten asennuksen poistaminen, jos niiden korvaaminen 32-bittisllä Office-sovelluksilla  <br/> |Jos 64-bittiset Office-sovellukset poistetaan, 32-bittinen Office 2016 -pika-asennusversio asennetaan  <br/> |
|Olemassa oleva Office 2016:n MSI-asennus ja erillissovellukset tai ei erillissovelluksia  <br/> |Poista MSI Office 2016:n asennus.  <br/> |32-bittinen Office 2016 -pika-asennusversio on asennettu. Ei muutoksia erillissovelluksiin  <br/> |
|Olemassa oleva Office 2013:n (tai aiemman version) MSI-asennus ja/tai Office-erillissovellukset  <br/> |Ei mitään  <br/> |32-bittinen Office 2016 -pika-asennusversio ja olemassa oleva MSI Office -asennus (ja erillissovellukset) ovat rinnakkain  <br/> |
||||
   
 **(\*) Huomautus:** Ei päivitä 32-bittiseen Office 2016 -pika-asennusversioon tunnetun ohjelmavirheen takia. Korjaus on käynnissä. 
  
