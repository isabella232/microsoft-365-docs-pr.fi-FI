---
title: Työtiedostojen suojaaminen mobiililaitteiden katoamisen tai varastamisen varalta
ms.author: sirkkuw
author: sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4StolenDevice
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c12164c7-6190-4294-b88a-590580c9869a
description: Lisätietoja asetuksia suojaamaan työ-tiedostoja, jos käyttäjän laite katoaa tai varastetaan.
ms.openlocfilehash: 1256f54b2ff626ea7b85d91020e355c8b611a8c0
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32285346"
---
# <a name="protect-work-files-when-a-mobile-device-is-lost-or-stolen"></a><span data-ttu-id="57c29-103">Työtiedostojen suojaaminen mobiililaitteiden katoamisen tai varastamisen varalta</span><span class="sxs-lookup"><span data-stu-id="57c29-103">Protect work files when a mobile device is lost or stolen</span></span>

<span data-ttu-id="57c29-p101">Käytäntöasetukset määrittävät, mitä tapahtuu automaattisesti kadonneen tai varastetun laitteen suojaamiseksi. On suositeltavaa hyväksyä oletusarvot asennuksen aikana kaikkia käyttäjiä koskevien sovelluskäytäntöjen luomiseksi Androidille, iOS:lle ja Windows 10:lle. Voit luoda lisää käytäntöjä asennuksen päätyttyä.</span><span class="sxs-lookup"><span data-stu-id="57c29-p101">The policy settings determine what happens automatically to protect a device that is lost or stolen. We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users. You can create more policies after setup completes.</span></span>
  
## <a name="settings-that-protect-work-files"></a><span data-ttu-id="57c29-107">Työtiedostojen suojaamisasetukset</span><span class="sxs-lookup"><span data-stu-id="57c29-107">Settings that protect work files</span></span>

<span data-ttu-id="57c29-108">Seuraavilla asetuksilla voidaan suojata työtiedostoja, jos käyttäjän laite katoaa tai varastetaan:</span><span class="sxs-lookup"><span data-stu-id="57c29-108">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="57c29-109">Asetus</span><span class="sxs-lookup"><span data-stu-id="57c29-109">Setting</span></span>  <br/> |<span data-ttu-id="57c29-110">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="57c29-110">Description</span></span>  <br/> |
|<span data-ttu-id="57c29-111">Poista työtiedostot passiivisesta laitteesta näin monen päivän kuluttua</span><span class="sxs-lookup"><span data-stu-id="57c29-111">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="57c29-112">Jos laitetta ei käytetä niin moneen päivään kuin tässä määrität, laitteeseen tallennetut työtiedostot poistetaan automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="57c29-112">If a device is not used for the number of days that you specify here, any work files stored on the device will automatically be deleted.</span></span>  <br/> |
|<span data-ttu-id="57c29-113">Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin</span><span class="sxs-lookup"><span data-stu-id="57c29-113">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="57c29-114">Jos tämä asetus on **käytössä**, ainoa käytettävissä oleva työtiedostojen tallennuspaikka on OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="57c29-114">If this setting is **On**, the only available save location for work files will be OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="57c29-115">Salaa työtiedostot</span><span class="sxs-lookup"><span data-stu-id="57c29-115">Encrypt work files</span></span>  <br/> |<span data-ttu-id="57c29-p102">Pidä tämä asetus **käytössä**, jotta työtiedostot suojataan salauksella. Vaikka laite katoaa tai varastetaan, kukaan voi lukea yritystietojasi.  </span><span class="sxs-lookup"><span data-stu-id="57c29-p102">Keep this setting **On** so that work files are protected by encryption. Even if the device is lost or stolen, no one will be able to read your company data.  </span></span><br/> |
   

