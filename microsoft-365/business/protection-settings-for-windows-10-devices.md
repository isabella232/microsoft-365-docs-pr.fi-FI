---
title: Sovelluksen suojausasetusten muokkaaminen tai määrittäminen Windows 10 -laitteissa
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
description: Opi luomaan tai muokkaamaan sovellusten hallintakäytäntöjä ja suojaamaan työtiedostoja käyttäjien henkilökohtaisissa Windows 10 -laitteissa.
ms.openlocfilehash: 64c6aa620171a373cd7564c7de3abbf4a4546c4e
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912818"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="1921f-103">Sovellusten suojausasetusten määrittäminen tai muokkaaminen Windows 10 -laitteissa</span><span class="sxs-lookup"><span data-stu-id="1921f-103">Set or edit application protection settings for Windows 10 devices</span></span>

<span data-ttu-id="1921f-104">Tämä artikkeli koskee Microsoft 365 Business Premiumia.</span><span class="sxs-lookup"><span data-stu-id="1921f-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="edit-an-app-management-policy-for-windows-10"></a><span data-ttu-id="1921f-105">Sovelluksen hallintakäytännön muokkaaminen Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="1921f-105">Edit an app management policy for Windows 10</span></span>

1. <span data-ttu-id="1921f-106">Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="1921f-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>     
2. <span data-ttu-id="1921f-107">Valitse vasemmassa siirtymispalkin kohdassa  \> **Laitekäytännöt.**</span><span class="sxs-lookup"><span data-stu-id="1921f-107">On the left nav, choose **Devices** \> **Policies** .</span></span>
1. <span data-ttu-id="1921f-108">Valitse olemassa oleva Windows-sovelluskäytäntö ja sitten **Muokkaa.**</span><span class="sxs-lookup"><span data-stu-id="1921f-108">Choose an existing Windows app policy and then **Edit**.</span></span>
1. <span data-ttu-id="1921f-109">Valitse **Muokkaa** sen asetuksen vieressä, jota haluat muuttaa, ja valitse **sitten Tallenna.**</span><span class="sxs-lookup"><span data-stu-id="1921f-109">Choose **Edit** next to a setting you want to change and then **Save**.</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="1921f-110">Windows 10:n sovellustenhallintakäytännön luominen</span><span class="sxs-lookup"><span data-stu-id="1921f-110">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="1921f-111">Jos käyttäjillä on henkilökohtaisia Windows 10 -laitteita, joissa he tekevät työtehtäviä, voit suojata tiedot myös kyseisissä laitteissa.</span><span class="sxs-lookup"><span data-stu-id="1921f-111">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="1921f-112">Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="1921f-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
2. <span data-ttu-id="1921f-113">Valitse vasemmassa siirtymispalkin kohdassa  \> **Laitekäytännöt** \> **Lisää.**</span><span class="sxs-lookup"><span data-stu-id="1921f-113">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
3. <span data-ttu-id="1921f-114">Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle.</span><span class="sxs-lookup"><span data-stu-id="1921f-114">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
4. <span data-ttu-id="1921f-115">Valitse **Käytännön tyyppi** -kohdassa **Windows 10:n sovellusten hallinta**.</span><span class="sxs-lookup"><span data-stu-id="1921f-115">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
5. <span data-ttu-id="1921f-116">Valitse **Laitetyyppi-kohdassa** joko **Henkilökohtainen tai** **Yrityksen omistama.**</span><span class="sxs-lookup"><span data-stu-id="1921f-116">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
6. <span data-ttu-id="1921f-117">**Salaa työtiedostot** otetaan automaattisesti käyttöön.</span><span class="sxs-lookup"><span data-stu-id="1921f-117">The **Encrypt work files** is turned on automatically.</span></span> 
7. <span data-ttu-id="1921f-118">Määritä **Estä käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin ja pakota heidät tallentamaan työtiedostot OneDrive for Businessiin** **käyttöön**, jos et halua käyttäjien tallentavan työtiedostoja tietokoneeseensa.</span><span class="sxs-lookup"><span data-stu-id="1921f-118">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
9. <span data-ttu-id="1921f-119">Laajenna **Palauta tietoja Windows-laitteissa.**</span><span class="sxs-lookup"><span data-stu-id="1921f-119">Expand **Recover data on Windows devices**.</span></span> <span data-ttu-id="1921f-120">On suositeltavaa ottaa se **käyttöön.**</span><span class="sxs-lookup"><span data-stu-id="1921f-120">We recommend that you turn it **On**.</span></span>
    <span data-ttu-id="1921f-121">Ennen kuin voit etsiä Tietojenpalautusagentti-varmenteen, sinun on ensin luotava se.</span><span class="sxs-lookup"><span data-stu-id="1921f-121">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one.</span></span> <span data-ttu-id="1921f-122">Ohjeet ovat kohdassa [EFS (Encrypting File System) -tietojenpalautusagentin (DRA) varmenteen luominen ja tarkistaminen.](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate)</span><span class="sxs-lookup"><span data-stu-id="1921f-122">For instructions, see [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate).</span></span>
    
    <span data-ttu-id="1921f-123">Työtiedostot on oletusarvoisesti salattu salaisella avaimella, joka on tallennettu laitteeseen ja liitetty käyttäjän profiiliin.</span><span class="sxs-lookup"><span data-stu-id="1921f-123">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile.</span></span> <span data-ttu-id="1921f-124">Vain käyttäjä itse voi avata tiedoston ja purkaa sen salauksen.</span><span class="sxs-lookup"><span data-stu-id="1921f-124">Only the user can open and decrypt the file.</span></span> <span data-ttu-id="1921f-125">Jos laite häviää tai jos käyttäjä poistetaan, tiedosto voi jäädä salattuun tilaan.</span><span class="sxs-lookup"><span data-stu-id="1921f-125">However, if a device is lost or a user is removed, a file can be stuck in an encrypted state.</span></span> <span data-ttu-id="1921f-126">Järjestelmänvalvoja voi purkaa tiedoston salauksen Tietojenpalautusagentti (DRA) -varmenteen avulla.</span><span class="sxs-lookup"><span data-stu-id="1921f-126">An admin can use the Data Recovery Agent (DRA) certificate to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="1921f-128">Laajenna **Suojaa lisää verkko- ja** pilvisijainteja, jos haluat lisätä muita toimialueita tai SharePoint Online -sijainteja ja varmistaa, että kaikkien luettelossa lueteltujen sovellusten tiedostot on suojattu.</span><span class="sxs-lookup"><span data-stu-id="1921f-128">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps are protected.</span></span> <span data-ttu-id="1921f-129">Jos sinun on annettava jompaankumpaan kenttään useita kohteita, lisää kohteiden väliin puolipiste (;).</span><span class="sxs-lookup"><span data-stu-id="1921f-129">If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="1921f-p104">Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja valitse käyttöoikeusryhmät, jotka saavat nämä asetukset \> **Valitse**.</span><span class="sxs-lookup"><span data-stu-id="1921f-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
12. <span data-ttu-id="1921f-133">Lopuksi tallenna käytäntö valitsemalla **Lisää** ja määritä se laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="1921f-133">Finally, choose **Add** to save the policy, and assign it to devices.</span></span>