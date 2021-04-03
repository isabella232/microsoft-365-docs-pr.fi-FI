---
title: Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Opi luomaan, muokkaamaan tai poistamaan sovellusten hallintakäytäntöä ja suojaamaan työtiedostoja Android- tai iOS-laitteissa.
ms.openlocfilehash: 2e157737990c7aca6e87a676e90f62f0d40ad372
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580290"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="5d8a1-103">Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten</span><span class="sxs-lookup"><span data-stu-id="5d8a1-103">Set app protection settings for Android or iOS devices</span></span>

<span data-ttu-id="5d8a1-104">Tämä artikkeli koskee Microsoft 365 Business Premiumia.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="create-an-app-management-policy"></a><span data-ttu-id="5d8a1-105">Sovellustenhallintakäytännön luominen</span><span class="sxs-lookup"><span data-stu-id="5d8a1-105">Create an app management policy</span></span>

1. <span data-ttu-id="5d8a1-106">Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="5d8a1-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="5d8a1-107">Valitse vasemmassa siirtymispalkin kohdassa  \> **Laitekäytännöt** \> **Lisää.**</span><span class="sxs-lookup"><span data-stu-id="5d8a1-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="5d8a1-108">Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="5d8a1-109">Valitse **Käytäntötyyppi-kohdassa** **Androidin** sovellusten hallinta tai **iOS:n** sovellusten hallinta sen mukaan, mitkä käytännöt haluat luoda.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS**, depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="5d8a1-110">Laajenna **Suojaa työtiedostot, kun laitteita katoaa tai varastetaan,** ja **hallitse, miten käyttäjät voivat käyttää Office-tiedostoja mobiililaitteissa.**</span><span class="sxs-lookup"><span data-stu-id="5d8a1-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices**.</span></span> <span data-ttu-id="5d8a1-111">Määritä asetukset, miten haluat.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-111">Configure the settings how you would like.</span></span> <span data-ttu-id="5d8a1-112">**Hallitse sitä, miten käyttäjät** voivat  käyttää Office-tiedostoja mobiililaitteissa, on oletusarvoisesti poissa käytöstä, mutta on suositeltavaa ottaa se **käyttöön** ja hyväksyä oletusarvot.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-112">**Manage how users access Office files on mobile devices** is **Off** by default, but we recommend that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="5d8a1-113">Lisätietoja on kohdassa Käytettävissä [olevat asetukset.](#available-settings)</span><span class="sxs-lookup"><span data-stu-id="5d8a1-113">For more information, see [Available settings](#available-settings).</span></span> 
    
    <span data-ttu-id="5d8a1-114">Voit aina palauttaa oletusasetuksen **Oletusasetusten palauttaminen** -linkin avulla.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-114">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="5d8a1-116">Päätä seuraavaksi, **ketkä saavat nämä asetukset**.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-116">Next decide **Who will get these settings?**</span></span> <span data-ttu-id="5d8a1-117">Jos et halua käyttää oletusarvoista  Kaikki käyttäjät -käyttöoikeusryhmää, valitse Muuta **ja** valitse käyttöoikeusryhmät, jotka saavat nämä \> **asetukset. Valitse**.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-117">If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups that get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="5d8a1-118">Lopuksi tallenna käytäntö valitsemalla **Valmis** ja määritä se laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-118">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="5d8a1-119">Sovellustenhallintakäytännön muokkaaminen</span><span class="sxs-lookup"><span data-stu-id="5d8a1-119">Edit an app management policy</span></span>

1. <span data-ttu-id="5d8a1-120">Valitse **Käytännöt-kortissa** **Muokkaa käytäntöä.**</span><span class="sxs-lookup"><span data-stu-id="5d8a1-120">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="5d8a1-121">Valitse **Muokkaa käytäntöä** -ruudussa käytäntö, jota haluat muuttaa.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-121">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="5d8a1-122">Valitse **Muokkaa** jokaisen asetuksen vieressä ja muuta käytännön arvoja.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-122">Choose **Edit** next to each setting to change the values in the policy.</span></span> <span data-ttu-id="5d8a1-123">Kun muutat arvoa, se tallennetaan automaattisesti käytäntöön.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-123">When you change a value, it's automatically saved in the policy.</span></span>
    
4. <span data-ttu-id="5d8a1-124">Kun olet valmis, sulje Muokkaa **käytäntöä -ruutu.**</span><span class="sxs-lookup"><span data-stu-id="5d8a1-124">When you're finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="5d8a1-125">Sovellustenhallintakäytännön poistaminen</span><span class="sxs-lookup"><span data-stu-id="5d8a1-125">Delete an app management policy</span></span>

1. <span data-ttu-id="5d8a1-126">Valitse **Käytännöt-sivulla** käytäntö ja valitse **sitten Poista.**</span><span class="sxs-lookup"><span data-stu-id="5d8a1-126">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="5d8a1-127">Valitse Poista **käytäntö -ruudussa** **Vahvista,** jos haluat poistaa valitsemasi käytännön tai käytännöt.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-127">On the **Delete policy** pane, choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="5d8a1-128">Käytettävissä olevat asetukset</span><span class="sxs-lookup"><span data-stu-id="5d8a1-128">Available settings</span></span>

