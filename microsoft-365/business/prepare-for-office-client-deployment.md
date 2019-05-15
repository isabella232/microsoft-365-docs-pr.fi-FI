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
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Opettele asentaa 32-bittisen Office-sovellukset Windows (10) tietokonetta ja pitää ne ajan tasalla automaattisesti.
ms.openlocfilehash: 20269c493b0e3b5a7deb56a24a5e1a9583ef9d0a
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074646"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="97ecc-103">Microsoft 365 Businessin Office-asiakkaan käyttöönottoon valmistautuminen</span><span class="sxs-lookup"><span data-stu-id="97ecc-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="97ecc-104">Valmistaudu Office-sovellusten automaattiseen asentamiseen asiakastietokoneisiin.</span><span class="sxs-lookup"><span data-stu-id="97ecc-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="97ecc-105">Voit Microsoft 365 Business:n avulla asentaa 32-bittiset Office-sovellukset Windows 10 -tietokoneisiin automaattisesti ja pitää ne ajan tasalla päivityksillä.</span><span class="sxs-lookup"><span data-stu-id="97ecc-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps to Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="97ecc-106">Tämä toimii parhaiten, jos käyttäjän tietokoneessa on Windows 10 Business ja seuraavat ominaisuudet:</span><span class="sxs-lookup"><span data-stu-id="97ecc-106">This works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="97ecc-107">Ei ole olemassa olevia Office-työpöytäsovelluksia (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ja OneDrive).</span><span class="sxs-lookup"><span data-stu-id="97ecc-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="97ecc-108">tai</span><span class="sxs-lookup"><span data-stu-id="97ecc-108">or</span></span>
    
- <span data-ttu-id="97ecc-109">Tietokoneeseen on asennettu Officen pika-asennusversio.</span><span class="sxs-lookup"><span data-stu-id="97ecc-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="97ecc-p101">Voit selvittää, onko käytössäsi Officen pika-asennusversio, valitsemalla missä tahansa Office-sovelluksessa **Tiedosto** \> **Tili** (Outlookissa **Office-tili**). Jos näkyviin tulevat seuraavassa kuvassa esitetyt Office-päivitykset, asennus on tehty pika-asennuksena.</span><span class="sxs-lookup"><span data-stu-id="97ecc-p101">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook). If you see Office Updates as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="97ecc-113">**Kuka hyötyy tästä ominaisuudesta**</span><span class="sxs-lookup"><span data-stu-id="97ecc-113">**Who will benefit from having this feature**</span></span>
  
