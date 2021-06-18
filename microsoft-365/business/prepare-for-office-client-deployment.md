---
title: Microsoft 365 for Businessin Office-asiakasohjelman käyttöönottoon valmistautuminen
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Opi asentamaan 32-bittiset Office-sovellukset automaattisesti Windows 10 -tietokoneisiin ja pitämään ne ajan tasalla.
ms.openlocfilehash: 843be426d817da1173769b3b66dc4c054179f0fd
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/14/2021
ms.locfileid: "52924223"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="5a916-103">Microsoft 365 for Businessin Office-asiakasohjelman käyttöönottoon valmistautuminen</span><span class="sxs-lookup"><span data-stu-id="5a916-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

<span data-ttu-id="5a916-104">Tämä artikkeli koskee Microsoft 365 Business Premiumia.</span><span class="sxs-lookup"><span data-stu-id="5a916-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="5a916-105">Valmistaudu Office-sovellusten automaattiseen asentamiseen asiakastietokoneisiin.</span><span class="sxs-lookup"><span data-stu-id="5a916-105">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="5a916-106">Microsoft 365 Business Premiumin avulla voit asentaa 32-bittiset Office-sovellukset automaattisesti Windows 10 -tietokoneisiin ja pitää ne ajan tasalla päivityksistä.</span><span class="sxs-lookup"><span data-stu-id="5a916-106">You can use Microsoft 365 Business Premium to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="5a916-107">Automaattinen asennus toimii parhaiten, jos loppukäyttäjän tietokone on Windows 10 Businessissa ja:</span><span class="sxs-lookup"><span data-stu-id="5a916-107">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="5a916-108">Ei ole olemassa olevia Office-työpöytäsovelluksia (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ja OneDrive).</span><span class="sxs-lookup"><span data-stu-id="5a916-108">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="5a916-109">tai</span><span class="sxs-lookup"><span data-stu-id="5a916-109">or</span></span>
    
- <span data-ttu-id="5a916-110">Tietokoneeseen on asennettu Officen pika-asennusversio.</span><span class="sxs-lookup"><span data-stu-id="5a916-110">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="5a916-111">Voit selvittää, onko käytössäsi Officen pika-asennusversio, valitsemalla missä tahansa Office-sovelluksessa **Tiedosto** \> **Tili** (Outlookissa **Office-tili**).</span><span class="sxs-lookup"><span data-stu-id="5a916-111">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="5a916-112">Jos **näet Office-päivitykset** seuraavassa kuvassa esitetyllä tavalla, asennus on tehty käyttämällä office-asennusta.</span><span class="sxs-lookup"><span data-stu-id="5a916-112">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="5a916-114">**Kuka hyötyy tästä ominaisuudesta**</span><span class="sxs-lookup"><span data-stu-id="5a916-114">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="5a916-115">Käyttäjä, jonka PC-tietokoneessa on seuraavat ominaisuudet:</span><span class="sxs-lookup"><span data-stu-id="5a916-115">The end user whose PC:</span></span>
  
