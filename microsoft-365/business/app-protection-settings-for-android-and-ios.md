---
title: Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten
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
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Opi luoda, muokata, tai poistaa app hallintakäytännön ja suojaamaan työn tiedostoja Android tai iOS-laitteissa.
ms.openlocfilehash: 04479360bf13a8ff685a91ed95440c08f8cf80b4
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660532"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="2995c-103">Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten</span><span class="sxs-lookup"><span data-stu-id="2995c-103">Set app protection settings for Android or iOS devices</span></span>

![Nauha, joka osoittaa https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a><span data-ttu-id="2995c-105">Sovellustenhallintakäytännön luominen</span><span class="sxs-lookup"><span data-stu-id="2995c-105">Create an app management policy</span></span>

1. <span data-ttu-id="2995c-106">Siirry hallintakeskukseen <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="2995c-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="2995c-107">Valitse vasemman nav- **laitteiden** \> **käytännöt** \> **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="2995c-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="2995c-108">Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle.</span><span class="sxs-lookup"><span data-stu-id="2995c-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="2995c-109">Valitse **Käytännön tyyppi** -kohdassa **Androidin sovellusten hallinta** tai **iOS:n sovellusten hallinta** sen mukaan, minkä käytäntöjoukon haluat luoda.</span><span class="sxs-lookup"><span data-stu-id="2995c-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS** depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="2995c-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like.</span><span class="sxs-lookup"><span data-stu-id="2995c-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like.</span></span> <span data-ttu-id="2995c-111">The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span><span class="sxs-lookup"><span data-stu-id="2995c-111">The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="2995c-112">Lisätietoja on kohdassa [käytettävissä olevat asetukset](#available-settings) .</span><span class="sxs-lookup"><span data-stu-id="2995c-112">See [Available settings](#available-settings)  for more information.</span></span> 
    
    <span data-ttu-id="2995c-113">Voit aina palauttaa oletusasetuksen **Oletusasetusten palauttaminen** -linkin avulla.</span><span class="sxs-lookup"><span data-stu-id="2995c-113">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="2995c-p102">Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja valitse käyttöoikeusryhmät, jotka saavat nämä asetukset \> **Valitse**.</span><span class="sxs-lookup"><span data-stu-id="2995c-p102">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="2995c-117">Lopuksi tallenna käytäntö valitsemalla **Valmis** ja määritä se laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="2995c-117">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="2995c-118">Sovellustenhallintakäytännön muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="2995c-118">Edit an app management policy</span></span>

1. <span data-ttu-id="2995c-119">**Käytännöt** kortilla Valitse **Muokkaa käytäntöä**.</span><span class="sxs-lookup"><span data-stu-id="2995c-119">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="2995c-120">Valitse **Muokkaa käytäntöä** -ruudussa käytäntö, jota haluat muuttaa.</span><span class="sxs-lookup"><span data-stu-id="2995c-120">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="2995c-p103">Valitse **Muokkaa** jokaisen asetuksen vieressä ja muuta käytännön arvoja. Kun muutat arvoa, se tallennetaan automaattisesti käytäntöön.</span><span class="sxs-lookup"><span data-stu-id="2995c-p103">Choose **Edit** next to each setting to change the values in the policy. When you change a value, it is automatically saved into the policy</span></span> 
    
4. <span data-ttu-id="2995c-123">Kun olet valmis, sulje **Muokkaa käytäntöä** -ruutu.</span><span class="sxs-lookup"><span data-stu-id="2995c-123">When you are finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="2995c-124">Sovellustenhallintakäytännön poistaminen</span><span class="sxs-lookup"><span data-stu-id="2995c-124">Delete an app management policy</span></span>

1. <span data-ttu-id="2995c-125">**Käytännöt** -sivulla Valitse käytäntö ja sitten **Poista**.</span><span class="sxs-lookup"><span data-stu-id="2995c-125">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="2995c-126">Valitse **Vahvista** poistaa käytännön tai käytäntöjen valitsit **Poista käytäntö** -ruudussa.</span><span class="sxs-lookup"><span data-stu-id="2995c-126">On the **Delete policy** pane choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="2995c-127">Käytettävissä olevat asetukset</span><span class="sxs-lookup"><span data-stu-id="2995c-127">Available settings</span></span>

<span data-ttu-id="2995c-128">Seuraavissa taulukoissa on tarkkoja tietoja käytettävissä olevista asetuksista, joilla voit suojata työtiedostoja laitteissa, sekä asetuksista, joilla voit hallita käyttäjien Office-tiedostojen käyttöä mobiililaitteissa.</span><span class="sxs-lookup"><span data-stu-id="2995c-128">The following tables give detailed information about the available settings to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="2995c-129">Katso lisätietoja artikkelista [Miten Microsoft 365 Businessin suojausominaisuudet vastaavat Intunen asetuksia](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="2995c-129">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="2995c-130">Työtiedostojen suojaamisasetukset</span><span class="sxs-lookup"><span data-stu-id="2995c-130">Settings that protect work files</span></span>

<span data-ttu-id="2995c-131">Seuraavilla asetuksilla voidaan suojata työtiedostoja, jos käyttäjän laite katoaa tai varastetaan:</span><span class="sxs-lookup"><span data-stu-id="2995c-131">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="2995c-132">Asetus</span><span class="sxs-lookup"><span data-stu-id="2995c-132">Setting</span></span>  <br/> |<span data-ttu-id="2995c-133">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="2995c-133">Description</span></span>  <br/> |
|<span data-ttu-id="2995c-134">Poista työtiedostot passiivisesta laitteesta näin monen päivän kuluttua</span><span class="sxs-lookup"><span data-stu-id="2995c-134">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="2995c-135">Jos laitetta ei käytetä niin moneen päivään kuin tässä määrität, laitteeseen tallennetut työtiedostot poistetaan automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="2995c-135">If a device is not used for the number of days that you specify here, any work files stored on the device will automatically be deleted.</span></span>  <br/> |
|<span data-ttu-id="2995c-136">Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin</span><span class="sxs-lookup"><span data-stu-id="2995c-136">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="2995c-137">Jos tämä asetus on **käytössä**, ainoa käytettävissä oleva työtiedostojen tallennuspaikka on OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="2995c-137">If this setting is **On**, the only available save location for work files will be OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="2995c-138">Salaa työtiedostot</span><span class="sxs-lookup"><span data-stu-id="2995c-138">Encrypt work files</span></span>  <br/> |<span data-ttu-id="2995c-p104">Pidä tämä asetus **käytössä**, jotta työtiedostot suojataan salauksella. Vaikka laite katoaa tai varastetaan, kukaan voi lukea yritystietojasi.  </span><span class="sxs-lookup"><span data-stu-id="2995c-p104">Keep this setting **On** so that work files are protected by encryption. Even if the device is lost or stolen, no one will be able to read your company data.  </span></span><br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="2995c-141">Asetukset, joilla hallitaan käyttäjien Office-tiedostojen käyttöä mobiililaitteissa</span><span class="sxs-lookup"><span data-stu-id="2995c-141">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="2995c-142">Käyttäjien Office-työtiedostojen käyttöä voidaan hallita seuraavilla asetuksilla:</span><span class="sxs-lookup"><span data-stu-id="2995c-142">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="2995c-143">Asetus</span><span class="sxs-lookup"><span data-stu-id="2995c-143">Setting</span></span>  <br/> |<span data-ttu-id="2995c-144">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="2995c-144">Description</span></span>  <br/> |
|<span data-ttu-id="2995c-145">Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä</span><span class="sxs-lookup"><span data-stu-id="2995c-145">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="2995c-146">Jos tämä asetus on **käytössä**, käyttäjien on annettava toinen todennusmuoto käyttäjänimensä ja salasanansa lisäksi, ennen kuin he voivat käyttää Office-sovelluksia mobiililaitteillaan.</span><span class="sxs-lookup"><span data-stu-id="2995c-146">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="2995c-147">Palauta PIN-koodi, jos kirjautuminen epäonnistuu näin monta kertaa</span><span class="sxs-lookup"><span data-stu-id="2995c-147">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="2995c-148">Jos haluat estää luvatonta käyttäjä arvaamasta PIN-koodia sattumalta, PIN-koodi palautetaan määrittämäsi virheellisten syöttökertojen määrän jälkeen.</span><span class="sxs-lookup"><span data-stu-id="2995c-148">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="2995c-149">Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä</span><span class="sxs-lookup"><span data-stu-id="2995c-149">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="2995c-150">Tämä asetus määrittää, kuinka kauan käyttäjä voi olla toimimatta, ennen kuin häntä kehotetaan kirjautumaan sisään uudelleen.</span><span class="sxs-lookup"><span data-stu-id="2995c-150">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="2995c-151">Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu</span><span class="sxs-lookup"><span data-stu-id="2995c-151">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="2995c-p105">Kekseliäällä käyttäjällä voi olla laite, jonka suojaus on murrettu. Tämä tarkoittaa, että käyttäjä voi muokata käyttöjärjestelmää, minkä vuoksi laite voi altistua helpommin haittaohjelmille. Tällaiset laitteet on estetty, kun tämä asetus on **käytössä**.  </span><span class="sxs-lookup"><span data-stu-id="2995c-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="2995c-155">Salli käyttäjille sisällön kopiointi Office-sovelluksista henkilökohtaisiin sovelluksiin</span><span class="sxs-lookup"><span data-stu-id="2995c-155">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="2995c-156">Oletuksena tätä ei sallita, mutta jos asetus on **käytössä**, käyttäjä voi kopioida työtiedoston tietoja henkilökohtaiseen tiedostoon.</span><span class="sxs-lookup"><span data-stu-id="2995c-156">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="2995c-157">Jos asetuksena on **Ei käytössä**, käyttäjä ei voi kopioida tietoja työtilistä henkilökohtaiseen sovellukseen tai henkilökohtaisen tiliin.</span><span class="sxs-lookup"><span data-stu-id="2995c-157">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
   

  

