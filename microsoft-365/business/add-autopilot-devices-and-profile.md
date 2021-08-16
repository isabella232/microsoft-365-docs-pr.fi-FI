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
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Opi käyttämään Windows AutoPilotia uusien Windows 10 yrityksesi kanssa, jotta ne ovat valmiina työntekijöiden käyttöön.
ms.openlocfilehash: b61ece9a82e12bec088be1b8e2611a13ea7f80d7669911ccaa57df72bf75ee84
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53896427"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Autopilot-laitteiden ja -profiilien lisääminen vaiheittaisen ohjeen avulla

Windows AutoPilotin avulla voit määrittää  uusia Windows 10-laitteita yrityksesi käyttöön, jotta ne ovat valmiita käytettäväksi, kun annat ne työntekijöillesi.
  
## <a name="device-requirements"></a>Laitevaatimukset

Laitteiden on täytettävä seuraavat vaatimukset:
  
- Windows 10, versio 1703 tai uudempi
    
- Uudet laitteet, joita ei ole Windows käyttökokemusta
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Käytä laitteiden ja profiilien määritysopasta

Jos et ole vielä luonut laiteryhmiä tai -profiileja, paras tapa päästä alkuun on käyttää vaiheittaista opasta. Voit myös lisätä [laitteita ja](create-and-edit-autopilot-devices.md) [määrittää profiileja](create-and-edit-autopilot-profiles.md) niihin ilman opasta. 
  
1. Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .

2. Valitse vasemmassa siirtymisruudussa **Laitteet** \> **AutoPilot**.

    ![Valitse hallintakeskuksessa laitteet ja valitse sitten AutoPilot.](../media/AutoPilot.png)
  
2. Napsauta **tai napauta AutoPilot-sivulla** **Aloitusopas**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Siirry **Upload .csv, jossa on laiteluettelo** -sivulla sijaintiin, johon olet valmistellut .CSV ja valitse **sitten** \> **Avaa seuraava.** Tiedostossa on oltava kolme otsikkoa:
    
    - Sarake A: Laitteen sarjanumero
    
    - Sarake B: Windows-tuotetunnus
    
    - Sarake C: Laitteisto-hash
    
    Saat nämä tiedot laitteiston toimittajalta tai voit luoda [CSV-tiedoston Käyttämällä PowerShell-komentosarjaa Get-WindowsAutoPilotInfo.](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) 
    
    Katso lisätietoja [Laiteluettelon CSV-tiedostosta](../admin/misc/device-list.md). Voit myös ladata esimerkkitiedoston **Lataa laiteluettelon sisältävä .csv-tiedosto** -sivulta. 
    
> [!NOTE]
> Tämä komentosarja noutaa WMI:n avulla ominaisuuksia, joita asiakas tarvitsee laitteen rekisteröimiseen Autopilotin Windows kanssa. Huomaa, että tuloksena syntyvä CSV-tiedosto ei tavallisesti kerää Windows Product ID (PKID) -arvoa, koska tätä ei tarvita laitteen rekisteröimiseen, ja PKID on tyhjäarvoinen CSV-tulostetiedostossa. Vain sarjanumero ja laitteiston hash täytetään.
    
4. Profiilin **määrittäminen -sivulla** voit joko valita olemassa olevan profiilin tai luoda uuden. Jos sinulla ei vielä ole sitä, sinua pyydetään luomaan sellainen. 
    
    Profiili on asetuskokoelma, jota voidaan soveltaa yksittäiseen laitteeseen tai laiteryhmään.
    
    Oletusominaisuudet ovat pakollisia, ja ne määritetään automaattisesti. Oletusominaisuudet ovat:
    
    - Ohita Cortana, OneDrive ja OEM-rekisteröinti.
    
    - Luo yrityskuvan mukainen kirjautumiskokemus.
    
    - Näyttöyhteys laitteet ja Azure Active Directory tilit ja rekisteröi ne automaattisesti hallinnoitavaksi Microsoft 365 Business Premium.
    
    Lisätietoja on kohdassa Tietoja [AutoPilot-profiilin asetuksista.](autopilot-profile-settings.md) 
    
5. Toiset asetukset ovat **Ohita suojausasetukset** ja **Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi**. Nämä molemmat ovat oletusarvoisesti **Poissa käytöstä**. 
    
    Valitse **Seuraava**.
    
6. **Kun olet valmis,** luomaasi (tai valitsemaasi) profiilia käytetään luomaasi laiteryhmään lataamalla laiteluettelo. Asetukset ovat voimassa, kun laitteen käyttäjät kirjautuvat seuraavan kerran. Valitse **Sulje**.

## <a name="related-content"></a>Aiheeseen liittyvä sisältö

[Tietoja AutoPilot-profiilin asetuksista](autopilot-profile-settings.md) (artikkeli)\
[Laitteiden ja sovellustietojen suojaamista koskevat vaihtoehdot](../admin/devices/choose-device-security.md) (artikkeli)
