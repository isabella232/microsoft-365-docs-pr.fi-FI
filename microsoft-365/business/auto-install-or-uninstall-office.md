---
title: Office asentaminen tai poistaminen automaattisesti Windows 10 -laitteissa
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
ms.openlocfilehash: 94e5761b516c150caa11048be73d97f468b09fb5
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660560"
---
# <a name="automatically-install-or-uninstall-office-on-windows-10-devices"></a><span data-ttu-id="afc32-103">Office asentaminen tai poistaminen automaattisesti Windows 10 -laitteissa</span><span class="sxs-lookup"><span data-stu-id="afc32-103">Automatically install or uninstall Office on Windows 10 devices</span></span>

![Nauha, joka osoittaa https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="afc32-105">Voit asentaa Officen helposti ja nopeasti Windows 10 -tietokoneisiin Microsoft 365 Business -hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="afc32-105">You can quickly and easily install Office to Windows 10 PCs from the Microsoft 365 Business admin center.</span></span>
  
<span data-ttu-id="afc32-106">Jotta ymmärrät, miten se toimii aiemmin asennettujen Office-sovellusten kanssa, lue [Office-asiakasohjelman asennuksen valmisteleminen](prepare-for-office-client-deployment.md) ennen aloittamista.</span><span class="sxs-lookup"><span data-stu-id="afc32-106">To understand how this works with previously installed Office apps, read [Prepare for Office client installation](prepare-for-office-client-deployment.md) before you get started.</span></span> 
  
## <a name="manage-office-deployments"></a><span data-ttu-id="afc32-107">Officen käyttöönoton hallinta</span><span class="sxs-lookup"><span data-stu-id="afc32-107">Manage Office deployments</span></span>

1. <span data-ttu-id="afc32-108">Kirjaudu [hallintakeskukseen](https://aka.ms/bcsportal) yleisen järjestelmänvalvojan tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="afc32-108">Sign in to the [admin center](https://aka.ms/bcsportal) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="afc32-109">Valitse **Laitteet**-kortissa **Officen käyttöönoton hallinta**.</span><span class="sxs-lookup"><span data-stu-id="afc32-109">On the **Devices** card, choose **Manage Office Deployment**.</span></span>
      <span data-ttu-id="afc32-110">Jos **laitteen toiminnot** , kortti ei ole admin Centerin **Koti** -sivulla, valitse **Lisää** (+) lisääminen admin kotona.</span><span class="sxs-lookup"><span data-stu-id="afc32-110">If you do not see the **Device actions** card, in the admin center **Home** page, click **Add** (+) to add it to your admin home.</span></span>
    
    ![Screenshot of the Devices card in the admin center](media/9982e784-dbf9-4a76-a159-bb3e2e5aa23f.png)
  
3. <span data-ttu-id="afc32-112">Valitse avautuvassa **Officen käyttöönoton hallinta** -ruudussa **Lisää ryhmä** ja sitten ryhmät, joita haluat käyttää.</span><span class="sxs-lookup"><span data-stu-id="afc32-112">On the **Manage Office deployment** pane that opens, choose **Add a group**, then select the groups you want use.</span></span>
    
4. <span data-ttu-id="afc32-113">Kun olet lisännyt ryhmät, joita haluat käyttää, valitse avattavasta **Käyttöönottotoiminto**-luettelosta joko **Asenna Office mahdollisimman pian** tai **Poista Officen asennus**.</span><span class="sxs-lookup"><span data-stu-id="afc32-113">After you have added the group or groups you want to use, from the **Deployment Action** drop-down, select either **Install Office as soon as possible** or **Uninstall Office**.</span></span>
    
    ![In the Manage Office deployment pane, choose either Install Office as soon as possible, or Uninstall Office.](media/00f24a61-1848-40c0-b037-78d726c7d757.png)
  
5. <span data-ttu-id="afc32-115">Valitse **Seuraava** \> tarkista asetukset ja valitse sitten **Vahvista**.</span><span class="sxs-lookup"><span data-stu-id="afc32-115">Choose **Next** \> review the settings and then choose **Confirm**.</span></span>
    
<span data-ttu-id="afc32-116">32-bittinen Office asennetaan automaattisesti käyttämiesi ryhmien määrittämien käyttäjien omistamiin laitteisiin tai asennus poistetaan niistä.</span><span class="sxs-lookup"><span data-stu-id="afc32-116">A 32-bit Office will be automatically installed, or uninstalled in the devices owned by users specified by the group or groups you used.</span></span>
  
<span data-ttu-id="afc32-117">Voit tarkistaa tilanteen avaamalla Tehtävienhallinnan tietokoneessa, joka valittiin Officen asennukseen, ja etsimällä Microsoft Officen pika-asennusprosessin.</span><span class="sxs-lookup"><span data-stu-id="afc32-117">To verify you can open the Task Manager on a computer that was selected for an Office install and look for Microsoft Office Click-to-Run process.</span></span>
  


