---
title: Microsoft 365 for Businessin Office-asiakaskäyttöön valmistautuminen
f1.keywords:
- CSH
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
description: Lue, miten voit asentaa 32-bittiset Office-sovellukset automaattisesti Windows 10 -tietokoneisiin ja pitää ne ajan tasalla.
ms.openlocfilehash: b5f01bc9bb10765929f3c6bdd5908e8b48a51a11
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43633095"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="1a72a-103">Microsoft 365 for Businessin Office-asiakaskäyttöön valmistautuminen</span><span class="sxs-lookup"><span data-stu-id="1a72a-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="1a72a-104">Valmistaudu Office-sovellusten automaattiseen asentamiseen asiakastietokoneisiin.</span><span class="sxs-lookup"><span data-stu-id="1a72a-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="1a72a-105">Microsoft 365 for Businessin avulla voit asentaa 32-bittiset Office-sovellukset automaattisesti Windows 10 -tietokoneisiin ja pitää ne ajan tasalla päivityksistä.</span><span class="sxs-lookup"><span data-stu-id="1a72a-105">You can use Microsoft 365 for business to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="1a72a-106">Automaattinen asennus toimii parhaiten, jos käyttäjän tietokone on Windows 10 Businessissa ja</span><span class="sxs-lookup"><span data-stu-id="1a72a-106">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="1a72a-107">Ei ole olemassa olevia Office-työpöytäsovelluksia (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ja OneDrive).</span><span class="sxs-lookup"><span data-stu-id="1a72a-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="1a72a-108">tai</span><span class="sxs-lookup"><span data-stu-id="1a72a-108">or</span></span>
    
- <span data-ttu-id="1a72a-109">Tietokoneeseen on asennettu Officen pika-asennusversio.</span><span class="sxs-lookup"><span data-stu-id="1a72a-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="1a72a-110">Voit selvittää, onko käytössäsi Officen pika-asennusversio, valitsemalla missä tahansa Office-sovelluksessa **Tiedosto** \> **Tili** (Outlookissa **Office-tili**).</span><span class="sxs-lookup"><span data-stu-id="1a72a-110">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="1a72a-111">Jos **näet Office-päivitykset** seuraavassa kuvassa esitetyllä tavalla, asennus tehtiin pika-asennuksen avulla.</span><span class="sxs-lookup"><span data-stu-id="1a72a-111">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="1a72a-113">**Kuka hyötyy tämän ominaisuuden käytöstä**</span><span class="sxs-lookup"><span data-stu-id="1a72a-113">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="1a72a-114">Käyttäjä, jonka PC-tietokoneessa on seuraavat ominaisuudet:</span><span class="sxs-lookup"><span data-stu-id="1a72a-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="1a72a-115">**Hänellä** on Windows 10 Business -käyttöoikeus, aktiivinen Microsoft 365 for Business -käyttöoikeus, Windows 10 Creators -päivitys ja se on liitetty Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="1a72a-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="1a72a-116">**Ei ole** 64-bittisiä Office-sovelluksia (esimerkiksi Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="1a72a-116">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="1a72a-117">Jos tarvitaan 64-bittisiä Office-sovelluksia, tämä ominaisuus ei sovi hyvin, koska 64-bittisen 2016 Officen pika-asennusversion käynnistäminen Microsoft 365 for Business -hallintakonsolista ei tue sitä.</span><span class="sxs-lookup"><span data-stu-id="1a72a-117">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="1a72a-118">**Tietokoneessa ei ole** mitään 2016 Windows Installer (MSI) -erillissovelluksia (esimerkiksi Visiota tai Projectia).</span><span class="sxs-lookup"><span data-stu-id="1a72a-118">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="1a72a-119">Microsoft 365 for Business päivittää Officen Office 2016:n pika-asennusversioksi, eikä se toimi Office 2016 MSI:n erillissovellusten kanssa.</span><span class="sxs-lookup"><span data-stu-id="1a72a-119">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="1a72a-120">Seuraavassa taulukossa on esitetty, mitä toimia loppukäyttäjien/järjestelmänvalvojien on ehkä suoritettava aloitustilastaan riippuen, jotta Microsoft 365 for Business -hallintakonsolin Officen käyttöönotto on onnistunut 32-bittisessä pika-asennusversiossa.</span><span class="sxs-lookup"><span data-stu-id="1a72a-120">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span>
  
