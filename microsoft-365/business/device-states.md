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
description: Lisätietoja eri laitetiloista on Microsoft 365 Businessin Järjestelmänvalvoja-aloitussivun Laitetoiminnot-luettelossa.
ms.openlocfilehash: 878050fbe11acca1d5d434a5d2ab0b5b48510e45
ms.sourcegitcommit: ab916c216053999c9c4ef4838217e82cd861f23f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2020
ms.locfileid: "42415661"
---
# <a name="device-states"></a><span data-ttu-id="da1b7-103">Laitteen tilat</span><span class="sxs-lookup"><span data-stu-id="da1b7-103">Device states</span></span>

<span data-ttu-id="da1b7-104">**Laitetoiminnot**-luettelon (hallintakeskuksen aloitussivu \> **Laitetoiminnot**) laitteilla voi olla seuraavat tilat.</span><span class="sxs-lookup"><span data-stu-id="da1b7-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="da1b7-106">**Tila**</span><span class="sxs-lookup"><span data-stu-id="da1b7-106">**Status**</span></span>|<span data-ttu-id="da1b7-107">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="da1b7-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="da1b7-108">Intunen hallitsema</span><span class="sxs-lookup"><span data-stu-id="da1b7-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="da1b7-109">Microsoft 365 Businessn hallitsema</span><span class="sxs-lookup"><span data-stu-id="da1b7-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="da1b7-110">Käytöstä poistaminen odottaa</span><span class="sxs-lookup"><span data-stu-id="da1b7-110">Retire pending</span></span>  <br/> |<span data-ttu-id="da1b7-111">Microsoft 365 Business on valmiina poistamaan yritystiedot laitteesta.</span><span class="sxs-lookup"><span data-stu-id="da1b7-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="da1b7-112">Käytöstä poistaminen on käynnissä</span><span class="sxs-lookup"><span data-stu-id="da1b7-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="da1b7-113">Microsoft 365 Business poistaa parhaillaan yritystietoja laitteesta.</span><span class="sxs-lookup"><span data-stu-id="da1b7-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="da1b7-114">Käytöstä poistaminen epäonnistui</span><span class="sxs-lookup"><span data-stu-id="da1b7-114">Retire failed</span></span>  <br/> | <span data-ttu-id="da1b7-115">Yritystietojen poisto epäonnistui.</span><span class="sxs-lookup"><span data-stu-id="da1b7-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="da1b7-116">Eläkkeelle peruuttaminen peruutettu</span><span class="sxs-lookup"><span data-stu-id="da1b7-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="da1b7-117">Eläkkeelle siirtyminen toiminto peruutettiin.</span><span class="sxs-lookup"><span data-stu-id="da1b7-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="da1b7-118">Tyhjennys odottaa</span><span class="sxs-lookup"><span data-stu-id="da1b7-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="da1b7-119">Tehdasasetusten palauttamista odotetaan.</span><span class="sxs-lookup"><span data-stu-id="da1b7-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="da1b7-120">Tyhjennys käynnissä</span><span class="sxs-lookup"><span data-stu-id="da1b7-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="da1b7-121">Tehdasasetusten palautus on määritetty.</span><span class="sxs-lookup"><span data-stu-id="da1b7-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="da1b7-122">Tyhjennys epäonnistui</span><span class="sxs-lookup"><span data-stu-id="da1b7-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="da1b7-123">Tehdasasetusten palautusta ei voitu tehdä.</span><span class="sxs-lookup"><span data-stu-id="da1b7-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="da1b7-124">Pyyhi peruutettu</span><span class="sxs-lookup"><span data-stu-id="da1b7-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="da1b7-125">Tehdaspyyhintä peruttiin.</span><span class="sxs-lookup"><span data-stu-id="da1b7-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="da1b7-126">Viallinen</span><span class="sxs-lookup"><span data-stu-id="da1b7-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="da1b7-127">Toiminto odottaa (tai on käynnissä), mutta laite ei ole kirjautunut sisään yli 30 päivään.</span><span class="sxs-lookup"><span data-stu-id="da1b7-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="da1b7-128">Poisto odottaa</span><span class="sxs-lookup"><span data-stu-id="da1b7-128">Delete pending</span></span>  <br/> |<span data-ttu-id="da1b7-129">Poistotoimintoa odotetaan.</span><span class="sxs-lookup"><span data-stu-id="da1b7-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="da1b7-130">Tunnistettu</span><span class="sxs-lookup"><span data-stu-id="da1b7-130">Discovered</span></span>  <br/> |<span data-ttu-id="da1b7-131">Microsoft 365 Business on tunnistanut laitteen.</span><span class="sxs-lookup"><span data-stu-id="da1b7-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
