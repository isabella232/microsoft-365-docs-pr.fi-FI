---
title: Laitteen tilat
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Lue lisä tietoja Microsoft 365 Businessin laite osavaltioista.
ms.openlocfilehash: b55e6a5d538ec28d195225e93797cea27afd2e8b
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320204"
---
# <a name="device-states"></a><span data-ttu-id="27e20-103">Laitteen tilat</span><span class="sxs-lookup"><span data-stu-id="27e20-103">Device states</span></span>

<span data-ttu-id="27e20-104">**Laitetoiminnot**-luettelon (hallintakeskuksen aloitussivu \> **Laitetoiminnot**) laitteilla voi olla seuraavat tilat.</span><span class="sxs-lookup"><span data-stu-id="27e20-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="27e20-106">**Tila**</span><span class="sxs-lookup"><span data-stu-id="27e20-106">**Status**</span></span>|<span data-ttu-id="27e20-107">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="27e20-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="27e20-108">Intunen hallitsema</span><span class="sxs-lookup"><span data-stu-id="27e20-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="27e20-109">Microsoft 365 Businessn hallitsema</span><span class="sxs-lookup"><span data-stu-id="27e20-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="27e20-110">Käytöstä poistaminen odottaa</span><span class="sxs-lookup"><span data-stu-id="27e20-110">Retire pending</span></span>  <br/> |<span data-ttu-id="27e20-111">Microsoft 365 Business on valmiina poistamaan yritystiedot laitteesta.</span><span class="sxs-lookup"><span data-stu-id="27e20-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="27e20-112">Käytöstä poistaminen on käynnissä</span><span class="sxs-lookup"><span data-stu-id="27e20-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="27e20-113">Microsoft 365 Business poistaa parhaillaan yritystietoja laitteesta.</span><span class="sxs-lookup"><span data-stu-id="27e20-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="27e20-114">Käytöstä poistaminen epäonnistui</span><span class="sxs-lookup"><span data-stu-id="27e20-114">Retire failed</span></span>  <br/> | <span data-ttu-id="27e20-115">Yritystietojen poisto epäonnistui.</span><span class="sxs-lookup"><span data-stu-id="27e20-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="27e20-116">Keskeytä peruutettu</span><span class="sxs-lookup"><span data-stu-id="27e20-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="27e20-117">Keskeytä-toiminto peruutettiin.</span><span class="sxs-lookup"><span data-stu-id="27e20-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="27e20-118">Tyhjennys odottaa</span><span class="sxs-lookup"><span data-stu-id="27e20-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="27e20-119">Tehdasasetusten palauttamista odotetaan.</span><span class="sxs-lookup"><span data-stu-id="27e20-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="27e20-120">Tyhjennys käynnissä</span><span class="sxs-lookup"><span data-stu-id="27e20-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="27e20-121">Tehdasasetusten palautus on määritetty.</span><span class="sxs-lookup"><span data-stu-id="27e20-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="27e20-122">Tyhjennys epäonnistui</span><span class="sxs-lookup"><span data-stu-id="27e20-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="27e20-123">Tehdas asetusten palauttamista ei voitu tehdä.</span><span class="sxs-lookup"><span data-stu-id="27e20-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="27e20-124">Pyyhi peruutettu</span><span class="sxs-lookup"><span data-stu-id="27e20-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="27e20-125">Tehdas pyyhkiä peruutettiin.</span><span class="sxs-lookup"><span data-stu-id="27e20-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="27e20-126">Viallinen</span><span class="sxs-lookup"><span data-stu-id="27e20-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="27e20-127">Toiminto on vireillä (tai käynnissä), mutta laitetta ei ole kuitattu sisään 30 + päivän ajan.</span><span class="sxs-lookup"><span data-stu-id="27e20-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="27e20-128">Poisto odottaa</span><span class="sxs-lookup"><span data-stu-id="27e20-128">Delete pending</span></span>  <br/> |<span data-ttu-id="27e20-129">Poistotoimintoa odotetaan.</span><span class="sxs-lookup"><span data-stu-id="27e20-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="27e20-130">Tunnistettu</span><span class="sxs-lookup"><span data-stu-id="27e20-130">Discovered</span></span>  <br/> |<span data-ttu-id="27e20-131">Microsoft 365 Business on tunnistanut laitteen.</span><span class="sxs-lookup"><span data-stu-id="27e20-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
