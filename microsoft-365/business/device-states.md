---
title: Laitteen tilat
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Lisätietoja laitteen eri muodoista on Microsoft 365 for Businessin hallintakeskuksen aloitussivun Laitetoiminnot-luettelossa.
ms.openlocfilehash: e6f1b428413d094e0a1ce3afb026528074038736
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578463"
---
# <a name="device-states"></a><span data-ttu-id="e66d1-103">Laitteen tilat</span><span class="sxs-lookup"><span data-stu-id="e66d1-103">Device states</span></span>

<span data-ttu-id="e66d1-104">Tämä artikkeli koskee Microsoft 365 Business Premiumia.</span><span class="sxs-lookup"><span data-stu-id="e66d1-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="e66d1-105">**Laitetoiminnot**-luettelon (hallintakeskuksen aloitussivu \> **Laitetoiminnot**) laitteilla voi olla seuraavat tilat.</span><span class="sxs-lookup"><span data-stu-id="e66d1-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="e66d1-107">**Tila**</span><span class="sxs-lookup"><span data-stu-id="e66d1-107">**Status**</span></span>|<span data-ttu-id="e66d1-108">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="e66d1-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e66d1-109">Intunen hallitsema</span><span class="sxs-lookup"><span data-stu-id="e66d1-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="e66d1-110">Microsoft 365 Business Premiumin hallinnoija.</span><span class="sxs-lookup"><span data-stu-id="e66d1-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="e66d1-111">Käytöstä poistaminen odottaa</span><span class="sxs-lookup"><span data-stu-id="e66d1-111">Retire pending</span></span>  <br/> |<span data-ttu-id="e66d1-112">Microsoft 365 Business Premium on valmistautumassa poistamaan yritystiedot laitteesta.</span><span class="sxs-lookup"><span data-stu-id="e66d1-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="e66d1-113">Käytöstä poistaminen on käynnissä</span><span class="sxs-lookup"><span data-stu-id="e66d1-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="e66d1-114">Microsoft 365 Business Premium poistaa tällä hetkellä yritystietoja laitteesta.</span><span class="sxs-lookup"><span data-stu-id="e66d1-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="e66d1-115">Käytöstä poistaminen epäonnistui</span><span class="sxs-lookup"><span data-stu-id="e66d1-115">Retire failed</span></span>  <br/> | <span data-ttu-id="e66d1-116">Yritystietojen poisto epäonnistui.</span><span class="sxs-lookup"><span data-stu-id="e66d1-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="e66d1-117">Käytöstä poistuminen peruutettu</span><span class="sxs-lookup"><span data-stu-id="e66d1-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="e66d1-118">Käytöstä poistunut toiminto peruutettiin.</span><span class="sxs-lookup"><span data-stu-id="e66d1-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="e66d1-119">Tyhjennys odottaa</span><span class="sxs-lookup"><span data-stu-id="e66d1-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="e66d1-120">Tehdasasetusten palauttamista odotetaan.</span><span class="sxs-lookup"><span data-stu-id="e66d1-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="e66d1-121">Tyhjennys käynnissä</span><span class="sxs-lookup"><span data-stu-id="e66d1-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="e66d1-122">Tehdasasetusten palautus on määritetty.</span><span class="sxs-lookup"><span data-stu-id="e66d1-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="e66d1-123">Tyhjennys epäonnistui</span><span class="sxs-lookup"><span data-stu-id="e66d1-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="e66d1-124">Tehdasasetusten palauttaminen ei pystynyt.</span><span class="sxs-lookup"><span data-stu-id="e66d1-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="e66d1-125">Tyhjennys peruutettu</span><span class="sxs-lookup"><span data-stu-id="e66d1-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="e66d1-126">Tehdasasetusten poisto peruutettiin.</span><span class="sxs-lookup"><span data-stu-id="e66d1-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="e66d1-127">Viallinen</span><span class="sxs-lookup"><span data-stu-id="e66d1-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="e66d1-128">Toiminto odottaa (tai on käynnissä), mutta laite ei ole kuitattu sisään yli 30 päivään.</span><span class="sxs-lookup"><span data-stu-id="e66d1-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="e66d1-129">Poisto odottaa</span><span class="sxs-lookup"><span data-stu-id="e66d1-129">Delete pending</span></span>  <br/> |<span data-ttu-id="e66d1-130">Poistotoimintoa odotetaan.</span><span class="sxs-lookup"><span data-stu-id="e66d1-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="e66d1-131">Tunnistettu</span><span class="sxs-lookup"><span data-stu-id="e66d1-131">Discovered</span></span>  <br/> |<span data-ttu-id="e66d1-132">Microsoft 365 Business Premium on havainnut laitteen.</span><span class="sxs-lookup"><span data-stu-id="e66d1-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
