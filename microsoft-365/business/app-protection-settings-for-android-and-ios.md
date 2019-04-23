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
ms.openlocfilehash: e81ff8a4bd71dbbbf7ccc31249d450e03f4bd241
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277443"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="a74ab-103">Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten</span><span class="sxs-lookup"><span data-stu-id="a74ab-103">Set app protection settings for Android or iOS devices</span></span>

## <a name="create-an-app-management-policy"></a><span data-ttu-id="a74ab-104">Sovellustenhallintakäytännön luominen</span><span class="sxs-lookup"><span data-stu-id="a74ab-104">Create an app management policy</span></span>

1. <span data-ttu-id="a74ab-105">Kirjautuminen [hallintakeskukseen 365 Microsoft Business](https://go.microsoft.com/fwlink/p/?linkid=837890) yleisen järjestelmänvalvojan tunnistetiedoin.</span><span class="sxs-lookup"><span data-stu-id="a74ab-105">Sign in to [Microsoft 365 Business admin center ](https://go.microsoft.com/fwlink/p/?linkid=837890) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="a74ab-106">Valitse **laitteet** -hallintakeskukseen, \> **käytännöt** \> **Lisää käytännön**.</span><span class="sxs-lookup"><span data-stu-id="a74ab-106">In the admin center, choose **Devices** \> **Policies** \> **Add policy**.</span></span>
  
3. <span data-ttu-id="a74ab-107">Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle.</span><span class="sxs-lookup"><span data-stu-id="a74ab-107">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="a74ab-108">Valitse **Käytännön tyyppi** -kohdassa **Androidin sovellusten hallinta** tai **iOS:n sovellusten hallinta** sen mukaan, minkä käytäntöjoukon haluat luoda.</span><span class="sxs-lookup"><span data-stu-id="a74ab-108">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS** depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="a74ab-109">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like.</span><span class="sxs-lookup"><span data-stu-id="a74ab-109">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like.</span></span> <span data-ttu-id="a74ab-110">The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span><span class="sxs-lookup"><span data-stu-id="a74ab-110">The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="a74ab-111">Lisätietoja on kohdassa [käytettävissä olevat asetukset](#available-settings) .</span><span class="sxs-lookup"><span data-stu-id="a74ab-111">See [Available settings](#available-settings)  for more information.</span></span> 
    
    <span data-ttu-id="a74ab-112">Voit aina palauttaa oletusasetuksen **Oletusasetusten palauttaminen** -linkin avulla.</span><span class="sxs-lookup"><span data-stu-id="a74ab-112">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="a74ab-p102">Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja valitse käyttöoikeusryhmät, jotka saavat nämä asetukset \> **Valitse**.</span><span class="sxs-lookup"><span data-stu-id="a74ab-p102">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="a74ab-116">Lopuksi tallenna käytäntö valitsemalla **Valmis** ja määritä se laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="a74ab-116">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="a74ab-117">Sovellustenhallintakäytännön muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="a74ab-117">Edit an app management policy</span></span>

1. <span data-ttu-id="a74ab-118">**Käytännöt** kortilla Valitse **Muokkaa käytäntöä**.</span><span class="sxs-lookup"><span data-stu-id="a74ab-118">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="a74ab-119">Valitse **Muokkaa käytäntöä** -ruudussa käytäntö, jota haluat muuttaa.</span><span class="sxs-lookup"><span data-stu-id="a74ab-119">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="a74ab-p103">Valitse **Muokkaa** jokaisen asetuksen vieressä ja muuta käytännön arvoja. Kun muutat arvoa, se tallennetaan automaattisesti käytäntöön.</span><span class="sxs-lookup"><span data-stu-id="a74ab-p103">Choose **Edit** next to each setting to change the values in the policy. When you change a value, it is automatically saved into the policy</span></span> 
    
4. <span data-ttu-id="a74ab-122">Kun olet valmis, sulje **Muokkaa käytäntöä** -ruutu.</span><span class="sxs-lookup"><span data-stu-id="a74ab-122">When you are finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="a74ab-123">Sovellustenhallintakäytännön poistaminen</span><span class="sxs-lookup"><span data-stu-id="a74ab-123">Delete an app management policy</span></span>

1. <span data-ttu-id="a74ab-124">Valitse **Käytännöt**-kortissa **Poista käytäntö**.</span><span class="sxs-lookup"><span data-stu-id="a74ab-124">On the **Policies** card, choose **Delete policy**.</span></span>
    
2. <span data-ttu-id="a74ab-125">Poista haluamasi käytännöt valitsemalla ne **Poista käytäntö** -ruudussa \> **Valitse**, sitten **Vahvista**.</span><span class="sxs-lookup"><span data-stu-id="a74ab-125">On the **Delete policy** pane, choose the policies you want to delete \> **Select**, then **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="a74ab-126">Käytettävissä olevat asetukset</span><span class="sxs-lookup"><span data-stu-id="a74ab-126">Available settings</span></span>

<span data-ttu-id="a74ab-127">Seuraavissa taulukoissa on tarkkoja tietoja käytettävissä olevista asetuksista, joilla voit suojata työtiedostoja laitteissa, sekä asetuksista, joilla voit hallita käyttäjien Office-tiedostojen käyttöä mobiililaitteissa.</span><span class="sxs-lookup"><span data-stu-id="a74ab-127">The following tables give detailed information about the available settings to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="a74ab-128">Katso lisätietoja artikkelista [Miten Microsoft 365 Businessin suojausominaisuudet vastaavat Intunen asetuksia](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="a74ab-128">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="a74ab-129">Työtiedostojen suojaamisasetukset</span><span class="sxs-lookup"><span data-stu-id="a74ab-129">Settings that protect work files</span></span>

<span data-ttu-id="a74ab-130">Seuraavilla asetuksilla voidaan suojata työtiedostoja, jos käyttäjän laite katoaa tai varastetaan:</span><span class="sxs-lookup"><span data-stu-id="a74ab-130">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="a74ab-131">Asetus</span><span class="sxs-lookup"><span data-stu-id="a74ab-131">Setting</span></span>  <br/> |<span data-ttu-id="a74ab-132">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="a74ab-132">Description</span></span>  <br/> |
|<span data-ttu-id="a74ab-133">Poista työtiedostot passiivisesta laitteesta näin monen päivän kuluttua</span><span class="sxs-lookup"><span data-stu-id="a74ab-133">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="a74ab-134">Jos laitetta ei käytetä niin moneen päivään kuin tässä määrität, laitteeseen tallennetut työtiedostot poistetaan automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="a74ab-134">If a device is not used for the number of days that you specify here, any work files stored on the device will automatically be deleted.</span></span>  <br/> |
|<span data-ttu-id="a74ab-135">Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin</span><span class="sxs-lookup"><span data-stu-id="a74ab-135">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="a74ab-136">Jos tämä asetus on **käytössä**, ainoa käytettävissä oleva työtiedostojen tallennuspaikka on OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="a74ab-136">If this setting is **On**, the only available save location for work files will be OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="a74ab-137">Salaa työtiedostot</span><span class="sxs-lookup"><span data-stu-id="a74ab-137">Encrypt work files</span></span>  <br/> |<span data-ttu-id="a74ab-p104">Pidä tämä asetus **käytössä**, jotta työtiedostot suojataan salauksella. Vaikka laite katoaa tai varastetaan, kukaan voi lukea yritystietojasi.  </span><span class="sxs-lookup"><span data-stu-id="a74ab-p104">Keep this setting **On** so that work files are protected by encryption. Even if the device is lost or stolen, no one will be able to read your company data.  </span></span><br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="a74ab-140">Asetukset, joilla hallitaan käyttäjien Office-tiedostojen käyttöä mobiililaitteissa</span><span class="sxs-lookup"><span data-stu-id="a74ab-140">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="a74ab-141">Käyttäjien Office-työtiedostojen käyttöä voidaan hallita seuraavilla asetuksilla:</span><span class="sxs-lookup"><span data-stu-id="a74ab-141">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="a74ab-142">Asetus</span><span class="sxs-lookup"><span data-stu-id="a74ab-142">Setting</span></span>  <br/> |<span data-ttu-id="a74ab-143">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="a74ab-143">Description</span></span>  <br/> |
|<span data-ttu-id="a74ab-144">Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä</span><span class="sxs-lookup"><span data-stu-id="a74ab-144">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="a74ab-145">Jos tämä asetus on **käytössä**, käyttäjien on annettava toinen todennusmuoto käyttäjänimensä ja salasanansa lisäksi, ennen kuin he voivat käyttää Office-sovelluksia mobiililaitteillaan.</span><span class="sxs-lookup"><span data-stu-id="a74ab-145">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="a74ab-146">Palauta PIN-koodi, jos kirjautuminen epäonnistuu näin monta kertaa</span><span class="sxs-lookup"><span data-stu-id="a74ab-146">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="a74ab-147">Jos haluat estää luvatonta käyttäjä arvaamasta PIN-koodia sattumalta, PIN-koodi palautetaan määrittämäsi virheellisten syöttökertojen määrän jälkeen.</span><span class="sxs-lookup"><span data-stu-id="a74ab-147">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="a74ab-148">Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä</span><span class="sxs-lookup"><span data-stu-id="a74ab-148">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="a74ab-149">Tämä asetus määrittää, kuinka kauan käyttäjä voi olla toimimatta, ennen kuin häntä kehotetaan kirjautumaan sisään uudelleen.</span><span class="sxs-lookup"><span data-stu-id="a74ab-149">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="a74ab-150">Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu</span><span class="sxs-lookup"><span data-stu-id="a74ab-150">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="a74ab-p105">Kekseliäällä käyttäjällä voi olla laite, jonka suojaus on murrettu. Tämä tarkoittaa, että käyttäjä voi muokata käyttöjärjestelmää, minkä vuoksi laite voi altistua helpommin haittaohjelmille. Tällaiset laitteet on estetty, kun tämä asetus on **käytössä**.  </span><span class="sxs-lookup"><span data-stu-id="a74ab-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="a74ab-154">Salli käyttäjille sisällön kopiointi Office-sovelluksista henkilökohtaisiin sovelluksiin</span><span class="sxs-lookup"><span data-stu-id="a74ab-154">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="a74ab-155">Oletuksena tätä ei sallita, mutta jos asetus on **käytössä**, käyttäjä voi kopioida työtiedoston tietoja henkilökohtaiseen tiedostoon.</span><span class="sxs-lookup"><span data-stu-id="a74ab-155">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="a74ab-156">Jos asetuksena on **Ei käytössä**, käyttäjä ei voi kopioida tietoja työtilistä henkilökohtaiseen sovellukseen tai henkilökohtaisen tiliin.</span><span class="sxs-lookup"><span data-stu-id="a74ab-156">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
   

  

