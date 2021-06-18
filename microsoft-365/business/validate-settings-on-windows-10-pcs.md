---
title: Sovellusten suojausasetusten vahvistaminen Windows 10 tietokoneissa
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Lue, miten voit varmistaa Microsoft 365 että yrityssovellusten suojausasetukset tulevat voimaan käyttäjien Windows 10 laitteissa.
ms.openlocfilehash: 464a246a0da65dcffeb70946287ce4fa0e67ae7c
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925255"
---
# <a name="validate-device-protection-settings-for-windows-10-pcs"></a><span data-ttu-id="9f5fa-103">Vahvista laitteiden suojausasetukset Windows 10 tietokoneissa</span><span class="sxs-lookup"><span data-stu-id="9f5fa-103">Validate device protection settings for Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="9f5fa-104">Windows 10:n laitekäytäntöjen määrityksen varmistaminen</span><span class="sxs-lookup"><span data-stu-id="9f5fa-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="9f5fa-105">Kun olet [määrittänyt laitekäytännöt](protection-settings-for-windows-10-pcs.md), saattaa kestää muutama tunti, ennen kuin käytäntöä sovelletaan käyttäjien laitteissa.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="9f5fa-106">Voit varmistaa, että käytännöt on otettu käyttöön, perehtymällä Windowsin asetusnäyttöihin käyttäjien laitteissa.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="9f5fa-107">Koska käyttäjät eivät voi muokata päivitys- ja Windows-Windows Defenderin virustentorjunta asetuksia Windows 10, monet asetukset näkyvät harmaina.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="9f5fa-108">Siirry kohtaan **Asetukset** Päivitä \> **&amp; Windows** uudelleenkäynnistysasetukset ja \>  \>  varmista, että kaikki asetukset näkyvät harmaina.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Kaikki Uudelleenkäynnistysasetukset näkyvät harmaina.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="9f5fa-110">Siirry **Asetukset** \> **päivitä suojaus &amp; -Windows** \> **ja** \>  varmista, että kaikki asetukset näkyvät harmaina.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Windows Kaikki lisäpäivitykset näkyvät harmaina.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="9f5fa-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="9f5fa-113">Varmista, että näet punaisella viestin siitä, että organisaatiosi on piilottanut tai hallinnoi joitakin asetuksia ja että kaikki asetukset näkyvät harmaina.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="9f5fa-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="9f5fa-116">Varmista, että kaikki asetukset näkyvät harmaina.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-116">Verify that all options are grayed out.</span></span> 
    
    ![Virusten ja uhkien uhkientorjunta-asetukset näkyvät harmaina.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="9f5fa-118">Aiheeseen liittyvät aiheet</span><span class="sxs-lookup"><span data-stu-id="9f5fa-118">Related Topics</span></span>

[<span data-ttu-id="9f5fa-119">Microsoft 365 for Businessin ohjeista ja resursseista</span><span class="sxs-lookup"><span data-stu-id="9f5fa-119">Microsoft 365 for business documentation and resources</span></span>](./index.yml)
  
[<span data-ttu-id="9f5fa-120">Microsoft 365 käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="9f5fa-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="9f5fa-121">Yrityksen Microsoft 365 hallinta</span><span class="sxs-lookup"><span data-stu-id="9f5fa-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="9f5fa-122">Windows 10 -tietokoneiden laitemääritysten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="9f5fa-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
