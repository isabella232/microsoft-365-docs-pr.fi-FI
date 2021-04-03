---
title: Tietoja Autopilot-profiilien asetuksista
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: AutoPilot-profiilien avulla voit hallita sitä, miten Windows asennetaan käyttäjien laitteisiin. Profiilit sisältävät oletusasetuksia ja valinnaisia asetuksia, kuten ohita Cortanan asennus.
ms.openlocfilehash: 86f8718131f0a0b93e18e65e39e02e7d65aded1a
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578503"
---
# <a name="about-autopilot-profile-settings"></a>Tietoja Autopilot-profiilien asetuksista

## <a name="autopilot-profile-settings"></a>Autopilot-profiilien asetukset

AutoPilot-profiilien avulla voit hallita sitä, miten Windows asennetaan käyttäjien laitteisiin. Profiilit sisältävät seuraavat asetukset.
  
 **AutoPilot-oletusominaisuudet (pakollinen), jotka määritetään automaattisesti:**
  
|**Asetus**|**Kuvaus**|
|:-----|:-----|
|Ohita Cortana, OneDrive ja OEM-rekisteröinti  <br/> |Asennus ohittaa kuluttajasovellusten, kuten Cortanan ja henkilökohtaisen OneDriven, asennuksen. Laitteen käyttäjä voi asentaa ne myöhemmin, kunhan käyttäjä on paikallinen järjestelmänvalvoja laitteessa. Alkuperäisen valmistajan rekisteröinti ohitetaan, koska laitetta hallitaan Microsoft 365 Business Premiumilla.  <br/> |
|Yrityskuvan mukainen kirjautumiskokemus  <br/> |Jos yritykselläsi on [Lisää yrityksesi brändi Microsoft 365:n](../admin/setup/customize-sign-in-page.md)kirjautumissivulle, laitteen käyttäjä saa tämän käyttökokemuksen kirjautumisen yhteydessä.  <br/> |
|Automaattinen MDM-rekisteröinti määritetyillä AAD-tileillä  <br/> |Käyttäjätietoja hallitaan Azure Active Directoryn avulla, ja käyttäjät kirjautuvat Windowsiin ja Microsoft 365:yn Microsoft 365 Business Premium -tunnistetiedoillaan.  <br/> |
   
 **Valinnaiset asetukset:**
  
|**Asetus**|**Kuvaus**|
|:-----|:-----|
|Ohita tietosuoja-asetukset (oletusarvoisesti poissa käytöstä)  <br/> |Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei näe laitteen ja Windowsin käyttöoikeussopimusta kirjautuessaan ensimmäisen kerran.  <br/> |
|Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi  <br/> |Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei voi asentaa henkilökohtaisia sovelluksia, kuten Cortanaa.<br/> |
