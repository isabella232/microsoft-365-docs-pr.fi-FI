---
title: Tietoja Autopilot-profiilien asetuksista
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Automaattiohjauksen profiilien avulla voit määrittää, miten Windowsin saa asentaa käyttäjän laitteisiin. Profiilit sisältävät oletusarvon ja valinnaisia asetuksia, kuten Cortana asennus ohittaa.
ms.openlocfilehash: d43a15e5f3dc83596b5c23dd0ceb416b24810298
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32276937"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="e9000-104">Tietoja Autopilot-profiilien asetuksista</span><span class="sxs-lookup"><span data-stu-id="e9000-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="e9000-105">Autopilot-profiilien asetukset</span><span class="sxs-lookup"><span data-stu-id="e9000-105">AutoPilot profile settings</span></span>

<span data-ttu-id="e9000-p102">Voit määrittää AutoPilot-profiilien avulla, miten Windows asennetaan käyttäjien laitteisiin. Profiilit sisältävät seuraavat asetukset.</span><span class="sxs-lookup"><span data-stu-id="e9000-p102">You can control how Windows gets installed on user devices by using the AutoPilot profiles. The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="e9000-108">**AutoPilot-oletusominaisuudet (pakollinen), jotka määritetään automaattisesti:**</span><span class="sxs-lookup"><span data-stu-id="e9000-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="e9000-109">**Asetus**</span><span class="sxs-lookup"><span data-stu-id="e9000-109">**Setting**</span></span>|<span data-ttu-id="e9000-110">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="e9000-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e9000-111">Ohita Cortana, OneDrive ja OEM-rekisteröinti</span><span class="sxs-lookup"><span data-stu-id="e9000-111">Skip Cortana, OneDrive and OEM registration</span></span>  <br/> |<span data-ttu-id="e9000-p103">Asennus ohittaa kuluttajasovellusten, kuten Cortanan ja henkilökohtaisen OneDriven, asennuksen. Laitteen käyttäjä voi asentaa nämä myöhemmin, kunhan hänellä on paikallisen järjestelmänvalvojan oikeudet laitteeseen. Alkuperäisen laitevalmistajan rekisteröinti ohitetaan, koska laitteen hallinnasta vastaa Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="e9000-p103">Skips the installation of consumer apps like Cortana and personal OneDrive. The device user can install these later as long as he or she is a local admin on the device. The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="e9000-115">Yrityskuvan mukainen kirjautumiskokemus</span><span class="sxs-lookup"><span data-stu-id="e9000-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="e9000-116">Jos yritykselläsi on [Lisää yrityksesi #microsoft Office 365: n sisään](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), laitteen käyttäjä saa kyseisen kokemuksen kirjautuessasi sisään.</span><span class="sxs-lookup"><span data-stu-id="e9000-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="e9000-117">Automaattinen MDM-rekisteröinti määritetyillä AAD-tileillä</span><span class="sxs-lookup"><span data-stu-id="e9000-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="e9000-118">Käyttäjätietoja hallitaan Azure Active Directoryn avulla, ja käyttäjät kirjautuvat Windowsiin ja Office 365:een käyttämällä Microsoft 365 Business -tunnistetietojaan.</span><span class="sxs-lookup"><span data-stu-id="e9000-118">The user identity will be managed by Azure Active directory, and the users will sign into Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="e9000-119">**Valinnaiset asetukset:**</span><span class="sxs-lookup"><span data-stu-id="e9000-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="e9000-120">**Asetus**</span><span class="sxs-lookup"><span data-stu-id="e9000-120">**Setting**</span></span>|<span data-ttu-id="e9000-121">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="e9000-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e9000-122">Ohita tietosuoja-asetukset (oletusarvoisesti poissa käytöstä)</span><span class="sxs-lookup"><span data-stu-id="e9000-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="e9000-123">Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei näe laitteen ja Windowsin käyttöoikeussopimusta kirjautuessaan ensimmäisen kerran.</span><span class="sxs-lookup"><span data-stu-id="e9000-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="e9000-124">Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi</span><span class="sxs-lookup"><span data-stu-id="e9000-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="e9000-125">Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei voi asentaa henkilökohtaisia sovelluksia, kuten Cortanaa.</span><span class="sxs-lookup"><span data-stu-id="e9000-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span>  <br/> |
   
