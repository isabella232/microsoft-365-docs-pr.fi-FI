---
title: Laitteen tilat
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Lisätietoja eri laitetiloista on Microsoft 365 for Businessin Järjestelmänvalvoja-aloitussivun Laitetoiminnot-luettelossa.
ms.openlocfilehash: 1a66e76dd3a74428923292427b01551db2449e48
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627242"
---
# <a name="device-states"></a><span data-ttu-id="21b1b-103">Laitteen tilat</span><span class="sxs-lookup"><span data-stu-id="21b1b-103">Device states</span></span>

<span data-ttu-id="21b1b-104">**Laitetoiminnot**-luettelon (hallintakeskuksen aloitussivu \> **Laitetoiminnot**) laitteilla voi olla seuraavat tilat.</span><span class="sxs-lookup"><span data-stu-id="21b1b-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="21b1b-106">**Tila**</span><span class="sxs-lookup"><span data-stu-id="21b1b-106">**Status**</span></span>|<span data-ttu-id="21b1b-107">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="21b1b-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="21b1b-108">Intunen hallitsema</span><span class="sxs-lookup"><span data-stu-id="21b1b-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="21b1b-109">Microsoft 365 Business Premiumin hallinnoima.</span><span class="sxs-lookup"><span data-stu-id="21b1b-109">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="21b1b-110">Käytöstä poistaminen odottaa</span><span class="sxs-lookup"><span data-stu-id="21b1b-110">Retire pending</span></span>  <br/> |<span data-ttu-id="21b1b-111">Microsoft 365 Business Premium valmistautuu poistamaan yrityksen tiedot laitteesta.</span><span class="sxs-lookup"><span data-stu-id="21b1b-111">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="21b1b-112">Käytöstä poistaminen on käynnissä</span><span class="sxs-lookup"><span data-stu-id="21b1b-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="21b1b-113">Microsoft 365 Business Premium poistaa parhaillaan yrityksen tietoja laitteesta.</span><span class="sxs-lookup"><span data-stu-id="21b1b-113">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="21b1b-114">Käytöstä poistaminen epäonnistui</span><span class="sxs-lookup"><span data-stu-id="21b1b-114">Retire failed</span></span>  <br/> | <span data-ttu-id="21b1b-115">Yritystietojen poisto epäonnistui.</span><span class="sxs-lookup"><span data-stu-id="21b1b-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="21b1b-116">Eläkkeelle peruutettu</span><span class="sxs-lookup"><span data-stu-id="21b1b-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="21b1b-117">Eläkkeelle siirtyminen peruutettiin.</span><span class="sxs-lookup"><span data-stu-id="21b1b-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="21b1b-118">Tyhjennys odottaa</span><span class="sxs-lookup"><span data-stu-id="21b1b-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="21b1b-119">Tehdasasetusten palauttamista odotetaan.</span><span class="sxs-lookup"><span data-stu-id="21b1b-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="21b1b-120">Tyhjennys käynnissä</span><span class="sxs-lookup"><span data-stu-id="21b1b-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="21b1b-121">Tehdasasetusten palautus on määritetty.</span><span class="sxs-lookup"><span data-stu-id="21b1b-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="21b1b-122">Tyhjennys epäonnistui</span><span class="sxs-lookup"><span data-stu-id="21b1b-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="21b1b-123">Tehdasasetusten palautusta ei voitu tehdä.</span><span class="sxs-lookup"><span data-stu-id="21b1b-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="21b1b-124">Pyyhitään peruutettu</span><span class="sxs-lookup"><span data-stu-id="21b1b-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="21b1b-125">Tehdaspyyhintä peruttiin.</span><span class="sxs-lookup"><span data-stu-id="21b1b-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="21b1b-126">Viallinen</span><span class="sxs-lookup"><span data-stu-id="21b1b-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="21b1b-127">Toiminto odottaa (tai on käynnissä), mutta laite ei ole kirjautunut sisään yli 30 päivään.</span><span class="sxs-lookup"><span data-stu-id="21b1b-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="21b1b-128">Poisto odottaa</span><span class="sxs-lookup"><span data-stu-id="21b1b-128">Delete pending</span></span>  <br/> |<span data-ttu-id="21b1b-129">Poistotoimintoa odotetaan.</span><span class="sxs-lookup"><span data-stu-id="21b1b-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="21b1b-130">Tunnistettu</span><span class="sxs-lookup"><span data-stu-id="21b1b-130">Discovered</span></span>  <br/> |<span data-ttu-id="21b1b-131">Microsoft 365 Business Premium on havainnut laitteen.</span><span class="sxs-lookup"><span data-stu-id="21b1b-131">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
