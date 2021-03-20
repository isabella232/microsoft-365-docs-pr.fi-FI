---
title: Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Lue, miten voit varmistaa, että Microsoft 365 for Business -sovelluksen suojausasetukset tulevat voimaan käyttäjien Windows 10 -laitteissa.
ms.openlocfilehash: ff99b3a4fce49aebdb5c72f51e46678a7821e186
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912410"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="33d8c-103">Laitteiden suojausasetusten vahvistaminen Windows 10 -tietokoneissa</span><span class="sxs-lookup"><span data-stu-id="33d8c-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="33d8c-104">Windows 10:n laitekäytäntöjen määrityksen varmistaminen</span><span class="sxs-lookup"><span data-stu-id="33d8c-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="33d8c-105">Kun olet [määrittänyt laitekäytännöt](protection-settings-for-windows-10-pcs.md), saattaa kestää muutama tunti, ennen kuin käytäntöä sovelletaan käyttäjien laitteissa.</span><span class="sxs-lookup"><span data-stu-id="33d8c-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="33d8c-106">Voit varmistaa, että käytännöt on otettu käyttöön, perehtymällä Windowsin asetusnäyttöihin käyttäjien laitteissa.</span><span class="sxs-lookup"><span data-stu-id="33d8c-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="33d8c-107">Koska käyttäjät eivät voi muokata Windows Updaten ja Windows Defenderin virustentorjunnan asetuksia Windows 10 -laitteissaan, monet vaihtoehdot näkyvät harmaina.</span><span class="sxs-lookup"><span data-stu-id="33d8c-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="33d8c-108">Siirry Asetuksiin **Päivitä** \> **&amp; suojaus** \> **Windows Updaten** \> **uudelleenkäynnistysasetuksiin** ja varmista, että kaikki asetukset näkyvät harmaina.</span><span class="sxs-lookup"><span data-stu-id="33d8c-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Kaikki uudelleenkäynnistysasetukset näkyvät harmaina.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="33d8c-110">Valitse  Asetukset \> **Päivitä &amp; suojaus** \> **Windows Updaten** \> **lisäasetukset** ja varmista, että kaikki asetukset näkyvät harmaina.</span><span class="sxs-lookup"><span data-stu-id="33d8c-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Windowsin Lisäasetukset-asetukset näkyvät harmaina.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="33d8c-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span><span class="sxs-lookup"><span data-stu-id="33d8c-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="33d8c-113">Varmista, että näet punaisella viestin siitä, että organisaatiosi on piilottanut tai hallinnoi joitakin asetuksia ja että kaikki vaihtoehdot näkyvät harmaina.</span><span class="sxs-lookup"><span data-stu-id="33d8c-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="33d8c-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span><span class="sxs-lookup"><span data-stu-id="33d8c-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="33d8c-116">Varmista, että kaikki asetukset näkyvät harmaina.</span><span class="sxs-lookup"><span data-stu-id="33d8c-116">Verify that all options are grayed out.</span></span> 
    
    ![Virusten ja uhkien torjunta-asetukset näkyvät harmaina.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="33d8c-118">Aiheeseen liittyvät aiheet</span><span class="sxs-lookup"><span data-stu-id="33d8c-118">Related Topics</span></span>

[<span data-ttu-id="33d8c-119">Microsoft 365 for Businessin dokumentaatio ja resurssit</span><span class="sxs-lookup"><span data-stu-id="33d8c-119">Microsoft 365 for business documentation and resources</span></span>](./index.yml)
  
[<span data-ttu-id="33d8c-120">Microsoft 365 for Businessin käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="33d8c-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="33d8c-121">Microsoft 365 for Businessin hallinta</span><span class="sxs-lookup"><span data-stu-id="33d8c-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="33d8c-122">Windows 10 -tietokoneiden laitemääritysten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="33d8c-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
