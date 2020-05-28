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
description: AutoPilot-profiilien avulla voit hallita, miten Windows asennetaan käyttäjän laitteisiin. Profiilit sisältävät oletus- ja valinnaisia asetuksia, kuten Cortanan asennuksen ohituksen.
ms.openlocfilehash: 100de5e9548f901008d3ae154ac5a237ef265ffb
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/27/2020
ms.locfileid: "44401030"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="b424f-104">Tietoja Autopilot-profiilien asetuksista</span><span class="sxs-lookup"><span data-stu-id="b424f-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="b424f-105">Autopilot-profiilien asetukset</span><span class="sxs-lookup"><span data-stu-id="b424f-105">AutoPilot profile settings</span></span>

<span data-ttu-id="b424f-106">AutoPilot-profiilien avulla voit hallita, miten Windows on asennettu käyttäjän laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="b424f-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="b424f-107">Profiilit sisältävät seuraavat asetukset.</span><span class="sxs-lookup"><span data-stu-id="b424f-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="b424f-108">**AutoPilot-oletusominaisuudet (pakollinen), jotka määritetään automaattisesti:**</span><span class="sxs-lookup"><span data-stu-id="b424f-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="b424f-109">**Asetus**</span><span class="sxs-lookup"><span data-stu-id="b424f-109">**Setting**</span></span>|<span data-ttu-id="b424f-110">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="b424f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b424f-111">Ohita Cortanan, OneDriven ja OEM-rekisteröinnin</span><span class="sxs-lookup"><span data-stu-id="b424f-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="b424f-112">Asennus ohittaa kuluttajasovellusten, kuten Cortanan ja henkilökohtaisen OneDriven, asennuksen.</span><span class="sxs-lookup"><span data-stu-id="b424f-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="b424f-113">Laitteen käyttäjä voi asentaa ne myöhemmin, kunhan käyttäjä on laitteen paikallinen järjestelmänvalvoja.</span><span class="sxs-lookup"><span data-stu-id="b424f-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="b424f-114">Alkuperäinen valmistajan rekisteröinti ohitetaan, koska microsoft 365 Business Premium hallitsee laitetta.</span><span class="sxs-lookup"><span data-stu-id="b424f-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="b424f-115">Yrityskuvan mukainen kirjautumiskokemus</span><span class="sxs-lookup"><span data-stu-id="b424f-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="b424f-116">Jos yritykselläsi on [Lisää yrityksen brändäys Microsoft 365 -kirjautumissivulle -sivu,](https://docs.microsoft.com/microsoft-365/admin/setup/customize-sign-in-page)laitteen käyttäjä saa tämän kokemuksen kirjautuessaan sisään.</span><span class="sxs-lookup"><span data-stu-id="b424f-116">If your company has a [Add your company branding to Microsoft 365 Sign In page](https://docs.microsoft.com/microsoft-365/admin/setup/customize-sign-in-page), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="b424f-117">Automaattinen MDM-rekisteröinti määritetyillä AAD-tileillä</span><span class="sxs-lookup"><span data-stu-id="b424f-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="b424f-118">Käyttäjätietoja hallitsee Azure Active Directory, ja käyttäjät kirjautuvat Windowsiin ja Microsoft 365:een Microsoft 365 Business Premium -tunnistetiedoillaan.</span><span class="sxs-lookup"><span data-stu-id="b424f-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Microsoft 365 with their Microsoft 365 Business Premium credentials.</span></span>  <br/> |
   
 <span data-ttu-id="b424f-119">**Valinnaiset asetukset:**</span><span class="sxs-lookup"><span data-stu-id="b424f-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="b424f-120">**Asetus**</span><span class="sxs-lookup"><span data-stu-id="b424f-120">**Setting**</span></span>|<span data-ttu-id="b424f-121">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="b424f-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b424f-122">Ohita tietosuoja-asetukset (oletusarvoisesti poissa käytöstä)</span><span class="sxs-lookup"><span data-stu-id="b424f-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="b424f-123">Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei näe laitteen ja Windowsin käyttöoikeussopimusta kirjautuessaan ensimmäisen kerran.</span><span class="sxs-lookup"><span data-stu-id="b424f-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="b424f-124">Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi</span><span class="sxs-lookup"><span data-stu-id="b424f-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="b424f-125">Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei voi asentaa henkilökohtaisia sovelluksia, kuten Cortanaa.</span><span class="sxs-lookup"><span data-stu-id="b424f-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
   
