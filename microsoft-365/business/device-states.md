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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Lue lisätietoja Microsoft 365 Businessin laitetiloista.
ms.openlocfilehash: 26b218cb7b6a14f17e33d34a2e712b06ac814c0c
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065758"
---
# <a name="device-states"></a><span data-ttu-id="7454c-103">Laitteen tilat</span><span class="sxs-lookup"><span data-stu-id="7454c-103">Device states</span></span>

<span data-ttu-id="7454c-104">**Laitetoiminnot**-luettelon (hallintakeskuksen aloitussivu \> **Laitetoiminnot**) laitteilla voi olla seuraavat tilat.</span><span class="sxs-lookup"><span data-stu-id="7454c-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="7454c-106">**Tila**</span><span class="sxs-lookup"><span data-stu-id="7454c-106">**Status**</span></span>|<span data-ttu-id="7454c-107">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="7454c-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7454c-108">Intunen hallitsema</span><span class="sxs-lookup"><span data-stu-id="7454c-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="7454c-109">Microsoft 365 Businessn hallitsema</span><span class="sxs-lookup"><span data-stu-id="7454c-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="7454c-110">Käytöstä poistaminen odottaa</span><span class="sxs-lookup"><span data-stu-id="7454c-110">Retire pending</span></span>  <br/> |<span data-ttu-id="7454c-111">Microsoft 365 Business on valmiina poistamaan yritystiedot laitteesta.</span><span class="sxs-lookup"><span data-stu-id="7454c-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="7454c-112">Käytöstä poistaminen on käynnissä</span><span class="sxs-lookup"><span data-stu-id="7454c-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="7454c-113">Microsoft 365 Business poistaa parhaillaan yritystietoja laitteesta.</span><span class="sxs-lookup"><span data-stu-id="7454c-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="7454c-114">Käytöstä poistaminen epäonnistui</span><span class="sxs-lookup"><span data-stu-id="7454c-114">Retire failed</span></span>  <br/> | <span data-ttu-id="7454c-115">Yritystietojen poisto epäonnistui.</span><span class="sxs-lookup"><span data-stu-id="7454c-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="7454c-116">Eläkkeelle peruuttaminen peruutettu</span><span class="sxs-lookup"><span data-stu-id="7454c-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="7454c-117">Eläkkeelle siirtyminen toiminto peruutettiin.</span><span class="sxs-lookup"><span data-stu-id="7454c-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="7454c-118">Tyhjennys odottaa</span><span class="sxs-lookup"><span data-stu-id="7454c-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="7454c-119">Tehdasasetusten palauttamista odotetaan.</span><span class="sxs-lookup"><span data-stu-id="7454c-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="7454c-120">Tyhjennys käynnissä</span><span class="sxs-lookup"><span data-stu-id="7454c-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="7454c-121">Tehdasasetusten palautus on määritetty.</span><span class="sxs-lookup"><span data-stu-id="7454c-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="7454c-122">Tyhjennys epäonnistui</span><span class="sxs-lookup"><span data-stu-id="7454c-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="7454c-123">Tehdasasetusten palautusta ei voitu tehdä.</span><span class="sxs-lookup"><span data-stu-id="7454c-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="7454c-124">Pyyhi peruutettu</span><span class="sxs-lookup"><span data-stu-id="7454c-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="7454c-125">Tehdaspyyhintä peruttiin.</span><span class="sxs-lookup"><span data-stu-id="7454c-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="7454c-126">Viallinen</span><span class="sxs-lookup"><span data-stu-id="7454c-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="7454c-127">Toiminto odottaa (tai on käynnissä), mutta laite ei ole kirjautunut sisään yli 30 päivään.</span><span class="sxs-lookup"><span data-stu-id="7454c-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="7454c-128">Poisto odottaa</span><span class="sxs-lookup"><span data-stu-id="7454c-128">Delete pending</span></span>  <br/> |<span data-ttu-id="7454c-129">Poistotoimintoa odotetaan.</span><span class="sxs-lookup"><span data-stu-id="7454c-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="7454c-130">Tunnistettu</span><span class="sxs-lookup"><span data-stu-id="7454c-130">Discovered</span></span>  <br/> |<span data-ttu-id="7454c-131">Microsoft 365 Business on tunnistanut laitteen.</span><span class="sxs-lookup"><span data-stu-id="7454c-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
