---
title: Autopilot-laitteen virheiden vianmääritys
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: troubleshooting
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Opi automaattiohjauksen laitteen tiedostojen virheiden vianmääritys.
ms.openlocfilehash: 9b8d8ab424dd3189ff5c228dab8f5c513ff5dafc
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982743"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="a91a6-103">Autopilot-laitteen virheiden vianmääritys</span><span class="sxs-lookup"><span data-stu-id="a91a6-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="a91a6-104">Lokitiedoston virhesanomia laitetta</span><span class="sxs-lookup"><span data-stu-id="a91a6-104">Device file error messages</span></span>

<span data-ttu-id="a91a6-105">Seuraavassa on joitakin virheitä, tiedot, näyttöön saattaa tulla käsitellessäsi automaattiohjauksen laitteen tiedostoja Microsoft Business-365.</span><span class="sxs-lookup"><span data-stu-id="a91a6-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="a91a6-106">**Virhekoodi**</span><span class="sxs-lookup"><span data-stu-id="a91a6-106">**Error code**</span></span>|<span data-ttu-id="a91a6-107">**Yritä korjata**</span><span class="sxs-lookup"><span data-stu-id="a91a6-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a91a6-108">Virheellinen pyynnön rungon</span><span class="sxs-lookup"><span data-stu-id="a91a6-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="a91a6-109">Tämä virhe tapahtuu harvoin, jos tämä virhe, yritä uudelleen.</span><span class="sxs-lookup"><span data-stu-id="a91a6-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="a91a6-110">Laitteen laitteiston hajautusarvo ei ole oikea.</span><span class="sxs-lookup"><span data-stu-id="a91a6-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="a91a6-p101">Jos näet tämän virheen, se tarkoittaa, että yhteen laitteeseen, laitteiston hajautusalgoritmi CSV-tiedostosi annettu arvo ei ole oikea. Varmista, että arvo on kirjoitettu oikein. Jos olet sitä mieltä, että arvo on oikein, mutta tämä virhe tapahtuu edelleen, kysy laitteen valmistajalta apua.</span><span class="sxs-lookup"><span data-stu-id="a91a6-p101">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct. First, verify that the value was typed correctly. If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="a91a6-114">Toisen vuokralaisen liitetyn laitteen</span><span class="sxs-lookup"><span data-stu-id="a91a6-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="a91a6-p102">Jos näet tämän virheen, se tarkoittaa sarjanumero tai product key-tunnus ja yksi tai useampi laite CSV-tiedosto annetun arvon oikeaksi. Varmista, että arvo on kirjoitettu oikein. Jos olet sitä mieltä, että arvo on oikein, mutta tämä virhe tapahtuu edelleen, kysy laitteen valmistajalta apua.</span><span class="sxs-lookup"><span data-stu-id="a91a6-p102">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct. First, verify that the value was typed correctly. If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="a91a6-118">CSV-tiedosto sisältää virheellinen sarjanumero tai product key-tunnus</span><span class="sxs-lookup"><span data-stu-id="a91a6-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="a91a6-p103">Jos näet tämän virheen, se tarkoittaa, että organisaatio on jo rekisteröity-tilassa yritettäessä rekisteröidä laitteelle. Voit korjata tämän, pyydä apua laitteen valmistajalta.</span><span class="sxs-lookup"><span data-stu-id="a91a6-p103">If you see this error it means that the device you are tyring to register is already registered by an other organization. To fix this, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="a91a6-121">Tämä laite ei tue asennuksen automaattiohjauksen avulla</span><span class="sxs-lookup"><span data-stu-id="a91a6-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="a91a6-p104">Tämä virhe tarkoittaa, että laite ei täytä automaattiohjauksen käyttöönoton. Laitteet tarvitsevat näitä vaatimuksia:</span><span class="sxs-lookup"><span data-stu-id="a91a6-p104">This error means the device does not meet AutoPilot deployment requirements. Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="a91a6-124">Windows 10, versio 1703 tai uudempi.</span><span class="sxs-lookup"><span data-stu-id="a91a6-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="a91a6-125">Uudet laitteet, joita ei ole määritetty Windowsin tervetuloa-ohjelmassa.</span><span class="sxs-lookup"><span data-stu-id="a91a6-125">New devices that have not been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="a91a6-126">Laitetta ei löydy</span><span class="sxs-lookup"><span data-stu-id="a91a6-126">Device not found</span></span>  <br/> |<span data-ttu-id="a91a6-p105">Tämä virhe tarkoittaa, että yksi tai useampi laite CSV-tiedostossa ei ole rekisteröity organisaation. Voit korjata tämän, pyydä apua laitteen valmistajalta.</span><span class="sxs-lookup"><span data-stu-id="a91a6-p105">This error means that one or more devices in your CSV file is not registered to your organization. To fix this, ask your hardware vendor for help.</span></span>  <br/> |
   
