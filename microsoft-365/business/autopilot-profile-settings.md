---
title: Tietoja Autopilot-profiilien asetuksista
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
description: Automaatti ohjaus profiilien avulla voit hallita sitä, miten Windows asennetaan käyttäjä laitteisiin. Profiilit sisältävät oletusarvoisia ja valinnaisia asetuksia, kuten Ohita Cortanan asennus.
ms.openlocfilehash: 912a24e3d458986a4bcf7dcf903f80211996aca2
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/14/2019
ms.locfileid: "38321781"
---
# <a name="about-autopilot-profile-settings"></a>Tietoja Autopilot-profiilien asetuksista

## <a name="autopilot-profile-settings"></a>Autopilot-profiilien asetukset

Automaatti ohjaus profiilien avulla voit määrittää, miten Windows asennetaan käyttäjä laitteisiin. Profiilit sisältävät seuraavat asetukset.
  
 **AutoPilot-oletusominaisuudet (pakollinen), jotka määritetään automaattisesti:**
  
|**Asetus**|**Kuvaus**|
|:-----|:-----|
|Ohita Cortana, OneDrive ja OEM-rekisteröinti  <br/> |Asennus ohittaa kuluttajasovellusten, kuten Cortanan ja henkilökohtaisen OneDriven, asennuksen. Laitteen käyttäjä voi asentaa nämä myöhemmin, kunhan käyttäjä on laitteen paikallinen järjestelmänvalvoja. Alkuperäisen laitevalmistajan rekisteröinti ohitetaan, koska laitteen hallinnasta vastaa Microsoft 365 Business.  <br/> |
|Yrityskuvan mukainen kirjautumiskokemus  <br/> |Jos yrityksesi on [lisännyt yrityksesi brändiä Office 365-kirjautumissivulle](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), laitteen käyttäjä saa kyseisen kokemuksen kirjautumiseen.  <br/> |
|Automaattinen MDM-rekisteröinti määritetyillä AAD-tileillä  <br/> |Azure Active Directory hallitsee käyttäjä tietoja, ja käyttäjät kirjauduttava sisään Windowsiin ja Office 365-palveluun Microsoft 365-yrityksen tunniste tiedoilla.  <br/> |
   
 **Valinnaiset asetukset:**
  
|**Asetus**|**Kuvaus**|
|:-----|:-----|
|Ohita tietosuoja-asetukset (oletusarvoisesti poissa käytöstä)  <br/> |Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei näe laitteen ja Windowsin käyttöoikeussopimusta kirjautuessaan ensimmäisen kerran.  <br/> |
|Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi  <br/> |Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei voi asentaa henkilökohtaisia sovelluksia, kuten Cortanaa.<br/> |
   
