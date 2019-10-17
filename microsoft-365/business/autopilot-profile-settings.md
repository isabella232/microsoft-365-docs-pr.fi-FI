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
ms.openlocfilehash: eb0d9a95c796909d024db1d061aaeace7d07ed1b
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/17/2019
ms.locfileid: "37574574"
---
# <a name="about-autopilot-profile-settings"></a>Tietoja Autopilot-profiilien asetuksista

## <a name="autopilot-profile-settings"></a>Autopilot-profiilien asetukset

Voit määrittää AutoPilot-profiilien avulla, miten Windows asennetaan käyttäjien laitteisiin. Profiilit sisältävät seuraavat asetukset.
  
 **AutoPilot-oletusominaisuudet (pakollinen), jotka määritetään automaattisesti:**
  
|**Asetus**|**Kuvaus**|
|:-----|:-----|
|Ohita Cortana, OneDrive ja OEM-rekisteröinti  <br/> |Asennus ohittaa kuluttajasovellusten, kuten Cortanan ja henkilökohtaisen OneDriven, asennuksen. Laitteen käyttäjä voi asentaa nämä myöhemmin, kunhan hänellä on paikallisen järjestelmänvalvojan oikeudet laitteeseen. Alkuperäisen laitevalmistajan rekisteröinti ohitetaan, koska laitteen hallinnasta vastaa Microsoft 365 Business.  <br/> |
|Yrityskuvan mukainen kirjautumiskokemus  <br/> |Jos yrityksesi on [lisännyt yrityksesi brändiä Office 365-kirjautumissivulle](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), laitteen käyttäjä saa kyseisen kokemuksen kirjautumiseen.  <br/> |
|Automaattinen MDM-rekisteröinti määritetyillä AAD-tileillä  <br/> |Käyttäjätietoja hallitaan Azure Active Directoryn avulla, ja käyttäjät kirjautuvat Windowsiin ja Office 365:een käyttämällä Microsoft 365 Business -tunnistetietojaan.  <br/> |
   
 **Valinnaiset asetukset:**
  
|**Asetus**|**Kuvaus**|
|:-----|:-----|
|Ohita tietosuoja-asetukset (oletusarvoisesti poissa käytöstä)  <br/> |Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei näe laitteen ja Windowsin käyttöoikeussopimusta kirjautuessaan ensimmäisen kerran.  <br/> |
|Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi  <br/> |Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei voi asentaa henkilökohtaisia sovelluksia, kuten Cortanaa.  <br/> |
   
