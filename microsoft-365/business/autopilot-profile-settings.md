---
title: Tietoja Autopilot-profiilien asetuksista
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Automaatti ohjaus profiilien avulla voit hallita sitä, miten Windows asennetaan käyttäjä laitteisiin. Profiilit sisältävät oletusarvoisia ja valinnaisia asetuksia, kuten Ohita Cortanan asennus.
ms.openlocfilehash: 912a24e3d458986a4bcf7dcf903f80211996aca2
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/14/2019
ms.locfileid: "38321781"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="6bbd0-104">Tietoja Autopilot-profiilien asetuksista</span><span class="sxs-lookup"><span data-stu-id="6bbd0-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="6bbd0-105">Autopilot-profiilien asetukset</span><span class="sxs-lookup"><span data-stu-id="6bbd0-105">AutoPilot profile settings</span></span>

<span data-ttu-id="6bbd0-106">Automaatti ohjaus profiilien avulla voit määrittää, miten Windows asennetaan käyttäjä laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="6bbd0-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="6bbd0-107">Profiilit sisältävät seuraavat asetukset.</span><span class="sxs-lookup"><span data-stu-id="6bbd0-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="6bbd0-108">**AutoPilot-oletusominaisuudet (pakollinen), jotka määritetään automaattisesti:**</span><span class="sxs-lookup"><span data-stu-id="6bbd0-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="6bbd0-109">**Asetus**</span><span class="sxs-lookup"><span data-stu-id="6bbd0-109">**Setting**</span></span>|<span data-ttu-id="6bbd0-110">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="6bbd0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6bbd0-111">Ohita Cortana, OneDrive ja OEM-rekisteröinti</span><span class="sxs-lookup"><span data-stu-id="6bbd0-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="6bbd0-112">Asennus ohittaa kuluttajasovellusten, kuten Cortanan ja henkilökohtaisen OneDriven, asennuksen.</span><span class="sxs-lookup"><span data-stu-id="6bbd0-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="6bbd0-113">Laitteen käyttäjä voi asentaa nämä myöhemmin, kunhan käyttäjä on laitteen paikallinen järjestelmänvalvoja.</span><span class="sxs-lookup"><span data-stu-id="6bbd0-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="6bbd0-114">Alkuperäisen laitevalmistajan rekisteröinti ohitetaan, koska laitteen hallinnasta vastaa Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="6bbd0-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="6bbd0-115">Yrityskuvan mukainen kirjautumiskokemus</span><span class="sxs-lookup"><span data-stu-id="6bbd0-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="6bbd0-116">Jos yrityksesi on [lisännyt yrityksesi brändiä Office 365-kirjautumissivulle](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), laitteen käyttäjä saa kyseisen kokemuksen kirjautumiseen.</span><span class="sxs-lookup"><span data-stu-id="6bbd0-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="6bbd0-117">Automaattinen MDM-rekisteröinti määritetyillä AAD-tileillä</span><span class="sxs-lookup"><span data-stu-id="6bbd0-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="6bbd0-118">Azure Active Directory hallitsee käyttäjä tietoja, ja käyttäjät kirjauduttava sisään Windowsiin ja Office 365-palveluun Microsoft 365-yrityksen tunniste tiedoilla.</span><span class="sxs-lookup"><span data-stu-id="6bbd0-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="6bbd0-119">**Valinnaiset asetukset:**</span><span class="sxs-lookup"><span data-stu-id="6bbd0-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="6bbd0-120">**Asetus**</span><span class="sxs-lookup"><span data-stu-id="6bbd0-120">**Setting**</span></span>|<span data-ttu-id="6bbd0-121">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="6bbd0-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6bbd0-122">Ohita tietosuoja-asetukset (oletusarvoisesti poissa käytöstä)</span><span class="sxs-lookup"><span data-stu-id="6bbd0-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="6bbd0-123">Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei näe laitteen ja Windowsin käyttöoikeussopimusta kirjautuessaan ensimmäisen kerran.</span><span class="sxs-lookup"><span data-stu-id="6bbd0-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="6bbd0-124">Älä salli käyttäjän ryhtyä paikalliseksi järjestelmänvalvojaksi</span><span class="sxs-lookup"><span data-stu-id="6bbd0-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="6bbd0-125">Jos täksi asetukseksi on määritetty **Käytössä**, laitteen käyttäjä ei voi asentaa henkilökohtaisia sovelluksia, kuten Cortanaa.</span><span class="sxs-lookup"><span data-stu-id="6bbd0-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
   
