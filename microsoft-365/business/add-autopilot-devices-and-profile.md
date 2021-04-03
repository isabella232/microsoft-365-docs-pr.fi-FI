---
title: Autopilot-laitteiden ja -profiilien lisääminen vaiheittaisen ohjeen avulla
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Opi käyttämään Windows AutoPilotin avulla uusia Windows 10 -laitteita yrityksesi käyttöön, jotta ne ovat valmiina työntekijöiden käyttöön.
ms.openlocfilehash: cd8777e6ae2e395506d2bf308c99309de1e24805
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578523"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Autopilot-laitteiden ja -profiilien lisääminen vaiheittaisen ohjeen avulla

Windows AutoPilotin avulla voit määrittää yrityksesi uudet **Windows** 10 -laitteet, jotta ne ovat valmiina käytettäväksi, kun annat ne työntekijöillesi.
  
## <a name="device-requirements"></a>Laitevaatimukset

Laitteiden on täytettävä seuraavat vaatimukset:
  
- Windows 10, versio 1703 tai uudempi
    
- Uudet laitteet, jotka eivät ole käyneet läpi Windowsin käyttökokemusta
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Käytä laitteiden ja profiilien määritysopasta

[![Selite, jossa ilmoitetaan, että hallintakeskus muuttuu. Lisätietoja löytyy osoitteesta aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](/office365/admin/microsoft-365-admin-center-preview)

Jos et ole vielä luonut laiteryhmiä tai -profiileja, paras tapa aloittaa on käyttää vaiheittaista opasta. Voit myös lisätä [laitteita ja](create-and-edit-autopilot-devices.md) [määrittää profiileja](create-and-edit-autopilot-profiles.md) niihin ilman opasta. 
  
1. Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .

2. Valitse vasemmassa siirtymisruudussa  \> **Laitteet- autopilotti.**

    ![Valitse hallintakeskuksessa laitteet ja sitten AutoPilot.](../media/AutoPilot.png)
  
2. Napsauta **tai napauta AutoPilot-sivulla** **Aloitusopas.**
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Siirry **.csv-tiedoston ja** laiteluettelon lataussivulla sijaintiin, johon olet valmistautunut. CSV-tiedosto ja **sitten Avaa** \> **seuraava.** Tiedostossa on oltava kolme otsikkoa:
    
    - Sarake A: Laitteen sarjanumero
    
    - Sarake B: Windows-tuotetunnus
    
    - Sarake C: Laitteisto-hash
    
    Saat nämä tiedot laitteiston toimittajalta tai voit luoda [CSV-tiedoston Käyttämällä Get-WindowsAutoPilotInfo PowerShell-komentosarjaa.](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) 
    
    Katso lisätietoja [Laiteluettelon CSV-tiedostosta](../admin/misc/device-list.md). Voit myös ladata esimerkkitiedoston **Lataa laiteluettelon sisältävä .csv-tiedosto** -sivulta. 
    
> [!NOTE]
> Tämä komentosarja noutaa WMI:n avulla ominaisuudet, joita tarvitaan, jotta asiakas voi rekisteröidä laitteen Windows Autopilotiin. Huomaa, että on normaalia, että tuloksena syntyvä CSV-tiedosto ei kerää Windows-tuotetunnusta (PKID), koska tätä ei tarvita laitteen rekisteröimiseen, ja PKID on tyhjäarvoinen csv-tulostetiedostossa. Vain sarjanumero ja laitteiston hash täytetään.
    
4. Määritä **profiili -sivulla** voit joko valita olemassa olevan profiilin tai luoda uuden. Jos sinulla ei vielä ole sitä, sinua pyydetään luomaan sellainen. 
    
    Profiili on asetuskokoelma, jota voidaan soveltaa yksittäiseen laitteeseen tai laiteryhmään.
    
    Oletusominaisuudet ovat pakollisia, ja ne määritetään automaattisesti. Oletusominaisuudet ovat:
    
    - Ohita Cortana, OneDrive ja OEM-rekisteröinti.
    
    - Luo yrityskuvan mukainen kirjautumiskokemus.
    
    - Yhdistä laitteet Azure Active Directory -tileihin ja rekisteröi ne automaattisesti Microsoft 365 Business Premiumin hallinnoitavaksi.
    
    Lisätietoja on kohdassa Tietoja [AutoPilot-profiiliasetuksista.](autopilot-profile-settings.md) 
    
5. Toiset asetukset ovat **Ohita suojausasetukset** ja **Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi**. Nämä molemmat ovat oletusarvoisesti **Poissa käytöstä**. 
    
    Valitse **Seuraava**.
    
6. **Kun olet valmis,** luomaasi (tai valitsemaasi) profiilia käytetään luomaasi laiteryhmään lataamalla laiteluettelo. Asetukset ovat voimassa, kun laitteen käyttäjät kirjautuvat sisään seuraavan kerran. Valitse **Sulje**.
