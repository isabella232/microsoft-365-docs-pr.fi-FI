---
title: Autopilot-laitteen virheiden vianmääritys
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Lue, miten voit tehdä vianmäärityksen, jonka saatat nähdä, kun käytät AutoPilot-laitetiedostoja Microsoft 365 Business Premiumissa.
ms.openlocfilehash: 1078ab74b07952e4bb565555a081b98ecce9db5c
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578083"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="7c449-103">Autopilot-laitteen virheiden vianmääritys</span><span class="sxs-lookup"><span data-stu-id="7c449-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="7c449-104">Laitetiedoston virhesanomat</span><span class="sxs-lookup"><span data-stu-id="7c449-104">Device file error messages</span></span>

<span data-ttu-id="7c449-105">Seuraavassa on tietoja virheistä, joita saatat nähdä, kun käytät AutoPilot-laitetiedostoja Microsoft 365 Business Premiumissa.</span><span class="sxs-lookup"><span data-stu-id="7c449-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business Premium.</span></span> 
  
|<span data-ttu-id="7c449-106">**Virhekoodi**</span><span class="sxs-lookup"><span data-stu-id="7c449-106">**Error code**</span></span>|<span data-ttu-id="7c449-107">**Korjaus kokeilemaan**</span><span class="sxs-lookup"><span data-stu-id="7c449-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7c449-108">Virheellinen pyynnön tekstiosa</span><span class="sxs-lookup"><span data-stu-id="7c449-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="7c449-109">Tämän virheen pitäisi tapahtua harvoin, jos näet tämän virheen, yritä toimintoa uudelleen.</span><span class="sxs-lookup"><span data-stu-id="7c449-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="7c449-110">Laitteen laitteiston hash-arvo ei ole oikein.</span><span class="sxs-lookup"><span data-stu-id="7c449-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="7c449-111">Jos näet tämän virheen, se tarkoittaa, että yhden laitteen laitteiston hash-arvo CSV-tiedostossa ei ole oikein.</span><span class="sxs-lookup"><span data-stu-id="7c449-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="7c449-112">Varmista ensin, että arvo on kirjoitettu oikein.</span><span class="sxs-lookup"><span data-stu-id="7c449-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="7c449-113">Jos uskot, että arvo on oikea, mutta virhe ilmenee edelleen, pyydä apua laitteiston toimittajalta.</span><span class="sxs-lookup"><span data-stu-id="7c449-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="7c449-114">Toiselle vuokraajassa määritetty laite</span><span class="sxs-lookup"><span data-stu-id="7c449-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="7c449-115">Jos näet tämän virheen, csv-tiedostossa annettu arvo, joka on joko sarjanumero tai yhden tai useamman laitteen tuoteavain, ei ole oikein.</span><span class="sxs-lookup"><span data-stu-id="7c449-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="7c449-116">Varmista ensin, että arvo on kirjoitettu oikein.</span><span class="sxs-lookup"><span data-stu-id="7c449-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="7c449-117">Jos uskot, että arvo on oikea, mutta virhe ilmenee edelleen, pyydä apua laitteiston toimittajalta.</span><span class="sxs-lookup"><span data-stu-id="7c449-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="7c449-118">CSV-tiedosto sisältää virheellisen sarjanumeron tai tuoteavaimen</span><span class="sxs-lookup"><span data-stu-id="7c449-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="7c449-119">Jos tämä virhe ilmenee, toinen organisaatio on jo rekisteröinyt laitteen, jota yrität rekisteröidä.</span><span class="sxs-lookup"><span data-stu-id="7c449-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="7c449-120">Voit korjata tämän virheen pyytämällä apua laitteiston toimittajalta.</span><span class="sxs-lookup"><span data-stu-id="7c449-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="7c449-121">Tätä laitetta ei tueta autopilotin määrityksessä</span><span class="sxs-lookup"><span data-stu-id="7c449-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="7c449-122">Tämä virhe tarkoittaa, että laite ei täytä AutoPilot-käyttöönottovaatimuksia.</span><span class="sxs-lookup"><span data-stu-id="7c449-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="7c449-123">Laitteiden on täytettävä nämä vaatimukset:</span><span class="sxs-lookup"><span data-stu-id="7c449-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="7c449-124">Windows 10, versio 1703 tai uudempi.</span><span class="sxs-lookup"><span data-stu-id="7c449-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="7c449-125">Uudet laitteet, jotka eivät ole käyneet läpi Windowsin käyttökokemusta.</span><span class="sxs-lookup"><span data-stu-id="7c449-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="7c449-126">Laitetta ei löydy</span><span class="sxs-lookup"><span data-stu-id="7c449-126">Device not found</span></span>  <br/> |<span data-ttu-id="7c449-127">Tämä virhe tarkoittaa, että vähintään yhtä CSV-tiedoston laitetta ei ole rekisteröity organisaatiollesi.</span><span class="sxs-lookup"><span data-stu-id="7c449-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="7c449-128">Voit korjata ongelman pyytämällä apua laitteiston toimittajalta.</span><span class="sxs-lookup"><span data-stu-id="7c449-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
