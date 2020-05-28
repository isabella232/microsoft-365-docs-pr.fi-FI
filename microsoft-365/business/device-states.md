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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Lisätietoja eri laitetiloista on Microsoft 365 for Businessin Järjestelmänvalvoja-aloitussivun Laitetoiminnot-luettelossa.
ms.openlocfilehash: 90c11caa03249408ba2916d303bcb4a59fbcca8c
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400950"
---
# <a name="device-states"></a><span data-ttu-id="405a8-103">Laitteen tilat</span><span class="sxs-lookup"><span data-stu-id="405a8-103">Device states</span></span>

<span data-ttu-id="405a8-104">**Laitetoiminnot**-luettelon (hallintakeskuksen aloitussivu \> **Laitetoiminnot**) laitteilla voi olla seuraavat tilat.</span><span class="sxs-lookup"><span data-stu-id="405a8-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="405a8-106">**Tila**</span><span class="sxs-lookup"><span data-stu-id="405a8-106">**Status**</span></span>|<span data-ttu-id="405a8-107">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="405a8-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="405a8-108">Intunen hallitsema</span><span class="sxs-lookup"><span data-stu-id="405a8-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="405a8-109">Microsoft 365 Business Premiumin hallinnoima.</span><span class="sxs-lookup"><span data-stu-id="405a8-109">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="405a8-110">Käytöstä poistaminen odottaa</span><span class="sxs-lookup"><span data-stu-id="405a8-110">Retire pending</span></span>  <br/> |<span data-ttu-id="405a8-111">Microsoft 365 Business Premium valmistautuu poistamaan yrityksen tiedot laitteesta.</span><span class="sxs-lookup"><span data-stu-id="405a8-111">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="405a8-112">Käytöstä poistaminen on käynnissä</span><span class="sxs-lookup"><span data-stu-id="405a8-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="405a8-113">Microsoft 365 Business Premium poistaa parhaillaan yrityksen tietoja laitteesta.</span><span class="sxs-lookup"><span data-stu-id="405a8-113">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="405a8-114">Käytöstä poistaminen epäonnistui</span><span class="sxs-lookup"><span data-stu-id="405a8-114">Retire failed</span></span>  <br/> | <span data-ttu-id="405a8-115">Yritystietojen poisto epäonnistui.</span><span class="sxs-lookup"><span data-stu-id="405a8-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="405a8-116">Eläkkeelle peruutettu</span><span class="sxs-lookup"><span data-stu-id="405a8-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="405a8-117">Eläkkeelle siirtyminen peruutettiin.</span><span class="sxs-lookup"><span data-stu-id="405a8-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="405a8-118">Tyhjennys odottaa</span><span class="sxs-lookup"><span data-stu-id="405a8-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="405a8-119">Tehdasasetusten palauttamista odotetaan.</span><span class="sxs-lookup"><span data-stu-id="405a8-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="405a8-120">Tyhjennys käynnissä</span><span class="sxs-lookup"><span data-stu-id="405a8-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="405a8-121">Tehdasasetusten palautus on määritetty.</span><span class="sxs-lookup"><span data-stu-id="405a8-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="405a8-122">Tyhjennys epäonnistui</span><span class="sxs-lookup"><span data-stu-id="405a8-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="405a8-123">Tehdasasetusten palautusta ei voitu tehdä.</span><span class="sxs-lookup"><span data-stu-id="405a8-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="405a8-124">Pyyhitään peruutettu</span><span class="sxs-lookup"><span data-stu-id="405a8-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="405a8-125">Tehdaspyyhintä peruttiin.</span><span class="sxs-lookup"><span data-stu-id="405a8-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="405a8-126">Viallinen</span><span class="sxs-lookup"><span data-stu-id="405a8-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="405a8-127">Toiminto odottaa (tai on käynnissä), mutta laite ei ole kirjautunut sisään yli 30 päivään.</span><span class="sxs-lookup"><span data-stu-id="405a8-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="405a8-128">Poisto odottaa</span><span class="sxs-lookup"><span data-stu-id="405a8-128">Delete pending</span></span>  <br/> |<span data-ttu-id="405a8-129">Poistotoimintoa odotetaan.</span><span class="sxs-lookup"><span data-stu-id="405a8-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="405a8-130">Tunnistettu</span><span class="sxs-lookup"><span data-stu-id="405a8-130">Discovered</span></span>  <br/> |<span data-ttu-id="405a8-131">Microsoft 365 Business Premium on havainnut laitteen.</span><span class="sxs-lookup"><span data-stu-id="405a8-131">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
