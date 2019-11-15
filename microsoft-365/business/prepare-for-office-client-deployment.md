---
title: Microsoft 365 Businessin Office-asiakkaan käyttöönottoon valmistautuminen
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Opi asentamaan 32-bittiset Office-sovellukset automaattisesti Windows 10-tieto koneisiin ja pitämään ne ajan tasalla.
ms.openlocfilehash: 09857ddeb28e953da07979045a65f6b91925aeaf
ms.sourcegitcommit: 2c2248b03f7753d64490f2f7e56ec644a235b65a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/15/2019
ms.locfileid: "38640765"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Microsoft 365 Businessin Office-asiakkaan käyttöönottoon valmistautuminen

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Valmistaudu Office-sovellusten automaattiseen asentamiseen asiakastietokoneisiin.

Microsoft 365 Businessin avulla voit asentaa 32-bittiset Office-sovellukset automaattisesti Windows 10-tieto koneisiin ja pitää ne ajan tasalla päivitysten avulla.
  
Automaattinen asennus toimii parhaiten, jos käyttäjän tieto kone on Windows 10 Businessissa ja:
  
- Ei ole olemassa olevia Office-työpöytäsovelluksia (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ja OneDrive).
    
    tai
    
- Tietokoneeseen on asennettu Officen pika-asennusversio.
    
Voit selvittää, onko käytössäsi Officen pika-asennusversio, valitsemalla missä tahansa Office-sovelluksessa **Tiedosto** \> **Tili** (Outlookissa **Office-tili**). Jos näet **Office-päivitykset** seuraavassa kuvassa esitetyllä tavalla, asennus tehtiin käyttämällä click-to-Run-kohdetta. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kuka hyötyy tämän ominaisuuden**
  
Käyttäjä, jonka PC-tietokoneessa on seuraavat ominaisuudet:
  
- **Tietokoneessa on** Windows 10 Business -käyttöoikeus, aktiivinen Microsoft 365 Business-käyttöoikeus sekä Windows 10:n Creators-päivitys ja se on liitetty Azure Active Directoryyn. 
    
- **Ei ole** 64-bittisiä Office-sovelluksia (esimerkki: Word, Excel, PowerPoint). Jos 64-bittisiä Office-sovelluksia tarvitaan, tämä ominaisuus ei ole hyvä istuvuus, koska ei ole tukea 64-bittisen 2016-version käynnistämisestä Office-versiosta Microsoft 365 Business admin Consolesta. 
    
- **Tietokoneessa ei ole** mitään 2016 Windows Installer (MSI) -erillissovelluksia (esimerkiksi Visiota tai Projectia). Microsoft 365 Business päivittää Office-version Office 2016-versioon ja se ei toimi Office 2016 MSI-sovellusten kanssa. 
    
Seuraavassa taulukossa on esitetty, mitä toimia loppu käyttäjien tai järjestelmänvalvojien on ehkä tehtävä alku tilan mukaan, jotta Office-käyttöönoton onnistunut 32-bittinen versio voidaan suorittaa Microsoft 365 Business admin Consolesta.
  
|**Office-asennuksen aloittamistila**|**Toimenpiteet ennen Microsoft 365 Business:n Office-asennusta**|**Lopputila**|
|:-----|:-----|:-----|
|Ei asennettua Office-ohjelmistopakettia  <br/> |Ei mitään  <br/> |Office 2016 32-bit asennetaan käyttämällä click-to-Run-  <br/> |
|Olemassa oleva 32-bittisen Officen (2016 tai aiempi versio) pika-asennusversio, mutta ei erillissovelluksia  <br/> |Ei mitään  <br/> |Päivitetty uusimpaan 32-bittiseen Office 2016 -pika-asennusversioon tarpeen mukaisesti **\*** <br/> |
|Officen aiemmin luotu 32-bittinen versio ja napsautus suoritettavaksi 32-bittinen tai 64-bittinen itsenäinen Office-sovellus (esimerkiksi Visio, projekti)  <br/> |Ei mitään  <br/> |Erilliset sovellukset eivät muutu. Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon  <br/> |
|Olemassa oleva 32-bittisen Officen pika-asennusversio ja mitkä tahansa 32- tai 64-bittiset (paitsi 2016) Office MSI -erillissovellukset  <br/> |Ei mitään  <br/> |Erilliset sovellukset eivät muutu. Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon  <br/> ||||
|Mikä tahansa 64-bittisen Officen pika-asennusversio  <br/> |Poista 64-bittisten Office-sovellusten asennus, jos ne on OK korvata 32-bittisellä Office-sovelluksilla  <br/> |Jos 64-bittiset Office-sovellukset poistetaan, 32-bittinen Office 2016 -pika-asennusversio asennetaan  <br/> |
|Olemassa oleva Office 2016:n MSI-asennus ja erillissovellukset tai ei erillissovelluksia  <br/> |Poista MSI Office 2016:n asennus.  <br/> |32-bittinen Office 2016 -pika-asennusversio on asennettu. Ei muutoksia erillissovelluksiin  <br/> |
|Olemassa oleva Office 2013:n (tai aiemman version) MSI-asennus ja/tai Office-erillissovellukset  <br/> |Ei mitään  <br/> |32-bittinen Office 2016 -pika-asennusversio ja olemassa oleva MSI Office -asennus (ja erillissovellukset) ovat rinnakkain  <br/> |
||||
   
 **(\*) Huomautus:** Ei päivitä 32-bittiseen Office 2016 -pika-asennusversioon tunnetun ohjelmavirheen takia. Korjaus on käynnissä. 
  