---
title: Autopilot-laitteen virheiden vianmääritys
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Lue tietoja automaattiohjauksen laitetiedostojen vianmäärityksestä Microsoft 365 Businessissa.
ms.openlocfilehash: 8b99e848fa040711785b921d12548f16dadb09af
ms.sourcegitcommit: 4a34b48584071e0c43c920bb35025e34cb4f5d15
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/09/2020
ms.locfileid: "43212129"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="1d051-103">Autopilot-laitteen virheiden vianmääritys</span><span class="sxs-lookup"><span data-stu-id="1d051-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="1d051-104">Laitetiedoston virhesanomat</span><span class="sxs-lookup"><span data-stu-id="1d051-104">Device file error messages</span></span>

<span data-ttu-id="1d051-105">Tässä on tietoja joistakin virheistä, joita saatat nähdä työskennellessäsi AutoPilot-laitetiedostojen kanssa Microsoft 365 Businessissa.</span><span class="sxs-lookup"><span data-stu-id="1d051-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="1d051-106">**Virhekoodi**</span><span class="sxs-lookup"><span data-stu-id="1d051-106">**Error code**</span></span>|<span data-ttu-id="1d051-107">**Yritä korjata**</span><span class="sxs-lookup"><span data-stu-id="1d051-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1d051-108">Virheellinen pyynnön teksti</span><span class="sxs-lookup"><span data-stu-id="1d051-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="1d051-109">Tämän virheen pitäisi tapahtua harvoin, jos näet tämän virheen, yritä toimintoa uudelleen.</span><span class="sxs-lookup"><span data-stu-id="1d051-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="1d051-110">Laitteen laitteiston hajautusarvo ei ole oikea.</span><span class="sxs-lookup"><span data-stu-id="1d051-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="1d051-111">Jos näet tämän virheen, se tarkoittaa, että CSV-tiedostossa antamasi arvo yhden laitteen laitteistohajautusarvolle ei ole oikea.</span><span class="sxs-lookup"><span data-stu-id="1d051-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="1d051-112">Varmista ensin, että arvo on kirjoitettu oikein.</span><span class="sxs-lookup"><span data-stu-id="1d051-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="1d051-113">Jos olet sitä mieltä, että arvo on oikea, mutta tämä virhe tapahtuu edelleen, pyydä apua laitteiston valmistajalta.</span><span class="sxs-lookup"><span data-stu-id="1d051-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="1d051-114">Toiselle vuokralaiselle määritetty laite</span><span class="sxs-lookup"><span data-stu-id="1d051-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="1d051-115">Jos näet tämän virheen, se tarkoittaa, että CSV-tiedostossa antamasi arvo yhden tai useamman laitteen sarjanumerolle tai tuotetunnukselle ei ole oikea.</span><span class="sxs-lookup"><span data-stu-id="1d051-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="1d051-116">Varmista ensin, että arvo on kirjoitettu oikein.</span><span class="sxs-lookup"><span data-stu-id="1d051-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="1d051-117">Jos olet sitä mieltä, että arvo on oikea, mutta tämä virhe tapahtuu edelleen, pyydä apua laitteiston valmistajalta.</span><span class="sxs-lookup"><span data-stu-id="1d051-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="1d051-118">CSV-tiedosto sisältää virheellisen sarjanumeron tai product key -tunnuksen</span><span class="sxs-lookup"><span data-stu-id="1d051-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="1d051-119">Jos näet tämän virheen, toinen organisaatio on jo rekisteröinyt laitteen, jota yrität rekisteröidä.</span><span class="sxs-lookup"><span data-stu-id="1d051-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="1d051-120">Voit korjata tämän virheen kysykää laitevalmistajaltaapua.</span><span class="sxs-lookup"><span data-stu-id="1d051-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="1d051-121">Tätä laitetta ei tueta automaattisen ohjauksen avulla</span><span class="sxs-lookup"><span data-stu-id="1d051-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="1d051-122">Tämä virhe tarkoittaa, että laite ei täytä AutoPilotin käyttöönottovaatimuksia.</span><span class="sxs-lookup"><span data-stu-id="1d051-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="1d051-123">Laitteiden on täytettävä nämä vaatimukset:</span><span class="sxs-lookup"><span data-stu-id="1d051-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="1d051-124">Windows 10, versio 1703 tai uudempi.</span><span class="sxs-lookup"><span data-stu-id="1d051-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="1d051-125">Uudet laitteet, joita ei ole käyty Windowsin käyttökokemuksen kautta.</span><span class="sxs-lookup"><span data-stu-id="1d051-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="1d051-126">Laitetta ei löydy</span><span class="sxs-lookup"><span data-stu-id="1d051-126">Device not found</span></span>  <br/> |<span data-ttu-id="1d051-127">Tämä virhe tarkoittaa, että yhtä tai useampaa CSV-tiedoston laitetta ei ole rekisteröity organisaatioosi.</span><span class="sxs-lookup"><span data-stu-id="1d051-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="1d051-128">Voit korjata ongelman kysykää laitevalmistajaltasi apua.</span><span class="sxs-lookup"><span data-stu-id="1d051-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
