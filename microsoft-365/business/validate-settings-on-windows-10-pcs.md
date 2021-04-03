---
title: Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Lue, miten voit varmistaa, että Microsoft 365 for Business -sovelluksen suojausasetukset tulevat voimaan käyttäjien Windows 10 -laitteissa.
ms.openlocfilehash: fcb463fd98f692f7d4802689e0c03fe4e3e648a1
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579838"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Laitteiden suojausasetusten vahvistaminen Windows 10 -tietokoneissa

## <a name="verify-that-windows-10-device-policies-are-set"></a>Windows 10:n laitekäytäntöjen määrityksen varmistaminen

Kun olet [määrittänyt laitekäytännöt](protection-settings-for-windows-10-pcs.md), saattaa kestää muutama tunti, ennen kuin käytäntöä sovelletaan käyttäjien laitteissa. Voit varmistaa, että käytännöt on otettu käyttöön, perehtymällä Windowsin asetusnäyttöihin käyttäjien laitteissa. Koska käyttäjät eivät voi muokata Windows Updaten ja Windows Defenderin virustentorjunnan asetuksia Windows 10 -laitteissaan, monet vaihtoehdot näkyvät harmaina.
  
1. Siirry Asetuksiin **Päivitä** \> **&amp; suojaus** \> **Windows Updaten** \> **uudelleenkäynnistysasetuksiin** ja varmista, että kaikki asetukset näkyvät harmaina. 
    
    ![Kaikki uudelleenkäynnistysasetukset näkyvät harmaina.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Valitse  Asetukset \> **Päivitä &amp; suojaus** \> **Windows Updaten** \> **lisäasetukset** ja varmista, että kaikki asetukset näkyvät harmaina. 
    
    ![Windowsin Lisäasetukset-asetukset näkyvät harmaina.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.
    
    Varmista, että näet punaisella viestin siitä, että organisaatiosi on piilottanut tai hallinnoi joitakin asetuksia ja että kaikki vaihtoehdot näkyvät harmaina.
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**. 
    
5. Varmista, että kaikki asetukset näkyvät harmaina. 
    
    ![Virusten ja uhkien torjunta-asetukset näkyvät harmaina.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Aiheeseen liittyvät aiheet

[Microsoft 365 for Businessin dokumentaatio ja resurssit](./index.yml)
  
[Microsoft 365 for Businessin käytön aloittaminen](microsoft-365-business-overview.md)
  
[Microsoft 365 for Businessin hallinta](manage.md)
  
[Windows 10 -tietokoneiden laitemääritysten määrittäminen](protection-settings-for-windows-10-pcs.md)
