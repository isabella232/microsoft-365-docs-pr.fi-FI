---
title: Microsoft 365 Businessin Office-asiakkaan käyttöönottoon valmistautuminen
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Opi asentamaan 32-bittiset Office-sovellukset automaattisesti Windows 10-tieto koneisiin ja pitämään ne ajan tasalla.
ms.openlocfilehash: 09857ddeb28e953da07979045a65f6b91925aeaf
ms.sourcegitcommit: 2c2248b03f7753d64490f2f7e56ec644a235b65a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/15/2019
ms.locfileid: "38640765"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="f28c2-103">Microsoft 365 Businessin Office-asiakkaan käyttöönottoon valmistautuminen</span><span class="sxs-lookup"><span data-stu-id="f28c2-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="f28c2-104">Valmistaudu Office-sovellusten automaattiseen asentamiseen asiakastietokoneisiin.</span><span class="sxs-lookup"><span data-stu-id="f28c2-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="f28c2-105">Microsoft 365 Businessin avulla voit asentaa 32-bittiset Office-sovellukset automaattisesti Windows 10-tieto koneisiin ja pitää ne ajan tasalla päivitysten avulla.</span><span class="sxs-lookup"><span data-stu-id="f28c2-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="f28c2-106">Automaattinen asennus toimii parhaiten, jos käyttäjän tieto kone on Windows 10 Businessissa ja:</span><span class="sxs-lookup"><span data-stu-id="f28c2-106">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="f28c2-107">Ei ole olemassa olevia Office-työpöytäsovelluksia (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ja OneDrive).</span><span class="sxs-lookup"><span data-stu-id="f28c2-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="f28c2-108">tai</span><span class="sxs-lookup"><span data-stu-id="f28c2-108">or</span></span>
    
