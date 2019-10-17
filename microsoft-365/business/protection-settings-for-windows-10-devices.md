---
title: Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Lue, miten voit luoda sovellusten hallinta käytännön ja suojata työtiedostoja Windows 10-laitteissa.
ms.openlocfilehash: 0e1221e533418166b80afd94431414016774f247
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575774"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="1f09a-103">Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille</span><span class="sxs-lookup"><span data-stu-id="1f09a-103">Set application protection settings for Windows 10 devices</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="1f09a-104">Windows 10:n sovellustenhallintakäytännön luominen</span><span class="sxs-lookup"><span data-stu-id="1f09a-104">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="1f09a-105">Jos käyttäjillä on henkilökohtaisia Windows 10 -laitteita, joissa he tekevät työtehtäviä, voit suojata tiedot myös kyseisissä laitteissa.</span><span class="sxs-lookup"><span data-stu-id="1f09a-105">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="1f09a-106">Siirry hallinta keskukseen-kohtaan <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="1f09a-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="1f09a-107">Valitse vasemmasta siirtymis kohdasta **laite** \> **käytännöt** \> - **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="1f09a-107">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>

3. <span data-ttu-id="1f09a-108">Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle.</span><span class="sxs-lookup"><span data-stu-id="1f09a-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="1f09a-109">Valitse **Käytännön tyyppi** -kohdassa **Windows 10:n sovellusten hallinta**.</span><span class="sxs-lookup"><span data-stu-id="1f09a-109">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="1f09a-110">Valitse **laite tyyppi**-kohdassa joko **henkilökohtainen** tai **yrityksen omistama**.</span><span class="sxs-lookup"><span data-stu-id="1f09a-110">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="1f09a-111">**Salaa työtiedostot** otetaan automaattisesti käyttöön.</span><span class="sxs-lookup"><span data-stu-id="1f09a-111">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="1f09a-112">Määritä **Estä käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin ja pakota heidät tallentamaan työtiedostot OneDrive for Businessiin** **käyttöön**, jos et halua käyttäjien tallentavan työtiedostoja tietokoneeseensa.</span><span class="sxs-lookup"><span data-stu-id="1f09a-112">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
9. <span data-ttu-id="1f09a-113">Laajenna **Palauta tietoja Windows-laitteissa**. On suositeltavaa ottaa se **käyttöön**.</span><span class="sxs-lookup"><span data-stu-id="1f09a-113">Expand **Recover data on Windows devices** and it is recommended that you turn it **On**.</span></span>
    
    <span data-ttu-id="1f09a-p101">Ennen kuin voit etsiä Tietojenpalautusagentti-varmenteen, sinun on ensin luotava se. Ohjeita on artikkelissa [EFS-tiedostojärjestelmän Tietojenpalautusagentti-varmenteen luominen ja vahvistaminen](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="1f09a-p101">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one. For instructions see, [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="1f09a-p102">Työtiedostot on oletusarvoisesti salattu salaisella avaimella, joka on tallennettu laitteeseen ja liitetty käyttäjän profiiliin. Vain käyttäjä itse voi avata tiedoston ja purkaa sen salauksen. Jos laite häviää tai jos käyttäjä poistetaan, tiedosto voi jäädä salattuun tilaan. Järjestelmänvalvoja voi purkaa tiedoston salauksen Tietojenpalautusagentti-varmenteen (Data Recovery Agent, DRA) avulla.</span><span class="sxs-lookup"><span data-stu-id="1f09a-p102">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile. Only the user can open and decrypt the file. However, if a device is lost or a user is removed, a file can be stuck in an encrypted state. The Data Recovery Agent (DRA) certificate can be used by an admin to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="1f09a-p103">Laajenna **Suojaa muita verkko- ja pilvisijainteja**, jos haluat lisätä muita toimialueita tai SharePoint Online -sijainteja ja varmistaa, että kaikkien ilmoitettujen sovellusten tiedostot suojataan. Jos sinun on annettava jompaankumpaan kenttään useita kohteita, lisää kohteiden väliin puolipiste (;).</span><span class="sxs-lookup"><span data-stu-id="1f09a-p103">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps will be protected. If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="1f09a-p104">Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja valitse käyttöoikeusryhmät, jotka saavat nämä asetukset \> **Valitse**.</span><span class="sxs-lookup"><span data-stu-id="1f09a-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="1f09a-126">Lopuksi tallenna käytäntö valitsemalla **Lisää** ja määritä se laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="1f09a-126">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 