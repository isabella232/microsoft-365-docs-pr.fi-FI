---
title: Vahvista sovellusten suojaus asetukset Android-tai iOS-laitteilla
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: Learn how to validate the Microsoft 365 Business app protection settings in your Android or iOS devices.
ms.openlocfilehash: 47ce137f785c595992886c756ad85b80957272fe
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594971"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="d03dd-103">Vahvista sovellusten suojaus asetukset Android-tai iOS-laitteilla</span><span class="sxs-lookup"><span data-stu-id="d03dd-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="d03dd-104">Tarkista sovellusten suojaus asetukset Android-tai iOS-laitteissa noudattamalla seuraavien osien ohjeita.</span><span class="sxs-lookup"><span data-stu-id="d03dd-104">Follow the instructions in the following sections to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="android"></a><span data-ttu-id="d03dd-105">Android</span><span class="sxs-lookup"><span data-stu-id="d03dd-105">Android</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="d03dd-106">Tarkista, että sovelluksen suojaus asetukset toimivat käyttäjä laitteilla</span><span class="sxs-lookup"><span data-stu-id="d03dd-106">Check that the app protection settings are working on user devices</span></span>

<span data-ttu-id="d03dd-107">Kun olet [määrittänyt Android-laitteiden sovellusasetukset](app-protection-settings-for-android-and-ios.md) sovellusten suojaamista varten, seuraavien ohjeiden avulla voit vahvistaa, että valitsemasi asetukset toimivat.</span><span class="sxs-lookup"><span data-stu-id="d03dd-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="d03dd-108">Varmista ensin, että käytäntö koskee sovellusta, jossa aiot tarkistaa sen.</span><span class="sxs-lookup"><span data-stu-id="d03dd-108">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="d03dd-109">Siirry Microsoft 365 Businessin [hallintakeskuksessa](https://portal.office.com) kohtaan **Käytännöt** \> **Muokkaa käytäntöä**.</span><span class="sxs-lookup"><span data-stu-id="d03dd-109">In the Microsoft 365 Business [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="d03dd-110">Valitse **Androidille sovellus käytäntö** asetuksille, jotka olet luonut asetukset-sovelluksessa, tai toinen luomasi käytäntö ja varmista, että se on käytössä esimerkiksi Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="d03dd-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook, for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="d03dd-112">Vahvista, että Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä</span><span class="sxs-lookup"><span data-stu-id="d03dd-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="d03dd-113">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä** on **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="d03dd-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Varmista, että vaadi PIN-koodi tai sormen jälki Office-sovellusten käyttöön on käytössä.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="d03dd-115">Avaa Outlook käyttäjän Android-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="d03dd-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="d03dd-116">Sinua pyydetään myös syöttämään PIN-koodi tai käyttämään sormen jälkeä.</span><span class="sxs-lookup"><span data-stu-id="d03dd-116">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="d03dd-118">Vahvista Palauta PIN-koodi, kun on tehty tämä määrä epäonnistuneita yrityksiä</span><span class="sxs-lookup"><span data-stu-id="d03dd-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="d03dd-119">Valitse **Muokkaa käytäntöä** -ruudussa **Office-asia kirjojen käyttö oikeus-ohjaus objektin**vieressä **Muokkaa** , Laajenna **Hallitse, miten käyttäjät voivat käyttää Office-tiedostoja mobiililaitteilla**, ja varmista, että **Palauta PIN-koodin jälkeen epäonnistuneiden yritysten määrä** on asetettu johonkin numeroon.</span><span class="sxs-lookup"><span data-stu-id="d03dd-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="d03dd-120">Tämä on oletusarvoisesti 5.</span><span class="sxs-lookup"><span data-stu-id="d03dd-120">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="d03dd-121">Avaa Outlook käyttäjän Android-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="d03dd-121">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="d03dd-122">Kirjoita virheellinen PIN-koodi niin monta kertaa kuin käytäntö määrittää.</span><span class="sxs-lookup"><span data-stu-id="d03dd-122">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="d03dd-123">Näkyviin tulee kehote, joka **antaa PIN-** koodin nollaamiseen.</span><span class="sxs-lookup"><span data-stu-id="d03dd-123">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="d03dd-125">Paina **Palauta PIN-koodi**.</span><span class="sxs-lookup"><span data-stu-id="d03dd-125">Press **Reset PIN**.</span></span> <span data-ttu-id="d03dd-126">Sinua pyydetään Kirjautu maan sisään käyttäjän Microsoft 365-yrityksen tunniste tiedoilla ja asettamaan sitten uusi PIN-koodi.</span><span class="sxs-lookup"><span data-stu-id="d03dd-126">You'll be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="d03dd-127">Vahvista Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin</span><span class="sxs-lookup"><span data-stu-id="d03dd-127">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="d03dd-128">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** on **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="d03dd-128">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="d03dd-130">Avaa Outlook käyttäjän Android-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.</span><span class="sxs-lookup"><span data-stu-id="d03dd-130">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="d03dd-131">Avaa sähköpostiviesti, jossa on liite, ja valitse liitteen tietojen vieressä oleva alanuolikuva.</span><span class="sxs-lookup"><span data-stu-id="d03dd-131">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="d03dd-133">Näytön alalaidassa **ei voi tallentaa laitteeseen** .</span><span class="sxs-lookup"><span data-stu-id="d03dd-133">You'll see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="d03dd-135">Tallentaminen OneDrive for Businessiin ei ole käytössä Androidissa tällä hetkellä, joten näet vain, että tallentaminen paikallisesti on estetty.</span><span class="sxs-lookup"><span data-stu-id="d03dd-135">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="d03dd-136">Vahvista Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä määritetyn ajan</span><span class="sxs-lookup"><span data-stu-id="d03dd-136">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="d03dd-137">Valitse **Muokkaa käytäntöä** -ruudussa **Office-asia kirjojen käyttö oikeus-ohjaus objektin**vieressä **Muokkaa** , Laajenna **Hallitse, miten käyttäjät voivat käyttää Office-tiedostoja mobiililaitteilla**, ja varmista, että edellytä, että **käyttäjät kirjautuvat uudelleen sisään, kun Office-sovellukset ovat olleet käyttämättömänä** , on asetettu joihinkin minuutteihin.</span><span class="sxs-lookup"><span data-stu-id="d03dd-137">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="d03dd-138">Tämä on oletusarvoisesti 30 minuuttia.</span><span class="sxs-lookup"><span data-stu-id="d03dd-138">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="d03dd-139">Avaa Outlook käyttäjän Android-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.</span><span class="sxs-lookup"><span data-stu-id="d03dd-139">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="d03dd-p105">Outlookin Saapuneet-kansion pitäisi nyt näkyä. Älä koske Android-laitteeseen vähintään 30 minuuttiin (tai muun käytäntöön määrittämääsi aikaa pidemmän ajan). Todennäköisesti laitteen näyttö himmenee.</span><span class="sxs-lookup"><span data-stu-id="d03dd-p105">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="d03dd-143">Avaa Outlook uudelleen Android-laitteella.</span><span class="sxs-lookup"><span data-stu-id="d03dd-143">Access Outlook on the Android device again.</span></span>
    