<span data-ttu-id="5d8a1-129">Seuraavissa taulukoissa annetaan yksityiskohtaisia tietoja käytettävissä olevista asetuksista työtiedostojen suojaamiseksi laitteissa sekä asetuksista, jotka ohjaavat sitä, miten käyttäjät voivat käyttää Office-tiedostoja mobiililaitteilla.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-129">The following tables give detailed information about settings available to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="5d8a1-130">Lisätietoja on kohdassa Miten [Microsoft 365 Business Premiumin suojausominaisuudet liittyvät Intune-asetuksiin.](map-protection-features-to-intune-settings.md)</span><span class="sxs-lookup"><span data-stu-id="5d8a1-130">For more information, see [How do protection features in Microsoft 365 Business Premium map to Intune settings](map-protection-features-to-intune-settings.md).</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="5d8a1-131">Työtiedostojen suojaamisasetukset</span><span class="sxs-lookup"><span data-stu-id="5d8a1-131">Settings that protect work files</span></span>

<span data-ttu-id="5d8a1-132">Seuraavilla asetuksilla voidaan suojata työtiedostoja, jos käyttäjän laite katoaa tai varastetaan:</span><span class="sxs-lookup"><span data-stu-id="5d8a1-132">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="5d8a1-133">Asetus</span><span class="sxs-lookup"><span data-stu-id="5d8a1-133">Setting</span></span>  <br/> |<span data-ttu-id="5d8a1-134">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="5d8a1-134">Description</span></span>  <br/> |
|<span data-ttu-id="5d8a1-135">Poista työtiedostot passiivisesta laitteesta näin monen päivän kuluttua</span><span class="sxs-lookup"><span data-stu-id="5d8a1-135">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="5d8a1-136">Jos laitetta ei käytetä tässä määrittämääsi päivien lukumäärään, laitteeseen tallennetut työtiedostot poistetaan automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-136">If a device isn't used for the number of days that you specify here, any work files stored on the device will be deleted automatically.</span></span>  <br/> |
|<span data-ttu-id="5d8a1-137">Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin</span><span class="sxs-lookup"><span data-stu-id="5d8a1-137">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="5d8a1-138">Jos tämä asetus **on Käytössä,** työtiedostojen ainoa käytettävissä oleva tallennussijainti on OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-138">If this setting is **On**, the only available save location for work files is OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="5d8a1-139">Salaa työtiedostot</span><span class="sxs-lookup"><span data-stu-id="5d8a1-139">Encrypt work files</span></span>  <br/> |<span data-ttu-id="5d8a1-140">Pidä tämä asetus **käytössä**, jotta työtiedostot suojataan salauksella.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-140">Keep this setting **On** so that work files are protected by encryption.</span></span> <span data-ttu-id="5d8a1-141">Vaikka laite katoaa tai varastetaan, kukaan ei voi lukea yrityksesi tietoja.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-141">Even if the device is lost or stolen, no one can read your company data.</span></span>  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="5d8a1-142">Asetukset, joilla hallitaan käyttäjien Office-tiedostojen käyttöä mobiililaitteilla</span><span class="sxs-lookup"><span data-stu-id="5d8a1-142">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="5d8a1-143">Käyttäjien Office-työtiedostojen käyttöä voidaan hallita seuraavilla asetuksilla:</span><span class="sxs-lookup"><span data-stu-id="5d8a1-143">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="5d8a1-144">Asetus</span><span class="sxs-lookup"><span data-stu-id="5d8a1-144">Setting</span></span>  <br/> |<span data-ttu-id="5d8a1-145">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="5d8a1-145">Description</span></span>  <br/> |
|<span data-ttu-id="5d8a1-146">Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä</span><span class="sxs-lookup"><span data-stu-id="5d8a1-146">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="5d8a1-147">Jos tämä asetus **on käytössä,** käyttäjien on annettava toinen todennusmuoto käyttäjänimen ja salasanan lisäksi, ennen kuin he voivat käyttää Office-sovelluksia mobiililaitteissaan.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-147">If this setting is **On** users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile devices.</span></span><br/> |
|<span data-ttu-id="5d8a1-148">Palauta PIN-koodi, jos kirjautuminen epäonnistuu näin monta kertaa</span><span class="sxs-lookup"><span data-stu-id="5d8a1-148">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="5d8a1-149">Jos haluat estää luvatonta käyttäjä arvaamasta PIN-koodia sattumalta, PIN-koodi palautetaan määrittämäsi virheellisten syöttökertojen määrän jälkeen.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-149">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="5d8a1-150">Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä</span><span class="sxs-lookup"><span data-stu-id="5d8a1-150">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="5d8a1-151">Tämä asetus määrittää, kuinka kauan käyttäjä voi olla käyttämättömänä, ennen kuin häntä pyydetään kirjautumaan uudelleen sisään.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-151">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="5d8a1-152">Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu</span><span class="sxs-lookup"><span data-stu-id="5d8a1-152">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="5d8a1-p105">Kekseliäällä käyttäjällä voi olla laite, jonka suojaus on murrettu. Tämä tarkoittaa, että käyttäjä voi muokata käyttöjärjestelmää, minkä vuoksi laite voi altistua helpommin haittaohjelmille. Tällaiset laitteet on estetty, kun tämä asetus on **käytössä**.  </span><span class="sxs-lookup"><span data-stu-id="5d8a1-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="5d8a1-156">Älä salli käyttäjien kopioida sisältöä Office-sovelluksista henkilökohtaisiin sovelluksiin</span><span class="sxs-lookup"><span data-stu-id="5d8a1-156">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="5d8a1-157">Oletuksena tätä ei sallita, mutta jos asetus on **käytössä**, käyttäjä voi kopioida työtiedoston tietoja henkilökohtaiseen tiedostoon.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-157">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="5d8a1-158">Jos asetuksena on **Ei käytössä**, käyttäjä ei voi kopioida tietoja työtilistä henkilökohtaiseen sovellukseen tai henkilökohtaisen tiliin.</span><span class="sxs-lookup"><span data-stu-id="5d8a1-158">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
