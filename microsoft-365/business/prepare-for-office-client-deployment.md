---
title: Microsoft 365 for Businessin Office-asiakassovelluksen käyttöönottoon valmistautuminen
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
description: Opi asentamaan 32-bittiset Office-sovellukset automaattisesti Windows 10 -tietokoneisiin ja pitämään ne ajan tasalla.
ms.openlocfilehash: 868d06fadfef0f55b41131b7fdfbb368b9128405
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580050"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Microsoft 365 for Businessin Office-asiakassovelluksen käyttöönottoon valmistautuminen

Tämä artikkeli koskee Microsoft 365 Business Premiumia.

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Valmistaudu Office-sovellusten automaattiseen asentamiseen asiakastietokoneisiin.

Microsoft 365 Business Premiumin avulla voit asentaa 32-bittiset Office-sovellukset automaattisesti Windows 10 -tietokoneisiin ja pitää ne ajan tasalla päivityksistä.
  
Automaattinen asennus toimii parhaiten, jos loppukäyttäjän tietokone on Windows 10 Businessissa ja:
  
- Ei ole olemassa olevia Office-työpöytäsovelluksia (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ja OneDrive).
    
    tai
    
- Tietokoneeseen on asennettu Officen pika-asennusversio.
    
Voit selvittää, onko käytössäsi Officen pika-asennusversio, valitsemalla missä tahansa Office-sovelluksessa **Tiedosto** \> **Tili** (Outlookissa **Office-tili**). Jos näet **Office-päivitykset** seuraavassa kuvassa esitetyllä tavalla, asennus on tehty käyttämällä asennuksen aikana suoritettavaa asennusta. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kuka hyötyy tämän ominaisuuden käytöstä**
  
Käyttäjä, jonka PC-tietokoneessa on seuraavat ominaisuudet:
  
- **Sinulla**  on Windows 10 Business -käyttöoikeus, aktiivinen Microsoft 365 for Business -käyttöoikeus, Windows 10 Creators -päivitys ja se on liitetty Azure Active Directoryyn. 
    
- **Siinä ei ole** 64-bittisiä Office-sovelluksia (esimerkiksi Word, Excel, PowerPoint). Jos 64-bittiset Office-sovellukset ovat pakollisia, tämä toiminto ei sovi tähän, koska 64-bittisen 2016:n office-version käynnistäminen Microsoft 365 for Business -hallintakonsolista ei tue tätä ominaisuutta. 
    
- **Tietokoneessa ei ole** mitään 2016 Windows Installer (MSI) -erillissovelluksia (esimerkiksi Visiota tai Projectia). Microsoft 365 for Business päivittää Officen Office 2016:n office 2016:n asennusversioksi, joka ei toimi Office 2016 MSI:n erillissovellusten kanssa. 
    
Seuraavassa taulukossa on esitetty, mitä toimia loppukäyttäjien/järjestelmänvalvojien on ehkä suoritettava, alkutilasta riippuen, jotta Officen 32-bittisen click-to-run-version käyttöönotto onnistuu Microsoft 365 for Business -hallintakonsolissa.
  
|**Office-asennuksen aloittamistila**|**Toimet, jotka on otettava ennen Microsoft 365 for Business Officen asentamista**|**Lopputila**|
|:-----|:-----|:-----|
|Ei asennettua Office-ohjelmistopakettia  <br/> |Ei mitään  <br/> |Office 2016:n 32-bittinen versio asennetaan käyttäen asennuksen aikana suoritettavaa asennusta  <br/> |
|Olemassa oleva 32-bittisen Officen (2016 tai aiempi versio) pika-asennusversio, mutta ei erillissovelluksia  <br/> |Ei mitään  <br/> |Päivitetty uusimpaan 32-bittiseen Office 2016 -pika-asennusversioon tarpeen mukaisesti **\*** <br/> |
|Officen 32-bittisen 32-bittisen version ja 32-bittisen tai 64-bittisen 32-bittisen 32-bittisen office-sovelluksen (esimerkiksi Visio, Project) olemassa oleva 32-bittinen tai 64-bittinen versio  <br/> |Ei mitään  <br/> |Tämä ei vaikuta erillissovelluksiin. Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon  <br/> |
|Olemassa oleva 32-bittisen Officen pika-asennusversio ja mitkä tahansa 32- tai 64-bittiset (paitsi 2016) Office MSI -erillissovellukset  <br/> |Ei mitään  <br/> |Tämä ei vaikuta erillissovelluksiin. Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon  <br/> ||||
|Mikä tahansa 64-bittisen Officen pika-asennusversio  <br/> |Poista 64-bittiset Office-sovellukset, jos niiden korvaaminen 32-bittisllä Office-sovelluksilla on ok  <br/> |Jos 64-bittiset Office-sovellukset poistetaan, 32-bittinen Office 2016 -pika-asennusversio asennetaan  <br/> |
|Olemassa oleva Office 2016:n MSI-asennus ja erillissovellukset tai ei erillissovelluksia  <br/> |Poista MSI Office 2016:n asennus.  <br/> |32-bittinen Office 2016 -pika-asennusversio on asennettu. Ei muutoksia erillissovelluksiin  <br/> |
|Olemassa oleva Office 2013:n (tai aiemman version) MSI-asennus ja/tai Office-erillissovellukset  <br/> |Ei mitään  <br/> |32-bittinen Office 2016 -pika-asennusversio ja olemassa oleva MSI Office -asennus (ja erillissovellukset) ovat rinnakkain  <br/> |
||||
   
 **(\*) Huomautus:** Ei päivitä 32-bittiseen Office 2016 -pika-asennusversioon tunnetun ohjelmavirheen takia. Korjaus on käynnissä. 
  