4. <span data-ttu-id="d03dd-144">Sinua pyydetään antamaan PIN-koodi, ennen kuin voit käyttää Outlookia uudelleen.</span><span class="sxs-lookup"><span data-stu-id="d03dd-144">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="d03dd-145">Vahvista Suojaa työtiedostot salauksella</span><span class="sxs-lookup"><span data-stu-id="d03dd-145">Validate Protect work files with encryption</span></span>

<span data-ttu-id="d03dd-146">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Suojaa työtiedostot salauksella** on **käytössä** ja **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** **pois käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="d03dd-146">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="d03dd-147">Avaa Outlook käyttäjän Android-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.</span><span class="sxs-lookup"><span data-stu-id="d03dd-147">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="d03dd-148">Avaa Sähkö posti viesti, joka sisältää muutamia kuva tiedosto liitteitä.</span><span class="sxs-lookup"><span data-stu-id="d03dd-148">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="d03dd-149">Voit tallentaa liitteen valitsemalla sen tietojen vieressä olevan alanuolikuvakkeen.</span><span class="sxs-lookup"><span data-stu-id="d03dd-149">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="d03dd-p106">Näyttöön voi tulla pyyntö sallia Outlookin käyttää laitteessa olevia valokuvia, mediatiedostoja ja muita tiedostoja. Valitse **Salli**.</span><span class="sxs-lookup"><span data-stu-id="d03dd-p106">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="d03dd-153">Valitse **Tallenna laitteeseen** näytön alareunassa ja avaa sitten **Galleria** -sovellus.</span><span class="sxs-lookup"><span data-stu-id="d03dd-153">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="d03dd-p107">Luettelossa pitäisi näkyä salattu valokuva (tai useita, jos tallensit useita kuvatiedostoliitteitä). Se voi näkyä Kuvat-luettelossa harmaana ruutuna, jonka keskellä on valkoisen ympyrän sisällä oleva valkoinen huutomerkki.</span><span class="sxs-lookup"><span data-stu-id="d03dd-p107">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="ios"></a><span data-ttu-id="d03dd-157">Ios</span><span class="sxs-lookup"><span data-stu-id="d03dd-157">iOS</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="d03dd-158">Sovellusten suojausasetusten toiminnan varmistaminen käyttäjien laitteissa</span><span class="sxs-lookup"><span data-stu-id="d03dd-158">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="d03dd-159">Kun olet [määrittänyt iOS-laitteiden sovellusasetukset](app-protection-settings-for-android-and-ios.md) sovellusten suojaamista varten, seuraavien ohjeiden avulla voit vahvistaa, että valitsemasi asetukset toimivat.</span><span class="sxs-lookup"><span data-stu-id="d03dd-159">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="d03dd-160">Varmista ensin, että käytäntö koskee sovellusta, jossa aiot tarkistaa sen.</span><span class="sxs-lookup"><span data-stu-id="d03dd-160">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="d03dd-161">Siirry Microsoft 365 Businessin [hallintakeskuksessa](https://portal.office.com) kohtaan **Käytännöt** \> **Muokkaa käytäntöä**.</span><span class="sxs-lookup"><span data-stu-id="d03dd-161">In the Microsoft 365 Business [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="d03dd-162">Valitse **iOS:n sovellus käytäntö** asetuksille, jotka olet luonut asetuksissa, tai toinen luomasi käytäntö ja varmista, että se on käytössä esimerkiksi Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="d03dd-162">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="d03dd-164">Vahvista Office-sovellusten käyttäminen edellyttää PIN-koodia</span><span class="sxs-lookup"><span data-stu-id="d03dd-164">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="d03dd-165">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Office-tiedostojen käytön hallinta** -kohdan vieressä, laajenna **Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa** ja varmista, että **Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä** on **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="d03dd-165">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Varmista, että vaadi PIN-koodi tai sormen jälki Office-sovellusten käyttöön on käytössä.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="d03dd-167">Avaa Outlook käyttäjän iOS-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="d03dd-167">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="d03dd-168">Sinua pyydetään myös syöttämään PIN-koodi tai käyttämään sormen jälkeä.</span><span class="sxs-lookup"><span data-stu-id="d03dd-168">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="d03dd-170">Vahvista Palauta PIN-koodi, kun on tehty tämä määrä epäonnistuneita yrityksiä</span><span class="sxs-lookup"><span data-stu-id="d03dd-170">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="d03dd-171">Valitse **Muokkaa käytäntöä** -ruudussa **Office-asia kirjojen käyttö oikeus-ohjaus objektin**vieressä **Muokkaa** , Laajenna **Hallitse, miten käyttäjät voivat käyttää Office-tiedostoja mobiililaitteilla**, ja varmista, että **Palauta PIN-koodin jälkeen epäonnistuneiden yritysten määrä** on asetettu johonkin numeroon.</span><span class="sxs-lookup"><span data-stu-id="d03dd-171">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="d03dd-172">Tämä on oletusarvoisesti 5.</span><span class="sxs-lookup"><span data-stu-id="d03dd-172">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="d03dd-173">Avaa Outlook käyttäjän iOS-laitteessa ja kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="d03dd-173">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="d03dd-174">Kirjoita virheellinen PIN-koodi niin monta kertaa kuin käytäntö määrittää.</span><span class="sxs-lookup"><span data-stu-id="d03dd-174">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="d03dd-175">Näkyviin tulee kehote, joka **antaa PIN-** koodin nollaamiseen.</span><span class="sxs-lookup"><span data-stu-id="d03dd-175">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="d03dd-177">Paina **OK**.</span><span class="sxs-lookup"><span data-stu-id="d03dd-177">Press **OK**.</span></span> <span data-ttu-id="d03dd-178">Sinua pyydetään Kirjautu maan sisään käyttäjän Microsoft 365-yrityksen tunniste tiedoilla ja asettamaan sitten uusi PIN-koodi.</span><span class="sxs-lookup"><span data-stu-id="d03dd-178">You'll be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="d03dd-179">Vahvista Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin</span><span class="sxs-lookup"><span data-stu-id="d03dd-179">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="d03dd-180">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** on **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="d03dd-180">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="d03dd-182">Avaa Outlook käyttäjän iOS-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.</span><span class="sxs-lookup"><span data-stu-id="d03dd-182">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="d03dd-183">Avaa liitteen sisältävä sähköpostiviesti, avaa liite ja valitse **Tallenna** näytön alareunassa.</span><span class="sxs-lookup"><span data-stu-id="d03dd-183">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="d03dd-185">Näkyvissä pitäisi olla vaihtoehto vain OneDrive for Businessille.</span><span class="sxs-lookup"><span data-stu-id="d03dd-185">You should only see an option for OneDrive for Business.</span></span> <span data-ttu-id="d03dd-186">Jos ei, napauta **Lisää tili** ja valitse **OneDrive for Business** **Lisää tallennus tili** -näytöstä.</span><span class="sxs-lookup"><span data-stu-id="d03dd-186">If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen.</span></span> <span data-ttu-id="d03dd-187">Kirjaudu sisään käyttäjän Microsoft 365 Business -tiedoilla kehotettaessa.</span><span class="sxs-lookup"><span data-stu-id="d03dd-187">Provide the end user's Microsoft 365 Business to sign in when prompted.</span></span> 
    
    <span data-ttu-id="d03dd-188">Napauta **Tallenna** ja valitse **OneDrive for Business**.</span><span class="sxs-lookup"><span data-stu-id="d03dd-188">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="d03dd-189">Vahvista Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä määritetyn ajan</span><span class="sxs-lookup"><span data-stu-id="d03dd-189">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="d03dd-190">Valitse **Muokkaa käytäntöä** -ruudussa **Office-asia kirjojen käyttö oikeus-ohjaus objektin**vieressä **Muokkaa** , Laajenna **Hallitse, miten käyttäjät voivat käyttää Office-tiedostoja mobiililaitteilla**, ja varmista, että edellytä, että **käyttäjät kirjautuvat uudelleen sisään, kun Office-sovellukset ovat olleet käyttämättömänä** , on asetettu joihinkin minuutteihin.</span><span class="sxs-lookup"><span data-stu-id="d03dd-190">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="d03dd-191">Tämä on oletusarvoisesti 30 minuuttia.</span><span class="sxs-lookup"><span data-stu-id="d03dd-191">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="d03dd-192">Avaa Outlook käyttäjän iOS-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.</span><span class="sxs-lookup"><span data-stu-id="d03dd-192">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="d03dd-p113">Outlookin Saapuneet-kansion pitäisi nyt näkyä. Älä koske iOS-laitteeseen vähintään 30 minuuttiin (tai muun käytäntöön määrittämääsi aikaa pidemmän ajan). Todennäköisesti laitteen näyttö himmenee.</span><span class="sxs-lookup"><span data-stu-id="d03dd-p113">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="d03dd-196">Avaa Outlook uudelleen iOS-laitteella.</span><span class="sxs-lookup"><span data-stu-id="d03dd-196">Access Outlook on the iOS device again.</span></span>
    
4. <span data-ttu-id="d03dd-197">Sinua pyydetään antamaan PIN-koodi, ennen kuin voit käyttää Outlookia uudelleen.</span><span class="sxs-lookup"><span data-stu-id="d03dd-197">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="d03dd-198">Vahvista Suojaa työtiedostot salauksella</span><span class="sxs-lookup"><span data-stu-id="d03dd-198">Validate Protect work files with encryption</span></span>

<span data-ttu-id="d03dd-199">Valitse **Muokkaa käytäntöä** -ruudussa **Muokkaa** **Kadonneiden tai varastettujen laitteiden suojaus** -kohdan vieressä, laajenna **Työtiedostojen suojaaminen laitteiden katoamisen tai varastamisen varalta** ja varmista, että **Suojaa työtiedostot salauksella** on **käytössä** ja **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** **pois käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="d03dd-199">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="d03dd-200">Avaa Outlook käyttäjän iOS-laitteessa, kirjaudu sisään käyttäjän Microsoft 365 Business -tunnistetiedoilla ja anna PIN-koodi pyydettäessä.</span><span class="sxs-lookup"><span data-stu-id="d03dd-200">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="d03dd-201">Avaa Sähkö posti viesti, joka sisältää muutamia kuva tiedosto liitteitä.</span><span class="sxs-lookup"><span data-stu-id="d03dd-201">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="d03dd-202">Napauta liitettä ja **Tallenna**-vaihtoehtoa sen alla.</span><span class="sxs-lookup"><span data-stu-id="d03dd-202">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="d03dd-p114">Avaa **Valokuvat**-sovellus aloitusnäytössä. Näkyviin tulee tallennettu mutta salattu valokuva (tai useampia, jos tallensit useita kuvatiedostoliitteitä).</span><span class="sxs-lookup"><span data-stu-id="d03dd-p114">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---

