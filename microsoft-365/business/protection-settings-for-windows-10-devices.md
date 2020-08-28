---
title: Sovellusten suojaus asetusten muokkaaminen tai määrittäminen Windows 10-laitteille
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
description: Lue, miten voit luoda tai muokata sovellusten hallinta käytäntöjä ja suojata työtiedostoja käyttäjien henkilökohtaisissa Windows 10-laitteissa.
ms.openlocfilehash: f85a59649e43c141b62091337b842a490d411833
ms.sourcegitcommit: abf63669daf12993ad3353e4b578f41c8910b20f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/27/2020
ms.locfileid: "47289195"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="8a004-103">Windows 10-laitteiden sovellusten suojaus asetusten määrittäminen tai muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="8a004-103">Set or edit application protection settings for Windows 10 devices</span></span>

<span data-ttu-id="8a004-104">Tämä artikkeli koskee Microsoft 365 Business Premiumia.</span><span class="sxs-lookup"><span data-stu-id="8a004-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="edit-an-app-management-policy-for-windows-10"></a><span data-ttu-id="8a004-105">Sovelluksen hallinta käytännön muokkaaminen Windows 10-sovelluksessa</span><span class="sxs-lookup"><span data-stu-id="8a004-105">Edit an app management policy for Windows 10</span></span>

1. <span data-ttu-id="8a004-106">Siirry hallinta keskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="8a004-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>     
2. <span data-ttu-id="8a004-107">Valitse vasemmanpuoleisesta siirtymis ruudusta **laitteet** - \> **käytännöt** .</span><span class="sxs-lookup"><span data-stu-id="8a004-107">On the left nav, choose **Devices** \> **Policies** .</span></span>
1. <span data-ttu-id="8a004-108">Valitse aiemmin luotu Windows-sovellus käytännössä ja **Muokkaa**sitä.</span><span class="sxs-lookup"><span data-stu-id="8a004-108">Choose an existing Windows app policy and then **Edit**.</span></span>
1. <span data-ttu-id="8a004-109">Valitse **Muokkaa** sen asetus kohdan vierestä, jota haluat muuttaa, ja valitse sitten **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="8a004-109">Choose **Edit** next to a setting you want to change and then **Save**.</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="8a004-110">Windows 10:n sovellustenhallintakäytännön luominen</span><span class="sxs-lookup"><span data-stu-id="8a004-110">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="8a004-111">Jos käyttäjillä on henkilökohtaisia Windows 10 -laitteita, joissa he tekevät työtehtäviä, voit suojata tiedot myös kyseisissä laitteissa.</span><span class="sxs-lookup"><span data-stu-id="8a004-111">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="8a004-112">Siirry hallinta keskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="8a004-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
2. <span data-ttu-id="8a004-113">Valitse vasemmanpuoleisesta siirtymis ruudusta **laitteet** \> **käytännöt** \> **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="8a004-113">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
3. <span data-ttu-id="8a004-114">Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle.</span><span class="sxs-lookup"><span data-stu-id="8a004-114">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
4. <span data-ttu-id="8a004-115">Valitse **Käytännön tyyppi** -kohdassa **Windows 10:n sovellusten hallinta**.</span><span class="sxs-lookup"><span data-stu-id="8a004-115">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
5. <span data-ttu-id="8a004-116">Valitse **laite tyyppi**-kohdassa joko **henkilökohtainen** tai **yrityksen omistama**.</span><span class="sxs-lookup"><span data-stu-id="8a004-116">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
6. <span data-ttu-id="8a004-117">**Salaa työtiedostot** otetaan automaattisesti käyttöön.</span><span class="sxs-lookup"><span data-stu-id="8a004-117">The **Encrypt work files** is turned on automatically.</span></span> 
7. <span data-ttu-id="8a004-118">Määritä **Estä käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin ja pakota heidät tallentamaan työtiedostot OneDrive for Businessiin** **käyttöön**, jos et halua käyttäjien tallentavan työtiedostoja tietokoneeseensa.</span><span class="sxs-lookup"><span data-stu-id="8a004-118">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
9. <span data-ttu-id="8a004-119">Laajenna **tietojen palauttaminen Windows-laitteissa**.</span><span class="sxs-lookup"><span data-stu-id="8a004-119">Expand **Recover data on Windows devices**.</span></span> <span data-ttu-id="8a004-120">Suosittelemme **, että otat sen käyttöön**.</span><span class="sxs-lookup"><span data-stu-id="8a004-120">We recommend that you turn it **On**.</span></span>
    <span data-ttu-id="8a004-121">Ennen kuin voit etsiä Tietojenpalautusagentti-varmenteen, sinun on ensin luotava se.</span><span class="sxs-lookup"><span data-stu-id="8a004-121">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one.</span></span> <span data-ttu-id="8a004-122">Lisä tietoja on artikkelissa EFS [(Encrypting File System)-tietojen palautus agentin (DRA) varmenteen luominen ja tarkistaminen](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="8a004-122">For instructions, see [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="8a004-123">Työtiedostot on oletusarvoisesti salattu salaisella avaimella, joka on tallennettu laitteeseen ja liitetty käyttäjän profiiliin.</span><span class="sxs-lookup"><span data-stu-id="8a004-123">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile.</span></span> <span data-ttu-id="8a004-124">Vain käyttäjä itse voi avata tiedoston ja purkaa sen salauksen.</span><span class="sxs-lookup"><span data-stu-id="8a004-124">Only the user can open and decrypt the file.</span></span> <span data-ttu-id="8a004-125">Jos laite häviää tai jos käyttäjä poistetaan, tiedosto voi jäädä salattuun tilaan.</span><span class="sxs-lookup"><span data-stu-id="8a004-125">However, if a device is lost or a user is removed, a file can be stuck in an encrypted state.</span></span> <span data-ttu-id="8a004-126">Järjestelmänvalvoja voi purkaa tiedoston Sala uksen käyttämällä tietojen palautus agentti (DRA)-varmennetta.</span><span class="sxs-lookup"><span data-stu-id="8a004-126">An admin can use the Data Recovery Agent (DRA) certificate to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="8a004-128">Laajenna **suojaa muita verkko-ja pilvi sijainteja** , jos haluat lisätä muita toimi alueita tai SharePoint Online-sijainteja varmistaaksesi, että kaikkien luettelossa olevien sovellusten tiedostot ovat suojattuja.</span><span class="sxs-lookup"><span data-stu-id="8a004-128">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps are protected.</span></span> <span data-ttu-id="8a004-129">Jos sinun on annettava jompaankumpaan kenttään useita kohteita, lisää kohteiden väliin puolipiste (;).</span><span class="sxs-lookup"><span data-stu-id="8a004-129">If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="8a004-p104">Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja valitse käyttöoikeusryhmät, jotka saavat nämä asetukset \> **Valitse**.</span><span class="sxs-lookup"><span data-stu-id="8a004-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
12. <span data-ttu-id="8a004-133">Lopuksi tallenna käytäntö valitsemalla **Lisää** ja määritä se laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="8a004-133">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
