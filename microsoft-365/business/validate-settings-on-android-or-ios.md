---
title: Tarkista suojausasetukset app Android tai iOS-laitteissa
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: 'Learn how to validate the Microsoft 365 Business app protection settings in your Android or iOS devices.  '
ms.openlocfilehash: 300f59e81a93cc3dfc03fd1d98891be1ac4f7795
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983673"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="01da9-103">Tarkista suojausasetukset app Android tai iOS-laitteissa</span><span class="sxs-lookup"><span data-stu-id="01da9-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="01da9-104">Tarkista suojausasetukset app Android tai iOS-laitteissa välilehdet ohjeiden mukaan.</span><span class="sxs-lookup"><span data-stu-id="01da9-104">Follow the instructions in the tabs to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="androidtab"></a>[<span data-ttu-id="01da9-105">Android</span><span class="sxs-lookup"><span data-stu-id="01da9-105">Android</span></span>](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="01da9-106">Sovellusten suojausasetusten toiminnan varmistaminen käyttäjien laitteissa</span><span class="sxs-lookup"><span data-stu-id="01da9-106">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="01da9-107">Kun olet [määrittänyt Android-laitteiden sovellusasetukset](app-protection-settings-for-android-and-ios.md) sovellusten suojaamista varten, seuraavien ohjeiden avulla voit vahvistaa, että valitsemasi asetukset toimivat.</span><span class="sxs-lookup"><span data-stu-id="01da9-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="01da9-108">Varmista ensin, että käytäntö koskee sovellusta, jossa aiot vahvistaa sen.</span><span class="sxs-lookup"><span data-stu-id="01da9-108">First, make sure that the policy applies to the app in which you are going to validate it.</span></span>
  
1. <span data-ttu-id="01da9-109">Siirry Microsoft 365 Businessin [hallintakeskuksessa](https://portal.office.com) kohtaan **Käytännöt** \> **Muokkaa käytäntöä**.</span><span class="sxs-lookup"><span data-stu-id="01da9-109">In the Microsoft 365 Business [admin center](https://portal.office.com) go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="01da9-110">Valitse **Androidin sovelluskäytäntö** asennuksen aikana luomillesi asetuksille tai toinen luomasi käytäntö ja varmista, että se on käytössä esimerkiksi Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="01da9-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it is enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="01da9-112">Vahvista, että Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä</span><span class="sxs-lookup"><span data-stu-id="01da9-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="01da9-113">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä** on **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="01da9-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="01da9-115">Avaa Outlook käyttäjän Android-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="01da9-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="01da9-116">Sinua pyydetään myös antamaan PIN-koodi tai käyttämään sormenjälkeä.</span><span class="sxs-lookup"><span data-stu-id="01da9-116">You will also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="01da9-118">Vahvista Palauta PIN-koodi, kun on tehty tämä määrä epäonnistuneita yrityksiä</span><span class="sxs-lookup"><span data-stu-id="01da9-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="01da9-119">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Palauta PIN-koodi, kun on tehty tämä määrä epäonnistuneita yrityksiä** -kohtaan on määritetty jokin luku. Oletusarvo on 5.</span><span class="sxs-lookup"><span data-stu-id="01da9-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number - this is 5 by default.</span></span> 
  
1. <span data-ttu-id="01da9-120">Avaa Outlook käyttäjän Android-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="01da9-120">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="01da9-p101">Kirjoita virheellinen PIN-koodi niin monta kertaa kuin käytäntö määrittää. Näyttöön tulee kehote, jossa ilmoitetaan **PIN-koodin syöttöyritysten rajoitus saavutettiin** ja pyydetään palauttamaan PIN-koodi.</span><span class="sxs-lookup"><span data-stu-id="01da9-p101">Enter an incorrect PIN as many times as specified by the policy. You will see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="01da9-p102">Paina **Palauta PIN-koodi**. Sinua pyydetään kirjautumaan sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja määrittämään uusi PIN-koodi.</span><span class="sxs-lookup"><span data-stu-id="01da9-p102">Press **Reset PIN**. You will be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="01da9-126">Vahvista Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin</span><span class="sxs-lookup"><span data-stu-id="01da9-126">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="01da9-127">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** on **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="01da9-127">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="01da9-129">Avaa Outlook käyttäjän Android-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.</span><span class="sxs-lookup"><span data-stu-id="01da9-129">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="01da9-130">Avaa sähköpostiviesti, jossa on liite, ja valitse liitteen tietojen vieressä oleva alanuolikuva.</span><span class="sxs-lookup"><span data-stu-id="01da9-130">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="01da9-132">Näytön alareunassa näkyy sanoma **Laitteeseen ei voi tallentaa**.</span><span class="sxs-lookup"><span data-stu-id="01da9-132">You will see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="01da9-134">Tallentaminen OneDrive for Businessiin ei ole käytössä Androidissa tällä hetkellä, joten näet vain, että tallentaminen paikallisesti on estetty.</span><span class="sxs-lookup"><span data-stu-id="01da9-134">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="01da9-135">Vahvista Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä määritetyn ajan</span><span class="sxs-lookup"><span data-stu-id="01da9-135">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="01da9-136">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä** -kohtaan on määritetty jokin luku. Oletusarvo on 30 minuuttia.</span><span class="sxs-lookup"><span data-stu-id="01da9-136">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes - this is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="01da9-137">Avaa Outlook käyttäjän Android-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.</span><span class="sxs-lookup"><span data-stu-id="01da9-137">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="01da9-p103">Outlookin Saapuneet-kansion pitäisi nyt näkyä. Älä koske Android-laitteeseen vähintään 30 minuuttiin (tai muun käytäntöön määrittämääsi aikaa pidemmän ajan). Todennäköisesti laitteen näyttö himmenee.</span><span class="sxs-lookup"><span data-stu-id="01da9-p103">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="01da9-141">Avaa Outlook uudelleen Android-laitteessa.</span><span class="sxs-lookup"><span data-stu-id="01da9-141">Re-access Outlook on the Android device.</span></span>
    
4. <span data-ttu-id="01da9-142">Sinua pyydetään antamaan PIN-koodi, ennen kuin voit käyttää Outlookia uudelleen.</span><span class="sxs-lookup"><span data-stu-id="01da9-142">You will be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="01da9-143">Vahvista Suojaa työtiedostot salauksella</span><span class="sxs-lookup"><span data-stu-id="01da9-143">Validate Protect work files with encryption</span></span>

<span data-ttu-id="01da9-144">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Suojaa työtiedostot salauksella** on **käytössä** ja **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** **pois käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="01da9-144">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="01da9-145">Avaa Outlook käyttäjän Android-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.</span><span class="sxs-lookup"><span data-stu-id="01da9-145">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="01da9-146">Avaa sähköpostiviesti, joka sisältää muutaman kuvatiedostoliitteen.</span><span class="sxs-lookup"><span data-stu-id="01da9-146">Open an email which contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="01da9-147">Voit tallentaa liitteen valitsemalla sen tietojen vieressä olevan alanuolikuvakkeen.</span><span class="sxs-lookup"><span data-stu-id="01da9-147">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="01da9-p104">Näyttöön voi tulla pyyntö sallia Outlookin käyttää laitteessa olevia valokuvia, mediatiedostoja ja muita tiedostoja. Valitse **Salli**.</span><span class="sxs-lookup"><span data-stu-id="01da9-p104">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="01da9-151">Valitse **Tallenna laitteeseen** näytön alareunassa ja avaa sitten **Galleria** -sovellus.</span><span class="sxs-lookup"><span data-stu-id="01da9-151">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="01da9-p105">Luettelossa pitäisi näkyä salattu valokuva (tai useita, jos tallensit useita kuvatiedostoliitteitä). Se voi näkyä Kuvat-luettelossa harmaana ruutuna, jonka keskellä on valkoisen ympyrän sisällä oleva valkoinen huutomerkki.</span><span class="sxs-lookup"><span data-stu-id="01da9-p105">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="iostab"></a>[<span data-ttu-id="01da9-155">iOS</span><span class="sxs-lookup"><span data-stu-id="01da9-155">iOS</span></span>](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="01da9-156">Sovellusten suojausasetusten toiminnan varmistaminen käyttäjien laitteissa</span><span class="sxs-lookup"><span data-stu-id="01da9-156">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="01da9-157">Kun olet [määrittänyt iOS-laitteiden sovellusasetukset](app-protection-settings-for-android-and-ios.md) sovellusten suojaamista varten, seuraavien ohjeiden avulla voit vahvistaa, että valitsemasi asetukset toimivat.</span><span class="sxs-lookup"><span data-stu-id="01da9-157">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="01da9-158">Varmista ensin, että käytäntö koskee sovellusta, jossa aiot vahvistaa sen.</span><span class="sxs-lookup"><span data-stu-id="01da9-158">First, make sure that the policy applies to the app in which you are going to validate it.</span></span>
  
1. <span data-ttu-id="01da9-159">Siirry Microsoft 365 Businessin [hallintakeskuksessa](https://portal.office.com) kohtaan **Käytännöt** \> **Muokkaa käytäntöä**.</span><span class="sxs-lookup"><span data-stu-id="01da9-159">In the Microsoft 365 Business [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="01da9-160">Valitse **iOS:n sovelluskäytäntö** asennuksen aikana luomillesi asetuksille tai toinen luomasi käytäntö ja varmista, että se on käytössä esimerkiksi Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="01da9-160">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it is enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="01da9-162">Vahvista Office-sovellusten käyttäminen edellyttää PIN-koodia</span><span class="sxs-lookup"><span data-stu-id="01da9-162">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="01da9-163">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä** on **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="01da9-163">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="01da9-165">Avaa Outlook käyttäjän iOS-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="01da9-165">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="01da9-166">Sinua pyydetään myös antamaan PIN-koodi tai käyttämään sormenjälkeä.</span><span class="sxs-lookup"><span data-stu-id="01da9-166">You will also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="01da9-168">Vahvista Palauta PIN-koodi, kun on tehty tämä määrä epäonnistuneita yrityksiä</span><span class="sxs-lookup"><span data-stu-id="01da9-168">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="01da9-169">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Palauta PIN-koodi, kun on tehty tämä määrä epäonnistuneita yrityksiä** -kohtaan on määritetty jokin luku. Oletusarvo on 5.</span><span class="sxs-lookup"><span data-stu-id="01da9-169">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number - this is 5 by default.</span></span> 
  
1. <span data-ttu-id="01da9-170">Avaa Outlook käyttäjän iOS-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="01da9-170">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="01da9-p106">Kirjoita virheellinen PIN-koodi niin monta kertaa kuin käytäntö määrittää. Näyttöön tulee kehote, jossa ilmoitetaan **PIN-koodin syöttöyritysten rajoitus saavutettiin** ja pyydetään palauttamaan PIN-koodi.</span><span class="sxs-lookup"><span data-stu-id="01da9-p106">Enter an incorrect PIN as many times as specified by the policy. You will see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="01da9-p107">Paina **OK**. Sinua pyydetään kirjautumaan sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja määrittämään uusi PIN-koodi.</span><span class="sxs-lookup"><span data-stu-id="01da9-p107">Press **OK**. You will be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="01da9-176">Vahvista Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin</span><span class="sxs-lookup"><span data-stu-id="01da9-176">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="01da9-177">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** on **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="01da9-177">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="01da9-179">Avaa Outlook käyttäjän iOS-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.</span><span class="sxs-lookup"><span data-stu-id="01da9-179">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="01da9-180">Avaa liitteen sisältävä sähköpostiviesti, avaa liite ja valitse **Tallenna** näytön alareunassa.</span><span class="sxs-lookup"><span data-stu-id="01da9-180">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="01da9-p108">Näkyvissä pitäisi olla vaihtoehto vain OneDrive for Businessille. Jos näin ei ole, napauta **Lisää tili** ja valitse **OneDrive for Business** **Lisää tallennustilatili** -näytössä. Kirjaudu sisään käyttäjän Microsoft 365 Business -tiedoilla kehotettaessa.</span><span class="sxs-lookup"><span data-stu-id="01da9-p108">You should only see an option for OneDrive for Business. If not If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen. Provide the end user's Microsoft 365 Business to sign in when prompted.</span></span> 
    
    <span data-ttu-id="01da9-185">Napauta **Tallenna** ja valitse **OneDrive for Business**.</span><span class="sxs-lookup"><span data-stu-id="01da9-185">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="01da9-186">Vahvista Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä määritetyn ajan</span><span class="sxs-lookup"><span data-stu-id="01da9-186">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="01da9-187">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä** -kohtaan on määritetty jokin luku. Oletusarvo on 30 minuuttia.</span><span class="sxs-lookup"><span data-stu-id="01da9-187">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes - this is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="01da9-188">Avaa Outlook käyttäjän iOS-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.</span><span class="sxs-lookup"><span data-stu-id="01da9-188">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="01da9-p109">Outlookin Saapuneet-kansion pitäisi nyt näkyä. Älä koske iOS-laitteeseen vähintään 30 minuuttiin (tai muun käytäntöön määrittämääsi aikaa pidemmän ajan). Todennäköisesti laitteen näyttö himmenee.</span><span class="sxs-lookup"><span data-stu-id="01da9-p109">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="01da9-192">Avaa Outlook uudelleen iOS-laitteessa.</span><span class="sxs-lookup"><span data-stu-id="01da9-192">Re-access Outlook on the iOS device.</span></span>
    
4. <span data-ttu-id="01da9-193">Sinua pyydetään antamaan PIN-koodi, ennen kuin voit käyttää Outlookia uudelleen.</span><span class="sxs-lookup"><span data-stu-id="01da9-193">You will be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="01da9-194">Vahvista Suojaa työtiedostot salauksella</span><span class="sxs-lookup"><span data-stu-id="01da9-194">Validate Protect work files with encryption</span></span>

<span data-ttu-id="01da9-195">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Suojaa työtiedostot salauksella** on **käytössä** ja **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** **pois käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="01da9-195">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="01da9-196">Avaa Outlook käyttäjän iOS-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.</span><span class="sxs-lookup"><span data-stu-id="01da9-196">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="01da9-197">Avaa sähköpostiviesti, joka sisältää muutaman kuvatiedostoliitteen.</span><span class="sxs-lookup"><span data-stu-id="01da9-197">Open an email which contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="01da9-198">Napauta liitettä ja **Tallenna**-vaihtoehtoa sen alla.</span><span class="sxs-lookup"><span data-stu-id="01da9-198">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="01da9-p110">Avaa **Valokuvat**-sovellus aloitusnäytössä. Näkyviin tulee tallennettu mutta salattu valokuva (tai useampia, jos tallensit useita kuvatiedostoliitteitä).</span><span class="sxs-lookup"><span data-stu-id="01da9-p110">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---

