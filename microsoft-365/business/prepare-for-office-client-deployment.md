---
title: Microsoft 365 Businessin Office-asiakkaan käyttöönottoon valmistautuminen
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Opettele asentaa 32-bittisen Office-sovellukset Windows (10) tietokonetta ja pitää ne ajan tasalla automaattisesti.
ms.openlocfilehash: 16a8230d60157f1c6731ac639d89533b05aa3afe
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982153"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Microsoft 365 Businessin Office-asiakkaan käyttöönottoon valmistautuminen

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Valmistaudu Office-sovellusten automaattiseen asentamiseen asiakastietokoneisiin.

Voit Microsoft 365 Business:n avulla asentaa 32-bittiset Office-sovellukset Windows 10 -tietokoneisiin automaattisesti ja pitää ne ajan tasalla päivityksillä.
  
Tämä toimii parhaiten, jos käyttäjän tietokoneessa on Windows 10 Business ja seuraavat ominaisuudet:
  
- Ei ole olemassa olevia Office-työpöytäsovelluksia (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ja OneDrive).
    
    tai
    
- Tietokoneeseen on asennettu Officen pika-asennusversio.
    
Voit selvittää, onko käytössäsi Officen pika-asennusversio, valitsemalla missä tahansa Office-sovelluksessa **Tiedosto** \> **Tili** (Outlookissa **Office-tili**). Jos näkyviin tulevat seuraavassa kuvassa esitetyt Office-päivitykset, asennus on tehty pika-asennuksena. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kuka hyötyy tästä ominaisuudesta**
  
Käyttäjä, jonka PC-tietokoneessa on seuraavat ominaisuudet:
  
- **Tietokoneessa on** Windows 10 Business -käyttöoikeus, aktiivinen Microsoft 365 Business-käyttöoikeus sekä Windows 10:n Creators-päivitys ja se on liitetty Azure Active Directoryyn. 
    
- **Tietokoneessa ei ole** 64-bittisiä Office-sovelluksia (esimerkki: Word, Excel, Powerpoint). Jos 64-bittiset Office-sovellukset tarvitaan, tämä toiminto ei ole sopiva, koska Microsoft 365 Business-hallintakonsolissa ei ole tukea 64-bittisen Office 2016 -pika-asennusversion käynnistämiseen. 
    
- **Tietokoneessa ei ole** mitään 2016 Windows Installer (MSI) -erillissovelluksia (esimerkiksi Visiota tai Projectia). Microsoft 365 Business päivittää Officen Office 2016 -pika-asennusversioksi, eikä se toimi Office 2016 -erillissovellusten kanssa. 
    
Seuraavassa taulukossa kerrotaan, mitä toimenpiteitä käyttäjien tai järjestelmänvalvojien on ehkä alkutilan mukaan tehtävä, jotta Officen 32-bittisen pika-asennusversion käyttöönotto Microsoft 365 Business-hallintakonsolista onnistuu.
  
|**Office-asennuksen aloittamistila**|**Toimenpiteet ennen Microsoft 365 Business:n Office-asennusta**|**Lopputila**|
|:-----|:-----|:-----|
|Ei asennettua Office-ohjelmistopakettia  <br/> |Ei mitään  <br/> |32-bittinen Office 2016 asennettu pika-asennuksena  <br/> |
|Olemassa oleva 32-bittisen Officen (2016 tai aiempi versio) pika-asennusversio, mutta ei erillissovelluksia  <br/> |Ei mitään  <br/> |Päivitetty uusimpaan 32-bittiseen Office 2016 -pika-asennusversioon tarpeen mukaisesti **\*** <br/> |
|Olemassa oleva 32-bittisen Officen pika-asennusversio ja 32- tai 64-bittisten Office-erillissovellusten (kuten Vision tai Projectin) pika-asennusversiot  <br/> |Ei mitään  <br/> |Ei vaikutusta erillissovelluksiin. Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon  <br/> |
|Olemassa oleva 32-bittisen Officen pika-asennusversio ja mitkä tahansa 32- tai 64-bittiset (paitsi 2016) Office MSI -erillissovellukset  <br/> |Ei mitään  <br/> |Ei vaikutusta erillissovelluksiin. Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon  <br/> ||||
|Mikä tahansa 64-bittisen Officen pika-asennusversio  <br/> |Poista 64-bittisten Office-sovellusten asennus, jos ne voidaan korvata 32-bittisillä Office-sovelluksilla  <br/> |Jos 64-bittiset Office-sovellukset poistetaan, 32-bittinen Office 2016 -pika-asennusversio asennetaan  <br/> |
|Olemassa oleva Office 2016:n MSI-asennus ja erillissovellukset tai ei erillissovelluksia  <br/> |Poista MSI Office 2016:n asennus.  <br/> |32-bittinen Office 2016 -pika-asennusversio on asennettu. Ei muutoksia erillissovelluksiin  <br/> |
|Olemassa oleva Office 2013:n (tai aiemman version) MSI-asennus ja/tai Office-erillissovellukset  <br/> |Ei mitään  <br/> |32-bittinen Office 2016 -pika-asennusversio ja olemassa oleva MSI Office -asennus (ja erillissovellukset) ovat rinnakkain  <br/> |
||||
   
 **(\*) Huomautus:** Ei päivitä 32-bittiseen Office 2016 -pika-asennusversioon tunnetun ohjelmavirheen takia. Korjausta valmistellaan. 
  