- <span data-ttu-id="f28c2-109">Tietokoneeseen on asennettu Officen pika-asennusversio.</span><span class="sxs-lookup"><span data-stu-id="f28c2-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="f28c2-110">Voit selvittää, onko käytössäsi Officen pika-asennusversio, valitsemalla missä tahansa Office-sovelluksessa **Tiedosto** \> **Tili** (Outlookissa **Office-tili**).</span><span class="sxs-lookup"><span data-stu-id="f28c2-110">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="f28c2-111">Jos näet **Office-päivitykset** seuraavassa kuvassa esitetyllä tavalla, asennus tehtiin käyttämällä click-to-Run-kohdetta.</span><span class="sxs-lookup"><span data-stu-id="f28c2-111">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="f28c2-113">**Kuka hyötyy tämän ominaisuuden**</span><span class="sxs-lookup"><span data-stu-id="f28c2-113">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="f28c2-114">Käyttäjä, jonka PC-tietokoneessa on seuraavat ominaisuudet:</span><span class="sxs-lookup"><span data-stu-id="f28c2-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="f28c2-115">**Tietokoneessa on** Windows 10 Business -käyttöoikeus, aktiivinen Microsoft 365 Business-käyttöoikeus sekä Windows 10:n Creators-päivitys ja se on liitetty Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="f28c2-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="f28c2-116">**Ei ole** 64-bittisiä Office-sovelluksia (esimerkki: Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="f28c2-116">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="f28c2-117">Jos 64-bittisiä Office-sovelluksia tarvitaan, tämä ominaisuus ei ole hyvä istuvuus, koska ei ole tukea 64-bittisen 2016-version käynnistämisestä Office-versiosta Microsoft 365 Business admin Consolesta.</span><span class="sxs-lookup"><span data-stu-id="f28c2-117">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="f28c2-118">**Tietokoneessa ei ole** mitään 2016 Windows Installer (MSI) -erillissovelluksia (esimerkiksi Visiota tai Projectia).</span><span class="sxs-lookup"><span data-stu-id="f28c2-118">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="f28c2-119">Microsoft 365 Business päivittää Office-version Office 2016-versioon ja se ei toimi Office 2016 MSI-sovellusten kanssa.</span><span class="sxs-lookup"><span data-stu-id="f28c2-119">Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="f28c2-120">Seuraavassa taulukossa on esitetty, mitä toimia loppu käyttäjien tai järjestelmänvalvojien on ehkä tehtävä alku tilan mukaan, jotta Office-käyttöönoton onnistunut 32-bittinen versio voidaan suorittaa Microsoft 365 Business admin Consolesta.</span><span class="sxs-lookup"><span data-stu-id="f28c2-120">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="f28c2-121">**Office-asennuksen aloittamistila**</span><span class="sxs-lookup"><span data-stu-id="f28c2-121">**Starting Office install status**</span></span>|<span data-ttu-id="f28c2-122">**Toimenpiteet ennen Microsoft 365 Business:n Office-asennusta**</span><span class="sxs-lookup"><span data-stu-id="f28c2-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="f28c2-123">**Lopputila**</span><span class="sxs-lookup"><span data-stu-id="f28c2-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f28c2-124">Ei asennettua Office-ohjelmistopakettia</span><span class="sxs-lookup"><span data-stu-id="f28c2-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="f28c2-125">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="f28c2-125">None</span></span>  <br/> |<span data-ttu-id="f28c2-126">Office 2016 32-bit asennetaan käyttämällä click-to-Run-</span><span class="sxs-lookup"><span data-stu-id="f28c2-126">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="f28c2-127">Olemassa oleva 32-bittisen Officen (2016 tai aiempi versio) pika-asennusversio, mutta ei erillissovelluksia</span><span class="sxs-lookup"><span data-stu-id="f28c2-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="f28c2-128">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="f28c2-128">None</span></span>  <br/> |<span data-ttu-id="f28c2-129">Päivitetty uusimpaan 32-bittiseen Office 2016 -pika-asennusversioon tarpeen mukaisesti **\***</span><span class="sxs-lookup"><span data-stu-id="f28c2-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="f28c2-130">Officen aiemmin luotu 32-bittinen versio ja napsautus suoritettavaksi 32-bittinen tai 64-bittinen itsenäinen Office-sovellus (esimerkiksi Visio, projekti)</span><span class="sxs-lookup"><span data-stu-id="f28c2-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="f28c2-131">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="f28c2-131">None</span></span>  <br/> |<span data-ttu-id="f28c2-132">Erilliset sovellukset eivät muutu.</span><span class="sxs-lookup"><span data-stu-id="f28c2-132">Standalone apps aren't affected.</span></span> <span data-ttu-id="f28c2-133">Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon</span><span class="sxs-lookup"><span data-stu-id="f28c2-133">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="f28c2-134">Olemassa oleva 32-bittisen Officen pika-asennusversio ja mitkä tahansa 32- tai 64-bittiset (paitsi 2016) Office MSI -erillissovellukset</span><span class="sxs-lookup"><span data-stu-id="f28c2-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="f28c2-135">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="f28c2-135">None</span></span>  <br/> |<span data-ttu-id="f28c2-136">Erilliset sovellukset eivät muutu.</span><span class="sxs-lookup"><span data-stu-id="f28c2-136">Standalone apps aren't affected.</span></span> <span data-ttu-id="f28c2-137">Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon</span><span class="sxs-lookup"><span data-stu-id="f28c2-137">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="f28c2-138">Mikä tahansa 64-bittisen Officen pika-asennusversio</span><span class="sxs-lookup"><span data-stu-id="f28c2-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="f28c2-139">Poista 64-bittisten Office-sovellusten asennus, jos ne on OK korvata 32-bittisellä Office-sovelluksilla</span><span class="sxs-lookup"><span data-stu-id="f28c2-139">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="f28c2-140">Jos 64-bittiset Office-sovellukset poistetaan, 32-bittinen Office 2016 -pika-asennusversio asennetaan</span><span class="sxs-lookup"><span data-stu-id="f28c2-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="f28c2-141">Olemassa oleva Office 2016:n MSI-asennus ja erillissovellukset tai ei erillissovelluksia</span><span class="sxs-lookup"><span data-stu-id="f28c2-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="f28c2-142">Poista MSI Office 2016:n asennus.</span><span class="sxs-lookup"><span data-stu-id="f28c2-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="f28c2-p106">32-bittinen Office 2016 -pika-asennusversio on asennettu. Ei muutoksia erillissovelluksiin</span><span class="sxs-lookup"><span data-stu-id="f28c2-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="f28c2-145">Olemassa oleva Office 2013:n (tai aiemman version) MSI-asennus ja/tai Office-erillissovellukset</span><span class="sxs-lookup"><span data-stu-id="f28c2-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="f28c2-146">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="f28c2-146">None</span></span>  <br/> |<span data-ttu-id="f28c2-147">32-bittinen Office 2016 -pika-asennusversio ja olemassa oleva MSI Office -asennus (ja erillissovellukset) ovat rinnakkain</span><span class="sxs-lookup"><span data-stu-id="f28c2-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="f28c2-148">**(\*) Huomautus:** Ei päivitä 32-bittiseen Office 2016 -pika-asennusversioon tunnetun ohjelmavirheen takia.</span><span class="sxs-lookup"><span data-stu-id="f28c2-148">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="f28c2-149">Korjaus on käynnissä.</span><span class="sxs-lookup"><span data-stu-id="f28c2-149">A fix is in progress.</span></span> 
  