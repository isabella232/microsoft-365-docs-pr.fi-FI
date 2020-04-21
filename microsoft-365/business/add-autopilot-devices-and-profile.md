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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Lue, miten voit käyttää Windowsin automaattista ohjausta uusien Windows 10 -laitteiden määrittämiseen yrityksellesi, jotta ne ovat valmiita työntekijöiden käyttöön.
ms.openlocfilehash: 98a2bfc721ce86c81ebd89e8f41603e619b31546
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627490"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Autopilot-laitteiden ja -profiilien lisääminen vaiheittaisen ohjeen avulla

Windowsin automaattiohjauksen avulla voit määrittää **uusia** Windows 10 -laitteita yrityksellesi, jotta ne ovat käyttövalmiita, kun annat ne työntekijöillesi.
  
## <a name="device-requirements"></a>Laitevaatimukset

Laitteiden on täytettävä seuraavat vaatimukset:
  
- Windows 10, versio 1703 tai uudempi
    
- Uudet laitteet, joita ei ole käyty Windowsin käyttökokemuksen kautta
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Käytä laitteiden ja profiilien määritysopasta

[![Selite, jossa ilmoitetaan, että hallintakeskus muuttuu. Lisätietoja löytyy osoitteesta aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Jos et ole vielä luonut laiteryhmiä tai profiileja, paras tapa aloittaa on käyttää vaiheittaista opasta. Voit myös [lisätä laitteita](create-and-edit-autopilot-devices.md) ja määrittää niihin [profiileja](create-and-edit-autopilot-profiles.md) käyttämättä opasta. 
  
1. Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.

2. Valitse vasemmasta siirtymisruudusta **Laitteet** \> **AutoPilot**.

    ![Valitse hallintakeskuksessa laitteet ja sitten AutoPilot.](../media/AutoPilot.png)
  
2. Napsauta tai napauta **Automaattiohjaus-sivulla** **Aloitusopas**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Siirry **Lataa .csv-tiedosto, jossa on laiteluettelo -sivulla** sijaintiin, jossa olet valmistellut . CSV-tiedosto ja **avaa** \> **seuraava**. Tiedostossa on oltava kolme otsikkoa:
    
    - Sarake A: Laitteen sarjanumero
    
    - Sarake B: Windows-tuotetunnus
    
    - Sarake C: Laitteisto-hash
    
    Saat nämä tiedot laitteistotoimittajaltasi tai voit luoda [CSV-tiedoston Get-WindowsAutoPilotInfo PowerShell -komentosarjan](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) avulla. 
    
    Katso lisätietoja [Laiteluettelon CSV-tiedostosta](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Voit myös ladata esimerkkitiedoston **Lataa laiteluettelon sisältävä .csv-tiedosto** -sivulta. 
    
4. Määritä **profiili -sivulla** voit joko valita aiemmin luodun profiilin tai luoda uuden profiilin. Jos sinulla ei vielä ole sellaista, sinua pyydetään luomaan sellainen. 
    
    Profiili on asetuskokoelma, jota voidaan soveltaa yksittäiseen laitteeseen tai laiteryhmään.
    
    Oletusominaisuudet ovat pakollisia, ja ne määritetään automaattisesti. Oletusominaisuudet ovat:
    
    - Ohita Cortanan, OneDriven ja OEM-rekisteröinnin ohitus.
    
    - Luo yrityskuvan mukainen kirjautumiskokemus.
    
    - Yhdistä laitteesi Azure Active Directory -tileihin ja rekisteröi ne automaattisesti Microsoft 365 Business Premiumin hallinnoimiksi.
    
    Lisätietoja on kohdassa [Tietoja automaattiohjauksen profiiliasetuksista](autopilot-profile-settings.md). 
    
5. Toiset asetukset ovat **Ohita suojausasetukset** ja **Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi**. Nämä molemmat ovat oletusarvoisesti **Poissa käytöstä**. 
    
    Valitse **Seuraava**.
    
6. **Olet valmis** ilmaisee, että luomasi (tai valitsemasi) profiili otetaan käyttöön luomassasi laiteryhmässä lataamalla laiteluettelo. Asetukset ovat voimassa, kun laitteen käyttäjät kirjautuvat sisään seuraavaksi. Valitse **Sulje**.
    