- <span data-ttu-id="5a916-116">**Sinulla**  on Windows 10 Business -käyttöoikeus, aktiivinen Microsoft 365 for Business -käyttöoikeus, Windows 10 Creators -päivitys, ja se on liitetty Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="5a916-116">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="5a916-117">**Siinä ei ole** 64-bittisiä Office-sovelluksia (esimerkki: Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="5a916-117">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="5a916-118">Jos tarvitaan 64-bittisiä Office-sovelluksia, tämä toiminto ei sovi hyvin, koska Microsoft 365 for Business -hallintakonsolista ei ole tukea Officen 64-bittisen 2016-version käynnistämiseen.</span><span class="sxs-lookup"><span data-stu-id="5a916-118">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="5a916-119">**Tietokoneessa ei ole** mitään 2016 Windows Installer (MSI) -erillissovelluksia (esimerkiksi Visiota tai Projectia).</span><span class="sxs-lookup"><span data-stu-id="5a916-119">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="5a916-120">Microsoft 365 for Business päivittää Officen Officen Office 2016:n asennusversioksi, eikä se toimi Office 2016 MSI -erillissovellusten kanssa.</span><span class="sxs-lookup"><span data-stu-id="5a916-120">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="5a916-121">Seuraavassa taulukossa on esitetty, mitä toimenpiteitä loppukäyttäjien tai järjestelmänvalvojien on ehkä suoritettava, jotta Officen 32-bittisen 32-bittisen click-to-run-version käyttöönotto onnistuu Microsoft 365 for Business -hallintakonsolista riippuen.</span><span class="sxs-lookup"><span data-stu-id="5a916-121">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span><br/>


|<span data-ttu-id="5a916-122">Office-asennuksen aloittamistila</span><span class="sxs-lookup"><span data-stu-id="5a916-122">Starting Office install status</span></span>|<span data-ttu-id="5a916-123">Toimet, jotka on otettava ennen Microsoft 365 for Businessin Officen asentamista</span><span class="sxs-lookup"><span data-stu-id="5a916-123">Action to take before Microsoft 365 for business Office install</span></span>|<span data-ttu-id="5a916-124">Lopputila</span><span class="sxs-lookup"><span data-stu-id="5a916-124">End state</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5a916-125">Ei asennettua Office-ohjelmistopakettia</span><span class="sxs-lookup"><span data-stu-id="5a916-125">No Office suite installed</span></span>  <br/> |<span data-ttu-id="5a916-126">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="5a916-126">None</span></span>  <br/> |<span data-ttu-id="5a916-127">Office 2016:n 32-bittinen versio asennetaan office-asennuksena</span><span class="sxs-lookup"><span data-stu-id="5a916-127">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="5a916-128">Olemassa oleva 32-bittisen Officen (2016 tai aiempi versio) pika-asennusversio, mutta ei erillissovelluksia</span><span class="sxs-lookup"><span data-stu-id="5a916-128">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="5a916-129">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="5a916-129">None</span></span>  <br/> |<span data-ttu-id="5a916-130">Päivitetty uusimpaan 32-bittiseen Office 2016 -pika-asennusversioon tarpeen mukaisesti **\***</span><span class="sxs-lookup"><span data-stu-id="5a916-130">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="5a916-131">Olemassa oleva 32-bittisen Officen 32-bittinen ja 32-bittisen tai 64-bittisen erillisversion Office-sovellus (esimerkiksi Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="5a916-131">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="5a916-132">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="5a916-132">None</span></span>  <br/> |<span data-ttu-id="5a916-133">Tämä ei vaikuta erillissovelluksiin.</span><span class="sxs-lookup"><span data-stu-id="5a916-133">Standalone apps aren't affected.</span></span> <span data-ttu-id="5a916-134">Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon</span><span class="sxs-lookup"><span data-stu-id="5a916-134">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="5a916-135">Olemassa oleva 32-bittisen Officen pika-asennusversio ja mitkä tahansa 32- tai 64-bittiset (paitsi 2016) Office MSI -erillissovellukset</span><span class="sxs-lookup"><span data-stu-id="5a916-135">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="5a916-136">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="5a916-136">None</span></span>  <br/> |<span data-ttu-id="5a916-137">Tämä ei vaikuta erillissovelluksiin.</span><span class="sxs-lookup"><span data-stu-id="5a916-137">Standalone apps aren't affected.</span></span> <span data-ttu-id="5a916-138">Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon</span><span class="sxs-lookup"><span data-stu-id="5a916-138">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="5a916-139">Mikä tahansa 64-bittisen Officen pika-asennusversio</span><span class="sxs-lookup"><span data-stu-id="5a916-139">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="5a916-140">Poista 64-bittiset Office-sovellukset, jos niiden korvaaminen 32-bittisllä Office-sovelluksilla on ok</span><span class="sxs-lookup"><span data-stu-id="5a916-140">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="5a916-141">Jos 64-bittiset Office-sovellukset poistetaan, 32-bittinen Office 2016 -pika-asennusversio asennetaan</span><span class="sxs-lookup"><span data-stu-id="5a916-141">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="5a916-142">Olemassa oleva Office 2016:n MSI-asennus ja erillissovellukset tai ei erillissovelluksia</span><span class="sxs-lookup"><span data-stu-id="5a916-142">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="5a916-143">Poista MSI Office 2016:n asennus.</span><span class="sxs-lookup"><span data-stu-id="5a916-143">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="5a916-p106">32-bittinen Office 2016 -pika-asennusversio on asennettu. Ei muutoksia erillissovelluksiin</span><span class="sxs-lookup"><span data-stu-id="5a916-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="5a916-146">Olemassa oleva Office 2013:n (tai aiemman version) MSI-asennus ja/tai Office-erillissovellukset</span><span class="sxs-lookup"><span data-stu-id="5a916-146">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="5a916-147">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="5a916-147">None</span></span>  <br/> |<span data-ttu-id="5a916-148">32-bittinen Office 2016 -pika-asennusversio ja olemassa oleva MSI Office -asennus (ja erillissovellukset) ovat rinnakkain</span><span class="sxs-lookup"><span data-stu-id="5a916-148">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="5a916-149">**(\*) Huomautus:** Ei päivitä 32-bittiseen Office 2016 -pika-asennusversioon tunnetun ohjelmavirheen takia.</span><span class="sxs-lookup"><span data-stu-id="5a916-149">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="5a916-150">Korjaus on käynnissä.</span><span class="sxs-lookup"><span data-stu-id="5a916-150">A fix is in progress.</span></span> 
  
