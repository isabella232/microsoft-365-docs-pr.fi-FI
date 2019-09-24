---
title: Autopilot-laitteiden ja -profiilien lisääminen vaiheittaisen ohjeen avulla
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Opi käyttämään Windowsin automaatti ohjausta uusien Windows 10-laitteiden käyttöön yrityksellesi.
ms.openlocfilehash: ee4b4a9b06c08b8f9456822b680542665c27baf3
ms.sourcegitcommit: 7690c8bfdea6e6d245cfa7c5b09b913b092cde0a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/23/2019
ms.locfileid: "37121194"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Autopilot-laitteiden ja -profiilien lisääminen vaiheittaisen ohjeen avulla

Windowsin automaatti ohjauksen avulla voit määrittää **uusia** Windows 10-laitteita yrityksellesi, jotta ne ovat valmiita tuottavaan käyttöön heti, kun annat ne työn tekijöille.
  
## <a name="device-requirements"></a>Laitevaatimukset

Laitteiden on täytettävä nämä vaatimukset:
  
- Windows 10, versio 1703 tai uudempi.
    
- Uudet laitteet, joita ei ole määritetty Windowsin tervetuloa-ohjelmassa.
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Käytä laitteiden ja profiilien määritysopasta

[![Etiketti, jonka avulla voit tietää, että hallinta keskus on muuttumassa ja löydät lisä tietoja osoitteessa aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Jos sinulla ei ole vielä luotuna laiteryhmiä tai -profiileja, aloittaminen on helpointa vaiheittaisen oppaan avulla, mutta voit myös [lisätä laitteita](create-and-edit-autopilot-devices.md) ja [määrittää profiileja](create-and-edit-autopilot-profiles.md) käyttämättä opasta. 
  
1. Siirry hallinta keskukseen-kohtaan <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.

2. Valitse vasemmassa NAV-ohjelmassa **laitteet** \> **automaatti ohjaus**.

    ![Valitse hallinta keskuksessa laitteet ja sitten automaatti ohjaus.](media/AutoPilot.png)
  
2. Napsauta tai napauta **automaatti ohjaus** -sivulla **Aloitus opas**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Valitse **Lataa laiteluettelon sisältävä .csv-tiedosto** -sivulta sijainti, johon olet valmistellut .csv-tiedoston, ja valitse sitten **Avaa** \> **Seuraava**. Tiedostossa pitäisi olla kolme otsikkoa:
    
  - Sarake A: Laitteen sarjanumero
    
  - Sarake B: Windows-tuotetunnus
    
  - Sarake C: Laitteisto-hash
    
    Saat nämä tiedot laitevalmistajalta tai voit käyttää PowerShell-komentosarjaa [Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), joka luo CSV-tiedoston. 
    
    Katso lisätietoja [Laiteluettelon CSV-tiedostosta](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Voit myös ladata esimerkkitiedoston **Lataa laiteluettelon sisältävä .csv-tiedosto** -sivulta. 
    
4. Voit valita joko olemassa olevan profiilin **Profiilin määrittäminen** -sivulta tai luoda uuden profiilin. Jos sinulla ei ole vielä profiilia, ohjelma pyytää luomaan uuden. 
    
    Profiili on asetuskokoelma, jota voidaan soveltaa yksittäiseen laitteeseen tai laiteryhmään.
    
    Oletusominaisuudet ovat pakolliset, ja ne määritetään automaattisesti. Oletusominaisuudet ovat:
    
  - Cortana, OneDrive ja OEM-rekisteröinti ohitetaan.
    
  - Luo yrityskuvan mukainen kirjautumiskokemus.
    
  - Laitteet yhdistetään Azure Active Directory -tileihin ja rekisteröidään automaattisesti Microsoft 365 Business:n hallinnoitavaksi.
    
    Katso lisätietoja kohdasta
    
    [Tietoja AutoPilot-profiilien asetuksista](autopilot-profile-settings.md) . 
    
5. Toiset asetukset ovat **Ohita suojausasetukset** ja **Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi**. Nämä molemmat ovat oletusarvoisesti **Poissa käytöstä**. 
    
    Valitse **Seuraava**.
    
6. **Olet valmis** -sivu osoittaa, että luomaasi (tai valitsemaasi) sivua sovelletaan luomaasi laiteryhmään lataamalla laiteluettelo. Nämä asetukset ovat voimassa, kun laitteen käyttäjät kirjautuvat seuraavan kerran. Valitse **Sulje**.
    