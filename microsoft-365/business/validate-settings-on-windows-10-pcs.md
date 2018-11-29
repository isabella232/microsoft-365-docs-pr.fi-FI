---
title: Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Opettele tarkistaa Microsoft 365 Business app suojausasetukset Windows 10-laitteet.
ms.openlocfilehash: db05c86bd75cc30e22e025034a3dab478d0f5365
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982703"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Laitteiden suojausasetusten vahvistaminen Windows 10 -tietokoneissa

## <a name="verify-that-windows-10-device-policies-are-set"></a>Windows 10:n laitekäytäntöjen määrityksen varmistaminen

Kun olet [määrittänyt laitekäytännöt](protection-settings-for-windows-10-pcs.md), saattaa kestää muutama tunti, ennen kuin käytäntöä sovelletaan käyttäjien laitteissa. Voit varmistaa, että käytännöt on otettu käyttöön, perehtymällä Windowsin asetusnäyttöihin käyttäjien laitteissa. Koska käyttäjät eivät voi muokata Windows Updaten ja Windows Defenderin virustentorjunnan asetuksia Windows 10 -laitteissa, valtaosa näistä asetuksista näkyy harmaana.
  
1. **Asetukset** \> **päivitys &amp; security** \> **Windows Update** \> **asetukset uudelleen** ja vahvista, että kaikki asetukset ovat harmaana. 
    
    ![All the Restart options are greyed out.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. **Asetukset** \> **päivitys &amp; security** \> **Windows Update** \> **Lisäasetukset** ja varmista, että kaikki asetukset ovat harmaana. 
    
    ![Windows Advanced updates options are all greyed out.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. **Asetukset** \> **päivitys &amp; security** \> **Windows Update** \> **lisäasetusten** \> **Valitse kuinka päivitykset toimitetaan**.
    
    Varmista, että näet (punaisella) viestin siitä, että organisaatio on piilottanut osan asetuksista tai hallitsee niitä, ja että kaikki asetukset näkyvät harmaana.
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Avaa Windows Defender Tietoturvakeskus, siirry **asetukset** \> **päivitys &amp; security** \> **Windows Defender** \> **Avaa Windows Defender Tietoturvakeskus** napsauttamalla \> **Virus &amp; säie suojaa** \> **Virus &amp; suojausasetukset uhka**. 
    
5. Varmista, että kaikki asetukset näkyvät harmaana. 
    
    ![The Virus and threat protection settings are greyed out.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Aiheeseen liittyvät artikkelit

[Microsoft 365 Businessin ohjeet ja resurssit](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Microsoft 365 Businessin käytön aloittaminen](microsoft-365-business-overview.md)
  
[Microsoft 365 Businessin hallinta](manage.md)
  
[Windows 10 -tietokoneiden laitemääritysten määrittäminen](protection-settings-for-windows-10-pcs.md)
  

