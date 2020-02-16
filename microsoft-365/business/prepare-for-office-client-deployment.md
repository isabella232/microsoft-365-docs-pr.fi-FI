---
title: Microsoft 365 Businessin Office-asiakkaan käyttöönottoon valmistautuminen
f1.keywords:
- CSH
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
description: Lue, miten voit asentaa 32-bittiset Office-sovellukset automaattisesti Windows 10 -tietokoneisiin ja pitää ne ajan tasalla.
ms.openlocfilehash: 0f8cd7df49ad627b190fad6737ec95a6d64d99d0
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065098"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Microsoft 365 Businessin Office-asiakkaan käyttöönottoon valmistautuminen

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Valmistaudu Office-sovellusten automaattiseen asentamiseen asiakastietokoneisiin.

Microsoft 365 Businessin avulla voit asentaa 32-bittiset Office-sovellukset automaattisesti Windows 10 -tietokoneisiin ja pitää ne ajan tasalla päivityksistä.
  
Automaattinen asennus toimii parhaiten, jos loppukäyttäjän tietokone on Windows 10 Businessissa ja:
  
- Ei ole olemassa olevia Office-työpöytäsovelluksia (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ja OneDrive).
    
    tai
    
- Tietokoneeseen on asennettu Officen pika-asennusversio.
    
Voit selvittää, onko käytössäsi Officen pika-asennusversio, valitsemalla missä tahansa Office-sovelluksessa **Tiedosto** \> **Tili** (Outlookissa **Office-tili**). Jos näet **Office-päivitykset** seuraavassa kuvassa esitetyllä tavalla, asennus tehtiin pika-asennuksen avulla. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kuka hyötyy tästä ominaisuudesta**
  
Käyttäjä, jonka PC-tietokoneessa on seuraavat ominaisuudet:
  
- **Tietokoneessa on** Windows 10 Business -käyttöoikeus, aktiivinen Microsoft 365 Business-käyttöoikeus sekä Windows 10:n Creators-päivitys ja se on liitetty Azure Active Directoryyn. 
    
- **Ei ole** 64-bittisiä Office-sovelluksia (esimerkiksi Word, Excel, PowerPoint). Jos 64-bittiset Office-sovellukset ovat pakollisia, tämä ominaisuus ei ole hyvä istuvuus, koska 64-bittisen 2016:n Pika-asennus -office-version käynnistäminen Microsoft 365 Business -hallintakonsolista ei ole tukea. 
    
- **Tietokoneessa ei ole** mitään 2016 Windows Installer (MSI) -erillissovelluksia (esimerkiksi Visiota tai Projectia). Microsoft 365 Business päivittää Officen Office 2016:n pika-käyttöversioksi, eikä se toimi Office 2016:n MSI-erillisissä sovelluksissa. 
    
Seuraavassa taulukossa on esitetty, mitä toimia loppukäyttäjät/järjestelmänvalvojat saattavat joutua tekemään alustatilastaan riippuen, jotta office-käyttöönoton 32-bittinen pika-asennusversio on onnistunut Microsoft 365 Business -hallintakonsolista.
  
|**Office-asennuksen aloittamistila**|**Toimenpiteet ennen Microsoft 365 Business:n Office-asennusta**|**Lopputila**|
|:-----|:-----|:-----|
|Ei asennettua Office-ohjelmistopakettia  <br/> |Ei mitään  <br/> |Office 2016:n 32-bittinen asennus pika-asennuksen avulla  <br/> |
|Olemassa oleva 32-bittisen Officen (2016 tai aiempi versio) pika-asennusversio, mutta ei erillissovelluksia  <br/> |Ei mitään  <br/> |Päivitetty uusimpaan 32-bittiseen Office 2016 -pika-asennusversioon tarpeen mukaisesti **\*** <br/> |
|Officen 32-bittinen pika-versio ja 32-bittinen 32-bittinen tai 64-bittinen erillinen Office-sovellus (esimerkiksi Visio, Project)  <br/> |Ei mitään  <br/> |Tämä ei vaikuta erillisiin sovelluksiin. Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon  <br/> |
|Olemassa oleva 32-bittisen Officen pika-asennusversio ja mitkä tahansa 32- tai 64-bittiset (paitsi 2016) Office MSI -erillissovellukset  <br/> |Ei mitään  <br/> |Tämä ei vaikuta erillisiin sovelluksiin. Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon  <br/> ||||
|Mikä tahansa 64-bittisen Officen pika-asennusversio  <br/> |64-bittisten Office-sovellusten asennuksen poistaminen, jos niiden korvaaminen 32-bittisillä Office-sovelluksilla on ok  <br/> |Jos 64-bittiset Office-sovellukset poistetaan, 32-bittinen Office 2016 -pika-asennusversio asennetaan  <br/> |
|Olemassa oleva Office 2016:n MSI-asennus ja erillissovellukset tai ei erillissovelluksia  <br/> |Poista MSI Office 2016:n asennus.  <br/> |32-bittinen Office 2016 -pika-asennusversio on asennettu. Ei muutoksia erillissovelluksiin  <br/> |
|Olemassa oleva Office 2013:n (tai aiemman version) MSI-asennus ja/tai Office-erillissovellukset  <br/> |Ei mitään  <br/> |32-bittinen Office 2016 -pika-asennusversio ja olemassa oleva MSI Office -asennus (ja erillissovellukset) ovat rinnakkain  <br/> |
||||
   
 **(\*) Huomautus:** Ei päivitä 32-bittiseen Office 2016 -pika-asennusversioon tunnetun ohjelmavirheen takia. Korjaus on käynnissä. 
  
