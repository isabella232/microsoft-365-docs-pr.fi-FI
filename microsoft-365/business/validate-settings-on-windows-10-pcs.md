---
title: Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Opi vahvistamaan Microsoft 365 Business-sovellusten suojaus asetukset Windows 10-laitteissa.
ms.openlocfilehash: b8793ab7f77bbc7f608f237e2455f6fd12c3bb26
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721796"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Laitteiden suojausasetusten vahvistaminen Windows 10 -tietokoneissa

## <a name="verify-that-windows-10-device-policies-are-set"></a>Windows 10:n laitekäytäntöjen määrityksen varmistaminen

Kun olet [määrittänyt laitekäytännöt](protection-settings-for-windows-10-pcs.md), saattaa kestää muutama tunti, ennen kuin käytäntöä sovelletaan käyttäjien laitteissa. Voit varmistaa, että käytännöt on otettu käyttöön, perehtymällä Windowsin asetusnäyttöihin käyttäjien laitteissa. Koska käyttäjät eivät voi muokata Windows Updaten ja Windows Defenderin virustentorjunnan asetuksia Windows 10-laitteissaan, monet asetukset näkyvät harmaina.
  
1. Siirry **Asetukset** \> ** &amp; Päivitä suojaus** \> **Windows Update** \> **uudelleenkäynnistyksen asetukset** ja vahvista, että kaikki asetukset näkyvät harmaana. 
    
    ![Kaikki uudelleenkäynnistyksen asetukset näkyvät harmaana.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Siirry **asetuksiin** \> **Päivitä &amp; suojaus** \> **Windows Updaten** \> **lisä asetukset** ja varmista, että kaikki asetukset on harmaana. 
    
    ![Windowsin lisä päivitysten asetukset ovat kaikki harmaana.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.
    
    Vahvista, että näet viestin (punaisella), että jotkin asetukset ovat piilotettuja tai hallittuja organisaatiossasi ja että kaikki vaihto ehdot näkyvät harmaana.
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**. 
    
5. Varmista, että kaikki asetukset on harmaana. 
    
    ![Virusten ja uhkien torjunta-asetukset näkyvät harmaina.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Aiheeseen liittyviä ohjeita

[Microsoft 365 Businessin ohjeet ja resurssit](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Microsoft 365 Businessin käytön aloittaminen](microsoft-365-business-overview.md)
  
[Microsoft 365 Businessin hallinta](manage.md)
  
[Windows 10 -tietokoneiden laitemääritysten määrittäminen](protection-settings-for-windows-10-pcs.md)
  

