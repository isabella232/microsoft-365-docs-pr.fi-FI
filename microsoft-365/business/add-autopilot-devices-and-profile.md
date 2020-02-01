---
title: Autopilot-laitteiden ja -profiilien lisääminen vaiheittaisen ohjeen avulla
f1.keywords:
- NOCSH
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Opi käyttämään Windowsin automaatti ohjausta uusien Windows 10-laitteiden käyttöön yrityksellesi.
ms.openlocfilehash: 1fd0abb76d16b79dd11ef27b6b27a87894d89ef9
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593269"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Autopilot-laitteiden ja -profiilien lisääminen vaiheittaisen ohjeen avulla

Windowsin automaatti ohjauksen avulla voit määrittää **uusia** Windows 10-laitteita yrityksellesi, jotta ne ovat valmiita käytettäväksi, kun annat ne työn tekijöillesi.
  
## <a name="device-requirements"></a>Laitevaatimukset

Laitteiden on täytettävä nämä vaatimukset:
  
- Windows 10, versio 1703 tai uudempi
    
- Uudet laitteet, jotka eivät ole olleet Windows-käyttö kokemuksen kautta
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Käytä laitteiden ja profiilien määritysopasta

[![Selite, jossa ilmoitetaan, että hallintakeskus muuttuu. Lisätietoja löytyy osoitteesta aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Jos et ole vielä luonut laite ryhmiä tai profiileja, paras tapa aloittaa se on käyttää vaiheittaisia ohjeita. Voit myös [lisätä laitteita](create-and-edit-autopilot-devices.md) ja [määrittää niille profiileja](create-and-edit-autopilot-profiles.md) käyttämättä opasta. 
  
1. Siirry hallinta keskukseen-kohtaan <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.

2. Valitse vasemmasta siirtymis ruudusta **laitteet** \> **automaatti ohjaus**.

    ![Valitse hallinta keskuksessa laitteet ja sitten automaatti ohjaus.](media/AutoPilot.png)
  
2. Napsauta tai napauta **automaatti ohjaus** -sivulla **Aloitus opas**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Siirry **Lataa. csv-tiedostoon ja laite luettelo-** sivulle selaamalla sijaintiin, jossa olet valmis. CSV-tiedosto ja **Avaa** \> **Seuraava**. Tiedostossa on oltava kolme otsikkoa:
    
    - Sarake A: Laitteen sarjanumero
    
    - Sarake B: Windows-tuotetunnus
    
    - Sarake C: Laitteisto-hash
    
    Voit hankkia nämä tiedot laitteiston toimittajalta, tai voit luoda CSV-tiedoston [Get-WindowsAutoPilotInfo PowerShell-komento sarjan](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) avulla. 
    
    Katso lisätietoja [Laiteluettelon CSV-tiedostosta](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Voit myös ladata esimerkkitiedoston **Lataa laiteluettelon sisältävä .csv-tiedosto** -sivulta. 
    
4. **Määritä profiili** -sivulla voit joko valita aiemmin luodun profiilin tai luoda uuden. Jos sinulla ei vielä ole sellaista, sinua pyydetään luomaan sellainen. 
    
    Profiili on asetuskokoelma, jota voidaan soveltaa yksittäiseen laitteeseen tai laiteryhmään.
    
    Oletus ominaisuudet ovat pakollisia, ja ne määritetään automaattisesti. Oletusominaisuudet ovat:
    
    - Ohita Cortana, OneDrive ja OEM-rekisteröinti.
    
    - Luo yrityskuvan mukainen kirjautumiskokemus.
    
    - Yhdistä laitteesi Azure Active Directory-tileihin ja rekisteröi ne automaattisesti Microsoft 365 Businessin hallitseman.
    
    Lisä tietoja on kohdassa [tietoja automaatti ohjauksen profiili asetuksista](autopilot-profile-settings.md). 
    
5. Toiset asetukset ovat **Ohita suojausasetukset** ja **Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi**. Nämä molemmat ovat oletusarvoisesti **Poissa käytöstä**. 
    
    Valitse **Seuraava**.
    
6. **Olet valmis** ilmaisee, että luomasi profiili (tai valittu) otetaan käyttöön laite ryhmälle, jonka olet luonut lataamalla laitteiden luettelon. Asetukset ovat voimassa, kun laitteen käyttäjät kirjauduttava sisään seuraavaksi. Valitse **Sulje**.
    