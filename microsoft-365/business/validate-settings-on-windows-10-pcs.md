---
title: Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Opettele tarkistaa Microsoft 365 Business app suojausasetukset Windows 10-laitteet.
ms.openlocfilehash: 5ab91d65fa7bd40ebc118df217c9711b7bbfe7a4
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32286711"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="5d907-103">Laitteiden suojausasetusten vahvistaminen Windows 10 -tietokoneissa</span><span class="sxs-lookup"><span data-stu-id="5d907-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="5d907-104">Windows 10:n laitekäytäntöjen määrityksen varmistaminen</span><span class="sxs-lookup"><span data-stu-id="5d907-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="5d907-p101">Kun olet [määrittänyt laitekäytännöt](protection-settings-for-windows-10-pcs.md), saattaa kestää muutama tunti, ennen kuin käytäntöä sovelletaan käyttäjien laitteissa. Voit varmistaa, että käytännöt on otettu käyttöön, perehtymällä Windowsin asetusnäyttöihin käyttäjien laitteissa. Koska käyttäjät eivät voi muokata Windows Updaten ja Windows Defenderin virustentorjunnan asetuksia Windows 10 -laitteissa, valtaosa näistä asetuksista näkyy harmaana.</span><span class="sxs-lookup"><span data-stu-id="5d907-p101">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices. You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices. Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, a lot of those options will be greyed out.</span></span>
  
1. <span data-ttu-id="5d907-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are greyed out.</span><span class="sxs-lookup"><span data-stu-id="5d907-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are greyed out.</span></span> 
    
    ![All the Restart options are greyed out.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="5d907-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are greyed out.</span><span class="sxs-lookup"><span data-stu-id="5d907-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are greyed out.</span></span> 
    
    ![Windows Advanced updates options are all greyed out.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="5d907-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span><span class="sxs-lookup"><span data-stu-id="5d907-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="5d907-113">Varmista, että näet (punaisella) viestin siitä, että organisaatio on piilottanut osan asetuksista tai hallitsee niitä, ja että kaikki asetukset näkyvät harmaana.</span><span class="sxs-lookup"><span data-stu-id="5d907-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are greyed out.</span></span>
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="5d907-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span><span class="sxs-lookup"><span data-stu-id="5d907-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="5d907-116">Varmista, että kaikki asetukset näkyvät harmaana.</span><span class="sxs-lookup"><span data-stu-id="5d907-116">Verify that all options are greyed out.</span></span> 
    
    ![The Virus and threat protection settings are greyed out.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="5d907-118">Aiheeseen liittyvät artikkelit</span><span class="sxs-lookup"><span data-stu-id="5d907-118">Related Topics</span></span>

[<span data-ttu-id="5d907-119">Microsoft 365 Businessin ohjeet ja resurssit</span><span class="sxs-lookup"><span data-stu-id="5d907-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="5d907-120">Microsoft 365 Businessin käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="5d907-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="5d907-121">Microsoft 365 Businessin hallinta</span><span class="sxs-lookup"><span data-stu-id="5d907-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="5d907-122">Windows 10 -tietokoneiden laitemääritysten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="5d907-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

