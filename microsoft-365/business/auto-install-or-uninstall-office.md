---
title: Office asentaminen tai poistaminen automaattisesti Windows 10 -laitteissa
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: cbc6bfe5-565a-4fb8-95f0-b06e7b74ac46
description: 'Asenna tai poista Windows-10 laitteissa hallintakeskukseen 365 Microsoft Business Office. '
ms.openlocfilehash: 997c001ed1520f1ac989255632d36f9b7bedd16c
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983333"
---
# <a name="automatically-install-or-uninstall-office-on-windows-10-devices"></a><span data-ttu-id="12b6f-103">Office asentaminen tai poistaminen automaattisesti Windows 10 -laitteissa</span><span class="sxs-lookup"><span data-stu-id="12b6f-103">Automatically install or uninstall Office on Windows 10 devices</span></span>

<span data-ttu-id="12b6f-104">Voit asentaa Officen helposti ja nopeasti Windows 10 -tietokoneisiin Microsoft 365 Business -hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="12b6f-104">You can quickly and easily install Office to Windows 10 PCs from the Microsoft 365 Business admin center.</span></span>
  
<span data-ttu-id="12b6f-105">Jotta ymmärrät, miten se toimii aiemmin asennettujen Office-sovellusten kanssa, lue [Office-asiakasohjelman asennuksen valmisteleminen](prepare-for-office-client-deployment.md) ennen aloittamista.</span><span class="sxs-lookup"><span data-stu-id="12b6f-105">To understand how this works with previously installed Office apps, read [Prepare for Office client installation](prepare-for-office-client-deployment.md) before you get started.</span></span> 
  
## <a name="manage-office-deployments"></a><span data-ttu-id="12b6f-106">Officen käyttöönoton hallinta</span><span class="sxs-lookup"><span data-stu-id="12b6f-106">Manage Office deployments</span></span>

1. <span data-ttu-id="12b6f-107">Kirjaudu [hallintakeskukseen](https://aka.ms/bcsportal) yleisen järjestelmänvalvojan tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="12b6f-107">Sign in to the [admin center](https://aka.ms/bcsportal) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="12b6f-p101">Valitse **laitteet** -kortin **Hallinta Office Deployment**.    Jos **laitteen toiminnot** , kortti ei ole admin Centerin **Koti** -sivulla, valitse **Lisää** (+) lisääminen admin kotona.</span><span class="sxs-lookup"><span data-stu-id="12b6f-p101">On the **Devices** card, choose **Manage Office Deployment**.    If you do not see the **Device actions** card, in the admin center **Home** page, click **Add** (+) to add it to your admin home.</span></span>
    
    ![Screenshot of the Devices card in the admin center](media/9982e784-dbf9-4a76-a159-bb3e2e5aa23f.png)
  
3. <span data-ttu-id="12b6f-111">Valitse avautuvassa **Officen käyttöönoton hallinta** -ruudussa **Lisää ryhmä** ja sitten ryhmät, joita haluat käyttää.</span><span class="sxs-lookup"><span data-stu-id="12b6f-111">On the **Manage Office deployment** pane that opens, choose **Add a group**, then select the groups you want use.</span></span>
    
4. <span data-ttu-id="12b6f-112">Kun olet lisännyt ryhmät, joita haluat käyttää, valitse avattavasta **Käyttöönottotoiminto**-luettelosta joko **Asenna Office mahdollisimman pian** tai **Poista Officen asennus**.</span><span class="sxs-lookup"><span data-stu-id="12b6f-112">After you have added the group or groups you want to use, from the **Deployment Action** drop-down, select either **Install Office as soon as possible** or **Uninstall Office**.</span></span>
    
    ![In the Manage Office deployment pane, choose either Install Office as soon as possible, or Uninstall Office.](media/00f24a61-1848-40c0-b037-78d726c7d757.png)
  
5. <span data-ttu-id="12b6f-114">Valitse **Seuraava** \> tarkista asetukset ja valitse sitten **Vahvista**.</span><span class="sxs-lookup"><span data-stu-id="12b6f-114">Choose **Next** \> review the settings and then choose **Confirm**.</span></span>
    
<span data-ttu-id="12b6f-115">32-bittinen Office asennetaan automaattisesti käyttämiesi ryhmien määrittämien käyttäjien omistamiin laitteisiin tai asennus poistetaan niistä.</span><span class="sxs-lookup"><span data-stu-id="12b6f-115">A 32-bit Office will be automatically installed, or uninstalled in the devices owned by users specified by the group or groups you used.</span></span>
  
<span data-ttu-id="12b6f-116">Voit tarkistaa tilanteen avaamalla Tehtävienhallinnan tietokoneessa, joka valittiin Officen asennukseen, ja etsimällä Microsoft Officen pika-asennusprosessin.</span><span class="sxs-lookup"><span data-stu-id="12b6f-116">To verify you can open the Task Manager on a computer that was selected for an Office install and look for Microsoft Office Click-to-Run process.</span></span>
  


