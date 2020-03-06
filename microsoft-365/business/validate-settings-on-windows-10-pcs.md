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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Lue, miten voit varmistaa, että Microsoft 365 Business -sovellusten suojausasetukset vaikuttavat käyttäjien Windows 10 -laitteisiin.
ms.openlocfilehash: 1b661b41a8042e81f653463cbd32fc6bf6428b53
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/06/2020
ms.locfileid: "42549953"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="cfd16-103">Laitteiden suojausasetusten vahvistaminen Windows 10 -tietokoneissa</span><span class="sxs-lookup"><span data-stu-id="cfd16-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="cfd16-104">Windows 10:n laitekäytäntöjen määrityksen varmistaminen</span><span class="sxs-lookup"><span data-stu-id="cfd16-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="cfd16-105">Kun olet [määrittänyt laitekäytännöt](protection-settings-for-windows-10-pcs.md), saattaa kestää muutama tunti, ennen kuin käytäntöä sovelletaan käyttäjien laitteissa.</span><span class="sxs-lookup"><span data-stu-id="cfd16-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="cfd16-106">Voit varmistaa, että käytännöt on otettu käyttöön, perehtymällä Windowsin asetusnäyttöihin käyttäjien laitteissa.</span><span class="sxs-lookup"><span data-stu-id="cfd16-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="cfd16-107">Koska käyttäjät eivät voi muokata Windows Updaten ja Windows Defenderin virustentorjunta-asetuksia Windows 10 -laitteissaan, monet asetukset näkyvät harmaina.</span><span class="sxs-lookup"><span data-stu-id="cfd16-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="cfd16-108">Siirry **Kohtaan Asetukset** \> **Päivitys &amp; -suojaus** \> **Windows UpdateN** \> **uudelleenkäynnistysasetukset** ja varmista, että kaikki asetukset näkyvät harmaina.</span><span class="sxs-lookup"><span data-stu-id="cfd16-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Kaikki uudelleenkäynnistysasetukset näkyvät harmaina.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="cfd16-110">Siirry **kohtaan Settings** \> **Update &amp; -suojaus** \> **Windows UpdateN** \> **lisäasetukset** ja varmista, että kaikki asetukset näkyvät harmaina.</span><span class="sxs-lookup"><span data-stu-id="cfd16-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Windowsin päivitysten lisäasetukset näkyvät harmaina.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="cfd16-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span><span class="sxs-lookup"><span data-stu-id="cfd16-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="cfd16-113">Varmista, että näet viestin (punaisena), että organisaatiosi on piilottanut tai hallinnut joitakin asetuksia ja että kaikki asetukset näkyvät harmaina.</span><span class="sxs-lookup"><span data-stu-id="cfd16-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="cfd16-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span><span class="sxs-lookup"><span data-stu-id="cfd16-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="cfd16-116">Varmista, että kaikki asetukset näkyvät harmaina.</span><span class="sxs-lookup"><span data-stu-id="cfd16-116">Verify that all options are grayed out.</span></span> 
    
    ![Virusten ja uhkien torjunta-asetukset näkyvät harmaina.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="cfd16-118">Aiheeseen liittyviä aiheita</span><span class="sxs-lookup"><span data-stu-id="cfd16-118">Related Topics</span></span>

[<span data-ttu-id="cfd16-119">Microsoft 365 Businessin ohjeet ja resurssit</span><span class="sxs-lookup"><span data-stu-id="cfd16-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="cfd16-120">Microsoft 365 Businessin käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="cfd16-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="cfd16-121">Microsoft 365 Businessin hallinta</span><span class="sxs-lookup"><span data-stu-id="cfd16-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="cfd16-122">Windows 10 -tietokoneiden laitemääritysten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="cfd16-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

