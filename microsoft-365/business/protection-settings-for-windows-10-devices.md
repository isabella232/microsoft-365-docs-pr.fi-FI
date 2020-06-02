---
title: Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Lue, miten voit luoda sovellusten hallintakäytännön ja suojata työtiedostoja käyttäjien henkilökohtaisissa Windows 10 -laitteissa.
ms.openlocfilehash: df10470c6bd7aad2f35700a267c4d24d949f569c
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470863"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="76ebb-103">Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille</span><span class="sxs-lookup"><span data-stu-id="76ebb-103">Set application protection settings for Windows 10 devices</span></span>

<span data-ttu-id="76ebb-104">Tämä artikkeli koskee Microsoft 365 Business Premiumia.</span><span class="sxs-lookup"><span data-stu-id="76ebb-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="76ebb-105">Windows 10:n sovellustenhallintakäytännön luominen</span><span class="sxs-lookup"><span data-stu-id="76ebb-105">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="76ebb-106">Jos käyttäjillä on henkilökohtaisia Windows 10 -laitteita, joissa he tekevät työtehtäviä, voit suojata tiedot myös kyseisissä laitteissa.</span><span class="sxs-lookup"><span data-stu-id="76ebb-106">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="76ebb-107">Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="76ebb-107">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="76ebb-108">Valitse vasemmanpuoleista **Devices** siirtymisruudusta \> **Laitteet-käytännöt** \> **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="76ebb-108">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>

3. <span data-ttu-id="76ebb-109">Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle.</span><span class="sxs-lookup"><span data-stu-id="76ebb-109">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="76ebb-110">Valitse **Käytännön tyyppi** -kohdassa **Windows 10:n sovellusten hallinta**.</span><span class="sxs-lookup"><span data-stu-id="76ebb-110">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="76ebb-111">Valitse **Laitetyyppi**-kohdassa joko **Henkilökohtainen** tai **Yrityksen omistama**.</span><span class="sxs-lookup"><span data-stu-id="76ebb-111">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="76ebb-112">**Salaa työtiedostot** otetaan automaattisesti käyttöön.</span><span class="sxs-lookup"><span data-stu-id="76ebb-112">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="76ebb-113">Määritä **Estä käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin ja pakota heidät tallentamaan työtiedostot OneDrive for Businessiin** **käyttöön**, jos et halua käyttäjien tallentavan työtiedostoja tietokoneeseensa.</span><span class="sxs-lookup"><span data-stu-id="76ebb-113">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
9. <span data-ttu-id="76ebb-114">Laajenna **Palauta tiedot Windows-laitteissa**.</span><span class="sxs-lookup"><span data-stu-id="76ebb-114">Expand **Recover data on Windows devices**.</span></span> <span data-ttu-id="76ebb-115">Suosittelemme, että otat sen **käyttöön**.</span><span class="sxs-lookup"><span data-stu-id="76ebb-115">We recommend that you turn it **On**.</span></span>
    
    <span data-ttu-id="76ebb-116">Ennen kuin voit etsiä Tietojenpalautusagentti-varmenteen, sinun on ensin luotava se.</span><span class="sxs-lookup"><span data-stu-id="76ebb-116">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one.</span></span> <span data-ttu-id="76ebb-117">Lisätietoja on [ohjeaiheessa EFS Data Recovery Agent (DRA) -varmenteen luominen ja tarkistaminen](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="76ebb-117">For instructions, see [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="76ebb-118">Työtiedostot on oletusarvoisesti salattu salaisella avaimella, joka on tallennettu laitteeseen ja liitetty käyttäjän profiiliin.</span><span class="sxs-lookup"><span data-stu-id="76ebb-118">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile.</span></span> <span data-ttu-id="76ebb-119">Vain käyttäjä itse voi avata tiedoston ja purkaa sen salauksen.</span><span class="sxs-lookup"><span data-stu-id="76ebb-119">Only the user can open and decrypt the file.</span></span> <span data-ttu-id="76ebb-120">Jos laite häviää tai jos käyttäjä poistetaan, tiedosto voi jäädä salattuun tilaan.</span><span class="sxs-lookup"><span data-stu-id="76ebb-120">However, if a device is lost or a user is removed, a file can be stuck in an encrypted state.</span></span> <span data-ttu-id="76ebb-121">Järjestelmänvalvoja voi purkaa tiedoston salauksen DRA (Data Recovery Agent) -varmenteen avulla.</span><span class="sxs-lookup"><span data-stu-id="76ebb-121">An admin can use the Data Recovery Agent (DRA) certificate to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="76ebb-123">Laajenna **Suojaa muita verkko- ja pilvisijainteja,** jos haluat lisätä toimialueita tai SharePoint Online -sijainteja varmistaaksesi, että kaikkien luettelossa olevien sovellusten tiedostot on suojattu.</span><span class="sxs-lookup"><span data-stu-id="76ebb-123">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps are protected.</span></span> <span data-ttu-id="76ebb-124">Jos sinun on annettava jompaankumpaan kenttään useita kohteita, lisää kohteiden väliin puolipiste (;).</span><span class="sxs-lookup"><span data-stu-id="76ebb-124">If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="76ebb-p105">Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja valitse käyttöoikeusryhmät, jotka saavat nämä asetukset \> **Valitse**.</span><span class="sxs-lookup"><span data-stu-id="76ebb-p105">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="76ebb-128">Lopuksi tallenna käytäntö valitsemalla **Lisää** ja määritä se laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="76ebb-128">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