<span data-ttu-id="97ecc-114">Käyttäjä, jonka PC-tietokoneessa on seuraavat ominaisuudet:</span><span class="sxs-lookup"><span data-stu-id="97ecc-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="97ecc-115">**Tietokoneessa on** Windows 10 Business -käyttöoikeus, aktiivinen Microsoft 365 Business-käyttöoikeus sekä Windows 10:n Creators-päivitys ja se on liitetty Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="97ecc-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="97ecc-p102">**Tietokoneessa ei ole** 64-bittisiä Office-sovelluksia (esimerkki: Word, Excel, Powerpoint). Jos 64-bittiset Office-sovellukset tarvitaan, tämä toiminto ei ole sopiva, koska Microsoft 365 Business-hallintakonsolissa ei ole tukea 64-bittisen Office 2016 -pika-asennusversion käynnistämiseen.</span><span class="sxs-lookup"><span data-stu-id="97ecc-p102">**Doesn't have** 64-bit Office apps (example: Word, Excel, Powerpoint). If 64-bit Office apps are required, then this feature is not a good fit because there is no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="97ecc-p103">**Tietokoneessa ei ole** mitään 2016 Windows Installer (MSI) -erillissovelluksia (esimerkiksi Visiota tai Projectia). Microsoft 365 Business päivittää Officen Office 2016 -pika-asennusversioksi, eikä se toimi Office 2016 -erillissovellusten kanssa.</span><span class="sxs-lookup"><span data-stu-id="97ecc-p103">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project). Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="97ecc-120">Seuraavassa taulukossa kerrotaan, mitä toimenpiteitä käyttäjien tai järjestelmänvalvojien on ehkä alkutilan mukaan tehtävä, jotta Officen 32-bittisen pika-asennusversion käyttöönotto Microsoft 365 Business-hallintakonsolista onnistuu.</span><span class="sxs-lookup"><span data-stu-id="97ecc-120">The following table details what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="97ecc-121">**Office-asennuksen aloittamistila**</span><span class="sxs-lookup"><span data-stu-id="97ecc-121">**Starting Office install status**</span></span>|<span data-ttu-id="97ecc-122">**Toimenpiteet ennen Microsoft 365 Business:n Office-asennusta**</span><span class="sxs-lookup"><span data-stu-id="97ecc-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="97ecc-123">**Lopputila**</span><span class="sxs-lookup"><span data-stu-id="97ecc-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="97ecc-124">Ei asennettua Office-ohjelmistopakettia</span><span class="sxs-lookup"><span data-stu-id="97ecc-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="97ecc-125">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="97ecc-125">None</span></span>  <br/> |<span data-ttu-id="97ecc-126">32-bittinen Office 2016 asennettu pika-asennuksena</span><span class="sxs-lookup"><span data-stu-id="97ecc-126">Office 2016 32-bit is installed by using click-to-run</span></span>  <br/> |
|<span data-ttu-id="97ecc-127">Olemassa oleva 32-bittisen Officen (2016 tai aiempi versio) pika-asennusversio, mutta ei erillissovelluksia</span><span class="sxs-lookup"><span data-stu-id="97ecc-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="97ecc-128">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="97ecc-128">None</span></span>  <br/> |<span data-ttu-id="97ecc-129">Päivitetty uusimpaan 32-bittiseen Office 2016 -pika-asennusversioon tarpeen mukaisesti **\***</span><span class="sxs-lookup"><span data-stu-id="97ecc-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="97ecc-130">Olemassa oleva 32-bittisen Officen pika-asennusversio ja 32- tai 64-bittisten Office-erillissovellusten (kuten Vision tai Projectin) pika-asennusversiot</span><span class="sxs-lookup"><span data-stu-id="97ecc-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32- or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="97ecc-131">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="97ecc-131">None</span></span>  <br/> |<span data-ttu-id="97ecc-p104">Ei vaikutusta erillissovelluksiin. Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon</span><span class="sxs-lookup"><span data-stu-id="97ecc-p104">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="97ecc-134">Olemassa oleva 32-bittisen Officen pika-asennusversio ja mitkä tahansa 32- tai 64-bittiset (paitsi 2016) Office MSI -erillissovellukset</span><span class="sxs-lookup"><span data-stu-id="97ecc-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="97ecc-135">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="97ecc-135">None</span></span>  <br/> |<span data-ttu-id="97ecc-p105">Ei vaikutusta erillissovelluksiin. Ohjelmistopaketti on päivitetty 32-bittiseen Office 2016 -pika-asennusversioon</span><span class="sxs-lookup"><span data-stu-id="97ecc-p105">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="97ecc-138">Mikä tahansa 64-bittisen Officen pika-asennusversio</span><span class="sxs-lookup"><span data-stu-id="97ecc-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="97ecc-139">Poista 64-bittisten Office-sovellusten asennus, jos ne voidaan korvata 32-bittisillä Office-sovelluksilla</span><span class="sxs-lookup"><span data-stu-id="97ecc-139">Uninstall the 64-bit Office apps, if it is OK to replace it with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="97ecc-140">Jos 64-bittiset Office-sovellukset poistetaan, 32-bittinen Office 2016 -pika-asennusversio asennetaan</span><span class="sxs-lookup"><span data-stu-id="97ecc-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="97ecc-141">Olemassa oleva Office 2016:n MSI-asennus ja erillissovellukset tai ei erillissovelluksia</span><span class="sxs-lookup"><span data-stu-id="97ecc-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="97ecc-142">Poista MSI Office 2016:n asennus.</span><span class="sxs-lookup"><span data-stu-id="97ecc-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="97ecc-p106">32-bittinen Office 2016 -pika-asennusversio on asennettu. Ei muutoksia erillissovelluksiin</span><span class="sxs-lookup"><span data-stu-id="97ecc-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="97ecc-145">Olemassa oleva Office 2013:n (tai aiemman version) MSI-asennus ja/tai Office-erillissovellukset</span><span class="sxs-lookup"><span data-stu-id="97ecc-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="97ecc-146">Ei mitään</span><span class="sxs-lookup"><span data-stu-id="97ecc-146">None</span></span>  <br/> |<span data-ttu-id="97ecc-147">32-bittinen Office 2016 -pika-asennusversio ja olemassa oleva MSI Office -asennus (ja erillissovellukset) ovat rinnakkain</span><span class="sxs-lookup"><span data-stu-id="97ecc-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="97ecc-p107">**(\*) Huomautus:** Ei päivitä 32-bittiseen Office 2016 -pika-asennusversioon tunnetun ohjelmavirheen takia. Korjausta valmistellaan.</span><span class="sxs-lookup"><span data-stu-id="97ecc-p107">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug. Fix is in progress.</span></span> 
  


