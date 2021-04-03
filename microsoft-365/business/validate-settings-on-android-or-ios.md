---
title: Sovellusten suojausasetusten vahvistaminen Android- tai iOS-laitteissa
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: Lue, miten voit vahvistaa Microsoft 365 Business Premium -sovelluksen suojausasetukset Android- tai iOS-laitteissasi.
ms.openlocfilehash: a0a4a6e6cff59f66a506929e97c99d361472a68b
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578063"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="5d7b2-103">Sovellusten suojausasetusten vahvistaminen Android- tai iOS-laitteissa</span><span class="sxs-lookup"><span data-stu-id="5d7b2-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="5d7b2-104">Vahvista sovellusten suojausasetukset Android- tai iOS-laitteissa seuraavien osioiden ohjeiden mukaisesti.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-104">Follow the instructions in the following sections to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="android"></a><span data-ttu-id="5d7b2-105">Android</span><span class="sxs-lookup"><span data-stu-id="5d7b2-105">Android</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="5d7b2-106">Tarkista, että sovellusten suojausasetukset toimivat käyttäjien laitteissa</span><span class="sxs-lookup"><span data-stu-id="5d7b2-106">Check that the app protection settings are working on user devices</span></span>

<span data-ttu-id="5d7b2-107">Kun olet [määrittänyt Android-laitteiden sovellusasetukset](app-protection-settings-for-android-and-ios.md) sovellusten suojaamista varten, seuraavien ohjeiden avulla voit vahvistaa, että valitsemasi asetukset toimivat.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="5d7b2-108">Varmista ensin, että käytäntö koskee sovellusta, jossa aiot vahvistaa sen.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-108">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="5d7b2-109">Valitse Microsoft 365 Business Premium [-hallintakeskuksessa](https://portal.office.com) **Käytäntöjen** \> **muokkauskäytäntö.**</span><span class="sxs-lookup"><span data-stu-id="5d7b2-109">In the Microsoft 365 Business Premium [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="5d7b2-110">Valitse **Androidin sovelluskäytäntö** asetuksissa, jotka olet luonut määrityksen yhteydessä, tai jokin muu luomasi käytäntö, ja varmista, että se on esimerkiksi pakotettu Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook, for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](../media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="5d7b2-112">Vahvista, että Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä</span><span class="sxs-lookup"><span data-stu-id="5d7b2-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="5d7b2-113">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä** on **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Varmista, että Office-sovellusten käyttäminen Edellyttää PIN-koodia tai sormenjälkeä -asetuksena on Käytössä.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="5d7b2-115">Avaa Outlook käyttäjän Android-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business Premium -tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="5d7b2-116">Sinua pyydetään myös antamaan PIN-koodi tai käyttämään sormenjälkeä.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-116">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](../media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="5d7b2-118">Vahvista Palauta PIN-koodi, kun on tehty tämä määrä epäonnistuneita yrityksiä</span><span class="sxs-lookup"><span data-stu-id="5d7b2-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="5d7b2-119">Valitse **Muokkaa** käytäntöä  -ruudussa **Muokkaa Office-tiedostojen** käytön hallinnan vieressä, laajenna Hallitse käyttäjien Office-tiedostojen käyttöä mobiililaitteissa ja varmista, että **PALAUTA PIN-koodi,** kun epäonnistuneita yrityksiä **on** määritetty joksikin määräksi.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="5d7b2-120">Tämä on oletusarvoisesti 5.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-120">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="5d7b2-121">Avaa Outlook käyttäjän Android-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business Premium -tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-121">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="5d7b2-122">Kirjoita virheellinen PIN-koodi niin monta kertaa kuin käytäntö määrittää.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-122">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="5d7b2-123">Näyttöön tulee kehote, jossa pyydetään, että **PIN-koodin palautusyritysrajoitus** on saavutettu.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-123">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="5d7b2-125">Paina **Palauta PIN-koodi**.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-125">Press **Reset PIN**.</span></span> <span data-ttu-id="5d7b2-126">Sinua pyydetään kirjautumaan sisään käyttäjän Microsoft 365 Business Premium -tunnistetiedoilla ja määrittämään uusi PIN-koodi.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-126">You'll be prompted to sign in with the user's Microsoft 365 Business Premium credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="5d7b2-127">Vahvista Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin</span><span class="sxs-lookup"><span data-stu-id="5d7b2-127">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="5d7b2-128">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** on **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-128">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="5d7b2-130">Avaa Outlook käyttäjän Android-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business Premium -tunnistetiedoilla ja anna TARVITTAESSA PIN-koodi.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-130">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="5d7b2-131">Avaa sähköpostiviesti, jossa on liite, ja valitse liitteen tietojen vieressä oleva alanuolikuva.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-131">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](../media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="5d7b2-133">Näytön alareunassa **näkyy Ei voi tallentaa** laitteeseen -kohta.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-133">You'll see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](../media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="5d7b2-135">Tallentaminen OneDrive for Businessiin ei ole käytössä Androidissa tällä hetkellä, joten näet vain, että tallentaminen paikallisesti on estetty.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-135">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="5d7b2-136">Vahvista Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä määritetyn ajan</span><span class="sxs-lookup"><span data-stu-id="5d7b2-136">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="5d7b2-137">Valitse **Muokkaa** käytäntöä  -ruudussa **Muokkaa Office-tiedostojen** käytön hallinta -kohdan vieressä, laajenna Hallitse käyttäjien **Office-tiedostojen** käyttöä mobiililaitteissa ja varmista, että Edellytä, että käyttäjät kirjautuvat uudelleen, kun **Office-sovellukset** ovat olleet käyttämättömänä, on määritetty joitakin minuutteja.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-137">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="5d7b2-138">Tämä on oletusarvoisesti 30 minuuttia.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-138">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="5d7b2-139">Avaa Outlook käyttäjän Android-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business Premium -tunnistetiedoilla ja anna TARVITTAESSA PIN-koodi.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-139">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="5d7b2-p105">Outlookin Saapuneet-kansion pitäisi nyt näkyä. Älä koske Android-laitteeseen vähintään 30 minuuttiin (tai muun käytäntöön määrittämääsi aikaa pidemmän ajan). Todennäköisesti laitteen näyttö himmenee.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-p105">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="5d7b2-143">Käytä Outlookia uudelleen Android-laitteessa.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-143">Access Outlook on the Android device again.</span></span>
    
