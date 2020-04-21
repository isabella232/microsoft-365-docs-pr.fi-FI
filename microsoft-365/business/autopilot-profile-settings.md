---
title: Tietoja Autopilot-profiilien asetuksista
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
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
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: AutoPilot-profiilien avulla voit hallita, miten Windows asennetaan käyttäjän laitteisiin. Profiilit sisältävät oletus- ja valinnaisia asetuksia, kuten Cortanan asennuksen ohituksen.
ms.openlocfilehash: 5c2ec3f4c3e0ebc4ea545d11f819c897f414ad52
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627410"
---
# <a name="about-autopilot-profile-settings"></a>Tietoja Autopilot-profiilien asetuksista

## <a name="autopilot-profile-settings"></a>Autopilot-profiilien asetukset

AutoPilot-profiilien avulla voit hallita, miten Windows on asennettu käyttäjän laitteisiin. Profiilit sisältävät seuraavat asetukset.
  
 **AutoPilot-oletusominaisuudet (pakollinen), jotka määritetään automaattisesti:**
  
|**Asetus**|**Kuvaus**|
|:-----|:-----|
|Ohita Cortanan, OneDriven ja OEM-rekisteröinnin  <br/> |Asennus ohittaa kuluttajasovellusten, kuten Cortanan ja henkilökohtaisen OneDriven, asennuksen. Laitteen käyttäjä voi asentaa ne myöhemmin, kunhan käyttäjä on laitteen paikallinen järjestelmänvalvoja. Alkuperäinen valmistajan rekisteröinti ohitetaan, koska microsoft 365 Business Premium hallitsee laitetta.  <br/> |
|Yrityskuvan mukainen kirjautumiskokemus  <br/> |Jos yritykselläsi on [Lisää yrityksen brändäys Microsoft 365 -kirjautumissivulle -sivu,](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a)laitteen käyttäjä saa tämän kokemuksen kirjautuessaan sisään.  <br/> |
|Automaattinen MDM-rekisteröinti määritetyillä AAD-tileillä  <br/> |Käyttäjätietoja hallitsee Azure Active Directory, ja käyttäjät kirjautuvat Windowsiin ja Microsoft 365:een Microsoft 365 Business Premium -tunnistetiedoillaan.  <br/> |
   
 **Valinnaiset asetukset:**
  
|**Asetus**|**Kuvaus**|
|:-----|:-----|
|Ohita tietosuoja-asetukset (oletusarvoisesti poissa käytöstä)  <br/> |Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei näe laitteen ja Windowsin käyttöoikeussopimusta kirjautuessaan ensimmäisen kerran.  <br/> |
|Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi  <br/> |Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei voi asentaa henkilökohtaisia sovelluksia, kuten Cortanaa.<br/> |
   
