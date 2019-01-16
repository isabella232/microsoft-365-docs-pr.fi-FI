---
title: Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Opi app hallintakäytännön luominen ja suojaamaan työn tiedostoja Windows 10-laitteissa.
ms.openlocfilehash: acf19a72d994185a35b2e425f8334a73a121ee10
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982823"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="28cc3-103">Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille</span><span class="sxs-lookup"><span data-stu-id="28cc3-103">Set application protection settings for Windows 10 devices</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="28cc3-104">Windows 10:n sovellustenhallintakäytännön luominen</span><span class="sxs-lookup"><span data-stu-id="28cc3-104">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="28cc3-105">Jos käyttäjillä on henkilökohtaisia Windows 10 -laitteita, joissa he tekevät työtehtäviä, voit suojata tiedot myös kyseisissä laitteissa.</span><span class="sxs-lookup"><span data-stu-id="28cc3-105">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="28cc3-p101">Kirjaudu [Microsoft 365 Businessiin](https://portal.office.com) yleisen järjestelmänvalvojan tunnistetiedoilla. Siirry hallintakeskukseen valitsemalla **Järjestelmänvalvoja** -ruutu.</span><span class="sxs-lookup"><span data-stu-id="28cc3-p101">Sign in to [Microsoft 365 Business](https://portal.office.com) with global admin credentials. Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="28cc3-108">Valitse hallintaportaalin **Laitekäytännöt**-kortissa **Lisää käytäntö**.</span><span class="sxs-lookup"><span data-stu-id="28cc3-108">On the **Device policies** card of the admin portal, choose **Add policy**.</span></span>
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. <span data-ttu-id="28cc3-110">Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle.</span><span class="sxs-lookup"><span data-stu-id="28cc3-110">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="28cc3-111">Valitse **Käytännön tyyppi** -kohdassa **Windows 10:n sovellusten hallinta**.</span><span class="sxs-lookup"><span data-stu-id="28cc3-111">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="28cc3-112">Valitse \*\* laitetyyppi \*\*, **henkilökohtaisia** tai **Yrityksen omistuksessa**.</span><span class="sxs-lookup"><span data-stu-id="28cc3-112">Under \*\* Device type \*\*, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="28cc3-113">**Salaa työtiedostot** otetaan automaattisesti käyttöön.</span><span class="sxs-lookup"><span data-stu-id="28cc3-113">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="28cc3-114">Määritä **Estä käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin ja pakota heidät tallentamaan työtiedostot OneDrive for Businessiin** **käyttöön**, jos et halua käyttäjien tallentavan työtiedostoja tietokoneeseensa.</span><span class="sxs-lookup"><span data-stu-id="28cc3-114">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
8. <span data-ttu-id="28cc3-p102">Laajenna **hallita, miten käyttäjät voivat käyttää Office-tiedostojen, laitteiden** \> miten asetukset. **Miten käyttäjät voivat käyttää Office-laitteita mobiililaitteiden hallinta** ei **ole käytössä** oletusarvoisesti, mutta voit ottaa sen **käyttöön** ja hyväksyä oletusarvot on suositeltavaa. Lisätietoja on kohdassa [käytettävissä olevat asetukset](protection-settings-for-windows-10-devices.md#bkmk_settings) .</span><span class="sxs-lookup"><span data-stu-id="28cc3-p102">Expand **Manage how users access Office files on devices** \> configure the settings how you would like. The **Manage how users access Office devices on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values. See [Available settings](protection-settings-for-windows-10-devices.md#bkmk_settings) for more information.</span></span> 
    
    <span data-ttu-id="28cc3-118">Voit aina palauttaa oletusasetuksen **Oletusasetusten palauttaminen** -linkin avulla.</span><span class="sxs-lookup"><span data-stu-id="28cc3-118">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
9. <span data-ttu-id="28cc3-119">Laajenna **Palauta tietoja Windows-laitteissa**. On suositeltavaa ottaa se **käyttöön**.</span><span class="sxs-lookup"><span data-stu-id="28cc3-119">Expand **Recover data on Windows devices** and it is recommended that you turn it **On**.</span></span>
    
    <span data-ttu-id="28cc3-p103">Ennen kuin voit etsiä Tietojenpalautusagentti-varmenteen, sinun on ensin luotava se. Ohjeita on artikkelissa [EFS-tiedostojärjestelmän Tietojenpalautusagentti-varmenteen luominen ja vahvistaminen](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="28cc3-p103">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one. For instructions see, [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="28cc3-p104">Työtiedostot on oletusarvoisesti salattu salaisella avaimella, joka on tallennettu laitteeseen ja liitetty käyttäjän profiiliin. Vain käyttäjä itse voi avata tiedoston ja purkaa sen salauksen. Jos laite häviää tai jos käyttäjä poistetaan, tiedosto voi jäädä salattuun tilaan. Järjestelmänvalvoja voi purkaa tiedoston salauksen Tietojenpalautusagentti-varmenteen (Data Recovery Agent, DRA) avulla.</span><span class="sxs-lookup"><span data-stu-id="28cc3-p104">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile. Only the user can open and decrypt the file. However, if a device is lost or a user is removed, a file can be stuck in an encrypted state. The Data Recovery Agent (DRA) certificate can be used by an admin to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="28cc3-p105">Laajenna **Suojaa muita verkko- ja pilvisijainteja**, jos haluat lisätä muita toimialueita tai SharePoint Online -sijainteja ja varmistaa, että kaikkien ilmoitettujen sovellusten tiedostot suojataan. Jos sinun on annettava jompaankumpaan kenttään useita kohteita, lisää kohteiden väliin puolipiste (;).</span><span class="sxs-lookup"><span data-stu-id="28cc3-p105">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps will be protected. If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span> 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="28cc3-p106">Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja valitse käyttöoikeusryhmät, jotka saavat nämä asetukset \> **Valitse**.</span><span class="sxs-lookup"><span data-stu-id="28cc3-p106">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="28cc3-132">Lopuksi tallenna käytäntö valitsemalla **Lisää** ja määritä se laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="28cc3-132">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="28cc3-133">Käytettävissä olevat asetukset</span><span class="sxs-lookup"><span data-stu-id="28cc3-133">Available settings</span></span>

<span data-ttu-id="28cc3-134">Käyttäjien Office-työtiedostojen käyttöä voidaan hallita seuraavilla asetuksilla:</span><span class="sxs-lookup"><span data-stu-id="28cc3-134">The following settings are available to manage how users access Office work files.</span></span>
  
<span data-ttu-id="28cc3-135">Katso lisätietoja artikkelista [Miten Microsoft 365 Businessin suojausominaisuudet vastaavat Intunen asetuksia](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="28cc3-135">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span>
  
|<span data-ttu-id="28cc3-136">**Asetus**</span><span class="sxs-lookup"><span data-stu-id="28cc3-136">**Setting**</span></span>|<span data-ttu-id="28cc3-137">**Kuvaus**</span><span class="sxs-lookup"><span data-stu-id="28cc3-137">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="28cc3-138">Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä</span><span class="sxs-lookup"><span data-stu-id="28cc3-138">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="28cc3-139">Jos tämä asetus on **käytössä**, käyttäjien on annettava toinen todennusmuoto käyttäjänimensä ja salasanansa lisäksi, ennen kuin he voivat käyttää Office-sovelluksia mobiililaitteillaan.</span><span class="sxs-lookup"><span data-stu-id="28cc3-139">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="28cc3-140">Palauta PIN-koodi, jos kirjautuminen epäonnistuu näin monta kertaa</span><span class="sxs-lookup"><span data-stu-id="28cc3-140">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="28cc3-141">Jos haluat estää luvatonta käyttäjä arvaamasta PIN-koodia sattumalta, PIN-koodi palautetaan määrittämäsi virheellisten syöttökertojen määrän jälkeen.</span><span class="sxs-lookup"><span data-stu-id="28cc3-141">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="28cc3-142">Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä</span><span class="sxs-lookup"><span data-stu-id="28cc3-142">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="28cc3-143">Tämä asetus määrittää, kuinka kauan käyttäjä voi olla toimimatta, ennen kuin häntä kehotetaan kirjautumaan sisään uudelleen.</span><span class="sxs-lookup"><span data-stu-id="28cc3-143">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
   