4. <span data-ttu-id="5d7b2-144">Sinua pyydetään antamaan PIN-koodi, ennen kuin voit käyttää Outlookia uudelleen.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-144">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="5d7b2-145">Vahvista Suojaa työtiedostot salauksella</span><span class="sxs-lookup"><span data-stu-id="5d7b2-145">Validate Protect work files with encryption</span></span>

<span data-ttu-id="5d7b2-146">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Suojaa työtiedostot salauksella** on **käytössä** ja **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** **pois käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-146">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="5d7b2-147">Avaa Outlook käyttäjän Android-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business Premium -tunnistetiedoilla ja anna TARVITTAESSA PIN-koodi.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-147">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="5d7b2-148">Avaa sähköpostiviesti, joka sisältää muutaman kuvatiedoston liitetiedoston.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-148">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="5d7b2-149">Voit tallentaa liitteen valitsemalla sen tietojen vieressä olevan alanuolikuvakkeen.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-149">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](../media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="5d7b2-p106">Näyttöön voi tulla pyyntö sallia Outlookin käyttää laitteessa olevia valokuvia, mediatiedostoja ja muita tiedostoja. Valitse **Salli**.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-p106">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="5d7b2-153">Valitse **Tallenna laitteeseen** näytön alareunassa ja avaa sitten **Galleria** -sovellus.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-153">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="5d7b2-p107">Luettelossa pitäisi näkyä salattu valokuva (tai useita, jos tallensit useita kuvatiedostoliitteitä). Se voi näkyä Kuvat-luettelossa harmaana ruutuna, jonka keskellä on valkoisen ympyrän sisällä oleva valkoinen huutomerkki.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-p107">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](../media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="ios"></a><span data-ttu-id="5d7b2-157">iOS</span><span class="sxs-lookup"><span data-stu-id="5d7b2-157">iOS</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="5d7b2-158">Sovellusten suojausasetusten toiminnan varmistaminen käyttäjien laitteissa</span><span class="sxs-lookup"><span data-stu-id="5d7b2-158">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="5d7b2-159">Kun olet [määrittänyt iOS-laitteiden sovellusasetukset](app-protection-settings-for-android-and-ios.md) sovellusten suojaamista varten, seuraavien ohjeiden avulla voit vahvistaa, että valitsemasi asetukset toimivat.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-159">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="5d7b2-160">Varmista ensin, että käytäntö koskee sovellusta, jossa aiot vahvistaa sen.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-160">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="5d7b2-161">Valitse Microsoft 365 Business Premium [-hallintakeskuksessa](https://portal.office.com) **Käytäntöjen** \> **muokkauskäytäntö.**</span><span class="sxs-lookup"><span data-stu-id="5d7b2-161">In the Microsoft 365 Business Premium [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="5d7b2-162">Valitse **iOS:n** sovelluskäytäntö asetuksissa, jotka olet luonut määrityksen yhteydessä, tai jokin muu luomasi käytäntö, ja varmista, että se on esimerkiksi pakotettu Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-162">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](../media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="5d7b2-164">Vahvista Office-sovellusten käyttäminen edellyttää PIN-koodia</span><span class="sxs-lookup"><span data-stu-id="5d7b2-164">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="5d7b2-165">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä** on **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-165">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Varmista, että Office-sovellusten käyttäminen Edellyttää PIN-koodia tai sormenjälkeä -asetuksena on Käytössä.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="5d7b2-167">Avaa Outlook käyttäjän iOS-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business Premium -tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-167">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="5d7b2-168">Sinua pyydetään myös antamaan PIN-koodi tai käyttämään sormenjälkeä.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-168">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](../media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="5d7b2-170">Vahvista Palauta PIN-koodi, kun on tehty tämä määrä epäonnistuneita yrityksiä</span><span class="sxs-lookup"><span data-stu-id="5d7b2-170">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="5d7b2-171">Valitse **Muokkaa** käytäntöä  -ruudussa **Muokkaa Office-tiedostojen** käytön hallinnan vieressä, laajenna Hallitse käyttäjien Office-tiedostojen käyttöä mobiililaitteissa ja varmista, että **PALAUTA PIN-koodi,** kun epäonnistuneita yrityksiä **on** määritetty joksikin määräksi.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-171">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="5d7b2-172">Tämä on oletusarvoisesti 5.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-172">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="5d7b2-173">Avaa Outlook käyttäjän iOS-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business Premium -tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-173">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="5d7b2-174">Kirjoita virheellinen PIN-koodi niin monta kertaa kuin käytäntö määrittää.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-174">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="5d7b2-175">Näyttöön tulee kehote, jossa pyydetään, että **PIN-koodin palautusyritysrajoitus** on saavutettu.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-175">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="5d7b2-177">Paina **OK**.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-177">Press **OK**.</span></span> <span data-ttu-id="5d7b2-178">Sinua pyydetään kirjautumaan sisään käyttäjän Microsoft 365 Business Premium -tunnistetiedoilla ja määrittämään uusi PIN-koodi.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-178">You'll be prompted to sign in with the user's Microsoft 365 Business Premium credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="5d7b2-179">Vahvista Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin</span><span class="sxs-lookup"><span data-stu-id="5d7b2-179">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="5d7b2-180">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** on **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-180">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="5d7b2-182">Avaa Outlook käyttäjän iOS-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business Premium -tunnistetiedoilla ja anna TARVITTAESSA PIN-koodi.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-182">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="5d7b2-183">Avaa liitteen sisältävä sähköpostiviesti, avaa liite ja valitse **Tallenna** näytön alareunassa.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-183">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](../media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="5d7b2-185">Näkyvissä pitäisi olla vaihtoehto vain OneDrive for Businessille.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-185">You should only see an option for OneDrive for Business.</span></span> <span data-ttu-id="5d7b2-186">Jos näin ei ole, valitse **Lisää tili** ja valitse Lisää **tallennustilatili** -näytössä **OneDrive for Business.**</span><span class="sxs-lookup"><span data-stu-id="5d7b2-186">If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen.</span></span> <span data-ttu-id="5d7b2-187">Anna loppukäyttäjän Microsoft 365 Business Premium kirjautuaksesi sisään pyydettäessä.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-187">Provide the end user's Microsoft 365 Business Premium to sign in when prompted.</span></span> 
    
    <span data-ttu-id="5d7b2-188">Napauta **Tallenna** ja valitse **OneDrive for Business**.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-188">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="5d7b2-189">Vahvista Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä määritetyn ajan</span><span class="sxs-lookup"><span data-stu-id="5d7b2-189">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="5d7b2-190">Valitse **Muokkaa** käytäntöä  -ruudussa **Muokkaa Office-tiedostojen** käytön hallinta -kohdan vieressä, laajenna Hallitse käyttäjien **Office-tiedostojen** käyttöä mobiililaitteissa ja varmista, että Edellytä, että käyttäjät kirjautuvat uudelleen, kun **Office-sovellukset** ovat olleet käyttämättömänä, on määritetty joitakin minuutteja.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-190">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="5d7b2-191">Tämä on oletusarvoisesti 30 minuuttia.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-191">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="5d7b2-192">Avaa Outlook käyttäjän iOS-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business Premium -tunnistetiedoilla ja anna TARVITTAESSA PIN-koodi.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-192">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="5d7b2-p113">Outlookin Saapuneet-kansion pitäisi nyt näkyä. Älä koske iOS-laitteeseen vähintään 30 minuuttiin (tai muun käytäntöön määrittämääsi aikaa pidemmän ajan). Todennäköisesti laitteen näyttö himmenee.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-p113">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="5d7b2-196">Käytä Outlookia uudelleen iOS-laitteessa.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-196">Access Outlook on the iOS device again.</span></span>
    
4. <span data-ttu-id="5d7b2-197">Sinua pyydetään antamaan PIN-koodi, ennen kuin voit käyttää Outlookia uudelleen.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-197">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="5d7b2-198">Vahvista Suojaa työtiedostot salauksella</span><span class="sxs-lookup"><span data-stu-id="5d7b2-198">Validate Protect work files with encryption</span></span>

<span data-ttu-id="5d7b2-199">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Suojaa työtiedostot salauksella** on **käytössä** ja **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** **pois käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-199">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="5d7b2-200">Avaa Outlook käyttäjän iOS-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business Premium -tunnistetiedoilla ja anna TARVITTAESSA PIN-koodi.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-200">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="5d7b2-201">Avaa sähköpostiviesti, joka sisältää muutaman kuvatiedoston liitetiedoston.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-201">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="5d7b2-202">Napauta liitettä ja **Tallenna**-vaihtoehtoa sen alla.</span><span class="sxs-lookup"><span data-stu-id="5d7b2-202">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="5d7b2-p114">Avaa **Valokuvat**-sovellus aloitusnäytössä. Näkyviin tulee tallennettu mutta salattu valokuva (tai useampia, jos tallensit useita kuvatiedostoliitteitä).</span><span class="sxs-lookup"><span data-stu-id="5d7b2-p114">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---

