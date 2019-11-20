---
title: Autopilot-laitteen virheiden vianmääritys
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: troubleshooting
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Tietoja automaatti ohjauksen laite virheiden vian määrityksestä.
ms.openlocfilehash: 1b5358bd6686c2548e82ec5297ac0ad675835718
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718695"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="94fc4-103">Autopilot-laitteen virheiden vianmääritys</span><span class="sxs-lookup"><span data-stu-id="94fc4-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="94fc4-104">Laite tiedoston virhe sanomat</span><span class="sxs-lookup"><span data-stu-id="94fc4-104">Device file error messages</span></span>

<span data-ttu-id="94fc4-105">Tässä on tietoja joistakin virheistä, joita saatat nähdä työskennellessään automaatti ohjauksen laite tiedostojen kanssa Microsoft 365 Businessissa.</span><span class="sxs-lookup"><span data-stu-id="94fc4-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="94fc4-106">**Virhekoodi**</span><span class="sxs-lookup"><span data-stu-id="94fc4-106">**Error code**</span></span>|<span data-ttu-id="94fc4-107">**Fix kokeilla**</span><span class="sxs-lookup"><span data-stu-id="94fc4-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="94fc4-108">Virheellinen pyynnön leipä teksti</span><span class="sxs-lookup"><span data-stu-id="94fc4-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="94fc4-109">Tämän virheen pitäisi tapahtua harvoin, jos näet tämän virheen, yritä toimintoa uudelleen.</span><span class="sxs-lookup"><span data-stu-id="94fc4-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="94fc4-110">Laitteen laitteiston hajautus arvo ei ole oikea.</span><span class="sxs-lookup"><span data-stu-id="94fc4-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="94fc4-111">Jos näet tämän virheen, se tarkoittaa, että yhden laitteen laitteiston hajautus arvon CSV-tiedostossa antama arvo ei ole oikea.</span><span class="sxs-lookup"><span data-stu-id="94fc4-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="94fc4-112">Tarkista ensin, että arvo on kirjoitettu oikein.</span><span class="sxs-lookup"><span data-stu-id="94fc4-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="94fc4-113">Jos arvelet, että arvo on oikea, mutta tämä virhe tapahtuu edelleen, pyydä apua laitteiston toimittajalta.</span><span class="sxs-lookup"><span data-stu-id="94fc4-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="94fc4-114">Toiseen vuokraajaan liitetty laite</span><span class="sxs-lookup"><span data-stu-id="94fc4-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="94fc4-115">Jos näet tämän virheen, se tarkoittaa, että CSV-tiedostossa annettu arvo joko yhden tai useamman laitteen sarja numeroa tai Product Key-tunnusta varten ei ole oikea.</span><span class="sxs-lookup"><span data-stu-id="94fc4-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="94fc4-116">Tarkista ensin, että arvo on kirjoitettu oikein.</span><span class="sxs-lookup"><span data-stu-id="94fc4-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="94fc4-117">Jos arvelet, että arvo on oikea, mutta tämä virhe tapahtuu edelleen, pyydä apua laitteiston toimittajalta.</span><span class="sxs-lookup"><span data-stu-id="94fc4-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="94fc4-118">CSV-tiedostossa on virheellinen sarja numero tai Product Key-tunnus</span><span class="sxs-lookup"><span data-stu-id="94fc4-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="94fc4-119">Jos näet tämän virheen, se tarkoittaa, että laite, jota yrität rekisteröidä, on jo toisen organisaation rekisteröimää.</span><span class="sxs-lookup"><span data-stu-id="94fc4-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="94fc4-120">Voit korjata tämän virheen pyytämällä laitteiston toimittajalta apua.</span><span class="sxs-lookup"><span data-stu-id="94fc4-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="94fc4-121">Tätä laitetta ei tueta asennuksessa käyttämällä automaatti ohjausta</span><span class="sxs-lookup"><span data-stu-id="94fc4-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="94fc4-122">Tämä virhe tarkoittaa, että laite ei vastaa automaatti ohjauksen käyttöönoton vaatimuksia.</span><span class="sxs-lookup"><span data-stu-id="94fc4-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="94fc4-123">Laitteiden on täytettävä nämä vaatimukset:</span><span class="sxs-lookup"><span data-stu-id="94fc4-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="94fc4-124">Windows 10, versio 1703 tai uudempi.</span><span class="sxs-lookup"><span data-stu-id="94fc4-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="94fc4-125">Uudet laitteet, jotka eivät ole olleet Windows out-of-Box-kokemuksen kautta.</span><span class="sxs-lookup"><span data-stu-id="94fc4-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="94fc4-126">Laitetta ei löydy</span><span class="sxs-lookup"><span data-stu-id="94fc4-126">Device not found</span></span>  <br/> |<span data-ttu-id="94fc4-127">Tämä virhe tarkoittaa sitä, että yhtä tai useampaa CSV-tiedostossa olevaa laitetta ei ole rekisteröity organisaatioosi.</span><span class="sxs-lookup"><span data-stu-id="94fc4-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="94fc4-128">Voit korjata tämän ongelman pyytämällä laitteiston toimittajalta apua.</span><span class="sxs-lookup"><span data-stu-id="94fc4-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
