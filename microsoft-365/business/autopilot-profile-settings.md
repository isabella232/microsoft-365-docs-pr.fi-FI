---
title: Tietoja Autopilot-profiilien asetuksista
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
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
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: AutoPilot-profiilien avulla voit hallita sitä, miten Windows asennetaan käyttäjien laitteisiin. Profiilit sisältävät oletusasetuksia ja valinnaisia asetuksia, kuten ohita Cortanan asennus.
ms.openlocfilehash: be10e0e1c8c96ce05aab8526d2010313662ed5f2
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913374"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="ae182-104">Tietoja Autopilot-profiilien asetuksista</span><span class="sxs-lookup"><span data-stu-id="ae182-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="ae182-105">Autopilot-profiilien asetukset</span><span class="sxs-lookup"><span data-stu-id="ae182-105">AutoPilot profile settings</span></span>

<span data-ttu-id="ae182-106">AutoPilot-profiilien avulla voit hallita sitä, miten Windows asennetaan käyttäjien laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="ae182-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="ae182-107">Profiilit sisältävät seuraavat asetukset.</span><span class="sxs-lookup"><span data-stu-id="ae182-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="ae182-108">**AutoPilot-oletusominaisuudet (pakollinen), jotka määritetään automaattisesti:**</span><span class="sxs-lookup"><span data-stu-id="ae182-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="ae182-109">**Asetus**</span><span class="sxs-lookup"><span data-stu-id="ae182-109">**Setting**</span></span>|<span data-ttu-id="ae182-110">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="ae182-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ae182-111">Ohita Cortana, OneDrive ja OEM-rekisteröinti</span><span class="sxs-lookup"><span data-stu-id="ae182-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="ae182-112">Asennus ohittaa kuluttajasovellusten, kuten Cortanan ja henkilökohtaisen OneDriven, asennuksen.</span><span class="sxs-lookup"><span data-stu-id="ae182-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="ae182-113">Laitteen käyttäjä voi asentaa ne myöhemmin, kunhan käyttäjä on paikallinen järjestelmänvalvoja laitteessa.</span><span class="sxs-lookup"><span data-stu-id="ae182-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="ae182-114">Alkuperäisen valmistajan rekisteröinti ohitetaan, koska laitetta hallitaan Microsoft 365 Business Premiumilla.</span><span class="sxs-lookup"><span data-stu-id="ae182-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="ae182-115">Yrityskuvan mukainen kirjautumiskokemus</span><span class="sxs-lookup"><span data-stu-id="ae182-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="ae182-116">Jos yritykselläsi on [Lisää yrityksesi brändi Microsoft 365:n](../admin/setup/customize-sign-in-page.md)kirjautumissivulle, laitteen käyttäjä saa tämän käyttökokemuksen kirjautumisen yhteydessä.</span><span class="sxs-lookup"><span data-stu-id="ae182-116">If your company has a [Add your company branding to Microsoft 365 Sign In page](../admin/setup/customize-sign-in-page.md), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="ae182-117">Automaattinen MDM-rekisteröinti määritetyillä AAD-tileillä</span><span class="sxs-lookup"><span data-stu-id="ae182-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="ae182-118">Käyttäjätietoja hallitaan Azure Active Directoryn avulla, ja käyttäjät kirjautuvat Windowsiin ja Microsoft 365:yn Microsoft 365 Business Premium -tunnistetiedoillaan.</span><span class="sxs-lookup"><span data-stu-id="ae182-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Microsoft 365 with their Microsoft 365 Business Premium credentials.</span></span>  <br/> |
   
 <span data-ttu-id="ae182-119">**Valinnaiset asetukset:**</span><span class="sxs-lookup"><span data-stu-id="ae182-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="ae182-120">**Asetus**</span><span class="sxs-lookup"><span data-stu-id="ae182-120">**Setting**</span></span>|<span data-ttu-id="ae182-121">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="ae182-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ae182-122">Ohita tietosuoja-asetukset (oletusarvoisesti poissa käytöstä)</span><span class="sxs-lookup"><span data-stu-id="ae182-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="ae182-123">Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei näe laitteen ja Windowsin käyttöoikeussopimusta kirjautuessaan ensimmäisen kerran.</span><span class="sxs-lookup"><span data-stu-id="ae182-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="ae182-124">Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi</span><span class="sxs-lookup"><span data-stu-id="ae182-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="ae182-125">Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei voi asentaa henkilökohtaisia sovelluksia, kuten Cortanaa.</span><span class="sxs-lookup"><span data-stu-id="ae182-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