|<span data-ttu-id="1a72a-121">**Office-asennuksen aloittamistila**</span><span class="sxs-lookup"><span data-stu-id="1a72a-121">**Starting Office install status**</span></span>|<span data-ttu-id="1a72a-122">**Ennen Microsoft 365 for Business Officen asentamista toteutettavat toimet**</span><span class="sxs-lookup"><span data-stu-id="1a72a-122">**Action to take before Microsoft 365 for business Office install**</span></span>|<span data-ttu-id="1a72a-123">**Lopputila**</span><span class="sxs-lookup"><span data-stu-id="1a72a-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1a72a-124">Ei asennettua Office-ohjelmistopakettia</span><span class="sxs-lookup"><span data-stu-id="1a72a-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="1a72a-125">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="1a72a-125">None</span></span>  <br/> |<span data-ttu-id="1a72a-126">Office 2016:n 32-bittinen asennus pika-asennuksen avulla</span><span class="sxs-lookup"><span data-stu-id="1a72a-126">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="1a72a-127">Olemassa oleva 32-bittisen Officen (2016 tai aiempi versio) pika-asennusversio, mutta ei erillissovelluksia</span><span class="sxs-lookup"><span data-stu-id="1a72a-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="1a72a-128">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="1a72a-128">None</span></span>  <br/> |<span data-ttu-id="1a72a-129">Päivitetty uusimpaan 32-bittiseen Office 2016 -pika-asennusversioon tarpeen mukaisesti **\***</span><span class="sxs-lookup"><span data-stu-id="1a72a-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="1a72a-130">Officen nykyinen pika-asennus- ja pika-asennus32- tai 64-bittiset erilliset Office-sovellukset (esimerkiksi Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="1a72a-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="1a72a-131">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="1a72a-131">None</span></span>  <br/> |<span data-ttu-id="1a72a-132">Tämä ei vaikuta erillisiin sovelluksiin.</span><span class="sxs-lookup"><span data-stu-id="1a72a-132">Standalone apps aren't affected.</span></span> <span data-ttu-id="1a72a-133">Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon</span><span class="sxs-lookup"><span data-stu-id="1a72a-133">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="1a72a-134">Olemassa oleva 32-bittisen Officen pika-asennusversio ja mitkä tahansa 32- tai 64-bittiset (paitsi 2016) Office MSI -erillissovellukset</span><span class="sxs-lookup"><span data-stu-id="1a72a-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="1a72a-135">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="1a72a-135">None</span></span>  <br/> |<span data-ttu-id="1a72a-136">Tämä ei vaikuta erillisiin sovelluksiin.</span><span class="sxs-lookup"><span data-stu-id="1a72a-136">Standalone apps aren't affected.</span></span> <span data-ttu-id="1a72a-137">Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon</span><span class="sxs-lookup"><span data-stu-id="1a72a-137">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="1a72a-138">Mikä tahansa 64-bittisen Officen pika-asennusversio</span><span class="sxs-lookup"><span data-stu-id="1a72a-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="1a72a-139">Poista 64-bittisten Office-sovellusten asennus, jos niiden korvaaminen 32-bittisillä Office-sovelluksilla on OK</span><span class="sxs-lookup"><span data-stu-id="1a72a-139">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="1a72a-140">Jos 64-bittiset Office-sovellukset poistetaan, 32-bittinen Office 2016 -pika-asennusversio asennetaan</span><span class="sxs-lookup"><span data-stu-id="1a72a-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="1a72a-141">Olemassa oleva Office 2016:n MSI-asennus ja erillissovellukset tai ei erillissovelluksia</span><span class="sxs-lookup"><span data-stu-id="1a72a-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="1a72a-142">Poista MSI Office 2016:n asennus.</span><span class="sxs-lookup"><span data-stu-id="1a72a-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="1a72a-p106">32-bittinen Office 2016 -pika-asennusversio on asennettu. Ei muutoksia erillissovelluksiin</span><span class="sxs-lookup"><span data-stu-id="1a72a-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="1a72a-145">Olemassa oleva Office 2013:n (tai aiemman version) MSI-asennus ja/tai Office-erillissovellukset</span><span class="sxs-lookup"><span data-stu-id="1a72a-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="1a72a-146">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="1a72a-146">None</span></span>  <br/> |<span data-ttu-id="1a72a-147">32-bittinen Office 2016 -pika-asennusversio ja olemassa oleva MSI Office -asennus (ja erillissovellukset) ovat rinnakkain</span><span class="sxs-lookup"><span data-stu-id="1a72a-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="1a72a-148">**(\*) Huomautus:** Ei päivitä 32-bittiseen Office 2016 -pika-asennusversioon tunnetun ohjelmavirheen takia.</span><span class="sxs-lookup"><span data-stu-id="1a72a-148">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="1a72a-149">Korjaus on käynnissä.</span><span class="sxs-lookup"><span data-stu-id="1a72a-149">A fix is in progress.</span></span> 
  
