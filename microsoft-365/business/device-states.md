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
description: Lisätietoja Microsoft 365 for Businessin Hallinta-kotisivun Laitetoiminnot-luettelon eri laitetilojen tiloista.
ms.openlocfilehash: 64138e2b6ae73c067709cde1912a96615d08ebf1
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471175"
---
# <a name="device-states"></a><span data-ttu-id="84e0b-103">Laitteen tilat</span><span class="sxs-lookup"><span data-stu-id="84e0b-103">Device states</span></span>

<span data-ttu-id="84e0b-104">Tämä artikkeli koskee Microsoft 365 Business Premiumia.</span><span class="sxs-lookup"><span data-stu-id="84e0b-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="84e0b-105">**Laitetoiminnot**-luettelon (hallintakeskuksen aloitussivu \> **Laitetoiminnot**) laitteilla voi olla seuraavat tilat.</span><span class="sxs-lookup"><span data-stu-id="84e0b-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="84e0b-107">**Tila**</span><span class="sxs-lookup"><span data-stu-id="84e0b-107">**Status**</span></span>|<span data-ttu-id="84e0b-108">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="84e0b-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="84e0b-109">Intunen hallitsema</span><span class="sxs-lookup"><span data-stu-id="84e0b-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="84e0b-110">Microsoft 365 Business Premiumin hallinnoima.</span><span class="sxs-lookup"><span data-stu-id="84e0b-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="84e0b-111">Käytöstä poistaminen odottaa</span><span class="sxs-lookup"><span data-stu-id="84e0b-111">Retire pending</span></span>  <br/> |<span data-ttu-id="84e0b-112">Microsoft 365 Business Premium valmistautuu poistamaan yrityksen tiedot laitteesta.</span><span class="sxs-lookup"><span data-stu-id="84e0b-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="84e0b-113">Käytöstä poistaminen on käynnissä</span><span class="sxs-lookup"><span data-stu-id="84e0b-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="84e0b-114">Microsoft 365 Business Premium poistaa parhaillaan yrityksen tietoja laitteesta.</span><span class="sxs-lookup"><span data-stu-id="84e0b-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="84e0b-115">Käytöstä poistaminen epäonnistui</span><span class="sxs-lookup"><span data-stu-id="84e0b-115">Retire failed</span></span>  <br/> | <span data-ttu-id="84e0b-116">Yritystietojen poisto epäonnistui.</span><span class="sxs-lookup"><span data-stu-id="84e0b-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="84e0b-117">Eläkkeelle siirtyminen peruutettu</span><span class="sxs-lookup"><span data-stu-id="84e0b-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="84e0b-118">Eläkkeelle siirtymistä koskeva toiminto peruutettiin.</span><span class="sxs-lookup"><span data-stu-id="84e0b-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="84e0b-119">Tyhjennys odottaa</span><span class="sxs-lookup"><span data-stu-id="84e0b-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="84e0b-120">Tehdasasetusten palauttamista odotetaan.</span><span class="sxs-lookup"><span data-stu-id="84e0b-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="84e0b-121">Tyhjennys käynnissä</span><span class="sxs-lookup"><span data-stu-id="84e0b-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="84e0b-122">Tehdasasetusten palautus on määritetty.</span><span class="sxs-lookup"><span data-stu-id="84e0b-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="84e0b-123">Tyhjennys epäonnistui</span><span class="sxs-lookup"><span data-stu-id="84e0b-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="84e0b-124">Tehdasasetusten palautusta ei voitu tehdä.</span><span class="sxs-lookup"><span data-stu-id="84e0b-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="84e0b-125">Pyyhi peruutettu</span><span class="sxs-lookup"><span data-stu-id="84e0b-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="84e0b-126">Tehdaspyyhin peruutettiin.</span><span class="sxs-lookup"><span data-stu-id="84e0b-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="84e0b-127">Viallinen</span><span class="sxs-lookup"><span data-stu-id="84e0b-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="84e0b-128">Toiminto odottaa (tai on käynnissä), mutta laite ei ole kirjautunut sisään 30+ päivään.</span><span class="sxs-lookup"><span data-stu-id="84e0b-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="84e0b-129">Poisto odottaa</span><span class="sxs-lookup"><span data-stu-id="84e0b-129">Delete pending</span></span>  <br/> |<span data-ttu-id="84e0b-130">Poistotoimintoa odotetaan.</span><span class="sxs-lookup"><span data-stu-id="84e0b-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="84e0b-131">Tunnistettu</span><span class="sxs-lookup"><span data-stu-id="84e0b-131">Discovered</span></span>  <br/> |<span data-ttu-id="84e0b-132">Microsoft 365 Business Premium on havainnut laitteen.</span><span class="sxs-lookup"><span data-stu-id="84e0b-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
