---
title: Työtiedostojen suojaaminen mobiililaitteiden katoamisen tai varastamisen varalta
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c12164c7-6190-4294-b88a-590580c9869a
description: Lue tietoja Microsoft 365 Businessin asetuksista työtiedostojen suojaamiseksi, jos käyttäjän laite katoaa tai varastetaan.
ms.openlocfilehash: 4371acd53da902aa4dea93e7b8bd087d1cf27100
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561646"
---
# <a name="protect-work-files-when-a-mobile-device-is-lost-or-stolen"></a><span data-ttu-id="3b4c8-103">Työtiedostojen suojaaminen mobiililaitteiden katoamisen tai varastamisen varalta</span><span class="sxs-lookup"><span data-stu-id="3b4c8-103">Protect work files when a mobile device is lost or stolen</span></span>

<span data-ttu-id="3b4c8-104">Käytäntöasetukset määrittävät, mitä tapahtuu automaattisesti kadonneen tai varastetun laitteen suojaamiseksi.</span><span class="sxs-lookup"><span data-stu-id="3b4c8-104">The policy settings determine what happens automatically to protect a device that is lost or stolen.</span></span> <span data-ttu-id="3b4c8-105">Suosittelemme, että hyväksyt oletusarvot asennuksen aikana ja luot sovelluskäytäntöjä Androidille, iOS:lle ja Windows 10:lle, jotka koskevat kaikkia käyttäjiä.</span><span class="sxs-lookup"><span data-stu-id="3b4c8-105">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="3b4c8-106">Voit luoda lisää käytäntöjä asennuksen päätyttyä.</span><span class="sxs-lookup"><span data-stu-id="3b4c8-106">You can create more policies after setup completes.</span></span>
  
## <a name="settings-that-protect-work-files"></a><span data-ttu-id="3b4c8-107">Työtiedostojen suojaamisasetukset</span><span class="sxs-lookup"><span data-stu-id="3b4c8-107">Settings that protect work files</span></span>

<span data-ttu-id="3b4c8-108">Seuraavilla asetuksilla voidaan suojata työtiedostoja, jos käyttäjän laite katoaa tai varastetaan:</span><span class="sxs-lookup"><span data-stu-id="3b4c8-108">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="3b4c8-109">Asetus</span><span class="sxs-lookup"><span data-stu-id="3b4c8-109">Setting</span></span>  <br/> |<span data-ttu-id="3b4c8-110">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="3b4c8-110">Description</span></span>  <br/> |
|<span data-ttu-id="3b4c8-111">Poista työtiedostot passiivisesta laitteesta näin monen päivän kuluttua</span><span class="sxs-lookup"><span data-stu-id="3b4c8-111">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="3b4c8-112">Jos laitetta ei käytetä tässä määritettyjen päivien lukumäärään, laitteeseen tallennetut työtiedostot poistetaan automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="3b4c8-112">If a device isn't used for the number of days that you specify here, any work files stored on the device are automatically deleted.</span></span>  <br/> |
|<span data-ttu-id="3b4c8-113">Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin</span><span class="sxs-lookup"><span data-stu-id="3b4c8-113">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="3b4c8-114">Jos tämä asetus on **Käytössä**, työtiedostojen ainoa käytettävissä oleva tallennussijainti on OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="3b4c8-114">If this setting is **On**, the only available save location for work files is OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="3b4c8-115">Salaa työtiedostot</span><span class="sxs-lookup"><span data-stu-id="3b4c8-115">Encrypt work files</span></span>  <br/> |<span data-ttu-id="3b4c8-116">Pidä tämä asetus **käytössä**, jotta työtiedostot suojataan salauksella.</span><span class="sxs-lookup"><span data-stu-id="3b4c8-116">Keep this setting **On** so that work files are protected by encryption.</span></span> <span data-ttu-id="3b4c8-117">Vaikka laite katoaa tai varastettaisiin, kukaan ei voi lukea yrityksen tietoja.</span><span class="sxs-lookup"><span data-stu-id="3b4c8-117">Even if the device is lost or stolen, no one can read your company data.</span></span>  <br/> |
   

