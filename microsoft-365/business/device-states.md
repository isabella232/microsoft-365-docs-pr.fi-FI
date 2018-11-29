---
title: Laitteen tilat
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
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
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Lisätietoja laitteen valtioiden Microsoft Business-365.
ms.openlocfilehash: bd6f1ad7f7671d9616fd14d477dfcfb164ff6bd0
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982903"
---
# <a name="device-states"></a><span data-ttu-id="89ed0-103">Laitteen tilat</span><span class="sxs-lookup"><span data-stu-id="89ed0-103">Device states</span></span>

## <a name="device-states"></a><span data-ttu-id="89ed0-104">Laitteen tilat</span><span class="sxs-lookup"><span data-stu-id="89ed0-104">Device states</span></span>

<span data-ttu-id="89ed0-105">**Laitetoiminnot**-luettelon (hallintakeskuksen aloitussivu \> **Laitetoiminnot**) laitteilla voi olla seuraavat tilat.</span><span class="sxs-lookup"><span data-stu-id="89ed0-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="89ed0-107">**Tila**</span><span class="sxs-lookup"><span data-stu-id="89ed0-107">**Status**</span></span>|<span data-ttu-id="89ed0-108">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="89ed0-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="89ed0-109">Intunen hallitsema</span><span class="sxs-lookup"><span data-stu-id="89ed0-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="89ed0-110">Microsoft 365 Businessn hallitsema</span><span class="sxs-lookup"><span data-stu-id="89ed0-110">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="89ed0-111">Käytöstä poistaminen odottaa</span><span class="sxs-lookup"><span data-stu-id="89ed0-111">Retire pending</span></span>  <br/> |<span data-ttu-id="89ed0-112">Microsoft 365 Business on valmiina poistamaan yritystiedot laitteesta.</span><span class="sxs-lookup"><span data-stu-id="89ed0-112">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="89ed0-113">Käytöstä poistaminen on käynnissä</span><span class="sxs-lookup"><span data-stu-id="89ed0-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="89ed0-114">Microsoft 365 Business poistaa parhaillaan yritystietoja laitteesta.</span><span class="sxs-lookup"><span data-stu-id="89ed0-114">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="89ed0-115">Käytöstä poistaminen epäonnistui</span><span class="sxs-lookup"><span data-stu-id="89ed0-115">Retire failed</span></span>  <br/> | <span data-ttu-id="89ed0-116">Yritystietojen poisto epäonnistui.</span><span class="sxs-lookup"><span data-stu-id="89ed0-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="89ed0-117">Käytöstä poistaminen peruutettu</span><span class="sxs-lookup"><span data-stu-id="89ed0-117">Retire cancelled</span></span>  <br/> |<span data-ttu-id="89ed0-118">Käytöstä poistaminen peruutettiin.</span><span class="sxs-lookup"><span data-stu-id="89ed0-118">Retire action was cancelled.</span></span>  <br/> |
|<span data-ttu-id="89ed0-119">Tyhjennys odottaa</span><span class="sxs-lookup"><span data-stu-id="89ed0-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="89ed0-120">Tehdasasetusten palauttamista odotetaan.</span><span class="sxs-lookup"><span data-stu-id="89ed0-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="89ed0-121">Tyhjennys käynnissä</span><span class="sxs-lookup"><span data-stu-id="89ed0-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="89ed0-122">Tehdasasetusten palautus on määritetty.</span><span class="sxs-lookup"><span data-stu-id="89ed0-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="89ed0-123">Tyhjennys epäonnistui</span><span class="sxs-lookup"><span data-stu-id="89ed0-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="89ed0-124">Tehdasasetusten palautusta ei voitu suorittaa.</span><span class="sxs-lookup"><span data-stu-id="89ed0-124">Couldn't perform factory reset.</span></span>  <br/> |
|<span data-ttu-id="89ed0-125">Tyhjennys peruutettu</span><span class="sxs-lookup"><span data-stu-id="89ed0-125">Wipe cancelled</span></span>  <br/> |<span data-ttu-id="89ed0-126">Tehdasasetusten tyhjennys peruutettiin.</span><span class="sxs-lookup"><span data-stu-id="89ed0-126">Factory wipe was cancelled.</span></span>  <br/> |
|<span data-ttu-id="89ed0-127">Viallinen</span><span class="sxs-lookup"><span data-stu-id="89ed0-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="89ed0-128">Tämä tarkoittaa, että toiminto odottaa (tai on käynnissä), mutta laite ei ole rekisteröitynyt yli 30:een päivään.</span><span class="sxs-lookup"><span data-stu-id="89ed0-128">This means that an action is pending (or in progress) but the device has not checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="89ed0-129">Poisto odottaa</span><span class="sxs-lookup"><span data-stu-id="89ed0-129">Delete pending</span></span>  <br/> |<span data-ttu-id="89ed0-130">Poistotoimintoa odotetaan.</span><span class="sxs-lookup"><span data-stu-id="89ed0-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="89ed0-131">Tunnistettu</span><span class="sxs-lookup"><span data-stu-id="89ed0-131">Discovered</span></span>  <br/> |<span data-ttu-id="89ed0-132">Microsoft 365 Business on tunnistanut laitteen.</span><span class="sxs-lookup"><span data-stu-id="89ed0-132">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
