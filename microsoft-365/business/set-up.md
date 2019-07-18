---
title: Microsoft 365 Businessin määrittäminen
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Opi määrittämään Microsoft 365 Business.
ms.openlocfilehash: ac9c8b828ff131a15bf057fa8bdc0bf56dd00987
ms.sourcegitcommit: 75b97d1ff617bc4b1b0ef9135dfe6a8842ea1b52
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/18/2019
ms.locfileid: "35772563"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="b177b-103">Määritä ohjatussa asennustoiminnossa 365 Microsoft Business</span><span class="sxs-lookup"><span data-stu-id="b177b-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="b177b-104">Lisää toimialueen käyttäjille ja käytäntöjen määrittäminen</span><span class="sxs-lookup"><span data-stu-id="b177b-104">Add your domain, users, and set up policies</span></span>

![Nauha, joka osoittaa https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="b177b-106">Kun ostat Microsoft 365 Business, voit halutessasi toimialue omistat tai ostaa yksi aikana [ilmoittautuminen](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="b177b-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="b177b-107">Jos olet ostanut uuden toimialueen Kun rekisteröidyit, toimialueesi on kaikki ylös ja voit siirtää [Lisää käyttäjät](#add-users-and-assign-licenses)ja määrittää käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="b177b-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="b177b-108">Voit mukauttaa sisään toimialueen lisääminen</span><span class="sxs-lookup"><span data-stu-id="b177b-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="b177b-109">Kirjautuminen [hallintakeskukseen Microsoft 365](https://admin.microsoft.com) yleisen järjestelmänvalvojan tunnuksilla.</span><span class="sxs-lookup"><span data-stu-id="b177b-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="b177b-110">Valitse **Lisää toimialueeseen** **Lisää käyttäjiä** tai Käynnistä ohjattu toiminto.</span><span class="sxs-lookup"><span data-stu-id="b177b-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="b177b-111">Jos olet ostanut toimialueen rekisteröitymisen yhteydessä, se ei katso **Lisää toimialue** vaiheen tähän.</span><span class="sxs-lookup"><span data-stu-id="b177b-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="b177b-112">Siirry [Lisää käyttäjiä](#add-users-and-assign-licenses) sen sijaan.</span><span class="sxs-lookup"><span data-stu-id="b177b-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Valitse Lisää toimialueeseen.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="b177b-114">Ohjatun toiminnon Kirjoita toimialuenimi, jota haluat käyttää (esimerkiksi contoso.com).</span><span class="sxs-lookup"><span data-stu-id="b177b-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Kuva Mukauta sivusi sisään.](media/personalizesignin.png)

    
4. <span data-ttu-id="b177b-116">Noudata ohjatun toiminnon [luoda DNS-tietueet on mahdollisesti DNS Office 365 videopalvelujen tarjoajan](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , joka tarkistaa, että omistat toimialueen.</span><span class="sxs-lookup"><span data-stu-id="b177b-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="b177b-117">Jos tiedät toimialueen isäntä, katso myös [tarkemmat ohjeet isäntä](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="b177b-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="b177b-118">Jos videopalvelujen tarjoajan on GoDaddy, on helppo prosessi ja sinua pyydetään automaattisesti kirjautua sisään ja anna Microsoft todentaa käyttäjän puolesta:</span><span class="sxs-lookup"><span data-stu-id="b177b-118">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![GoDaddy Vahvista sivun Valitse Hyväksy.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="b177b-120">Lisää käyttäjiä ja määritä käyttöoikeuksia</span><span class="sxs-lookup"><span data-stu-id="b177b-120">Add users and assign licenses</span></span>

<span data-ttu-id="b177b-121">Ohjatussa toiminnossa voit lisätä käyttäjiä, mutta voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) admin Centerissä.</span><span class="sxs-lookup"><span data-stu-id="b177b-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="b177b-122">Lisäksi jos paikalliseen toimialueen ohjauskoneeseen, voit lisätä käyttäjät, joilla on [Azure AD-muodosta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="b177b-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="b177b-123">Ohjatun käyttäjien lisääminen</span><span class="sxs-lookup"><span data-stu-id="b177b-123">Add users in the wizard</span></span>

<span data-ttu-id="b177b-124">Lisättävien käyttäjien ohjatun toiminnon Hae automaattisesti määritetty Microsoft 365 Business käyttöoikeuden.</span><span class="sxs-lookup"><span data-stu-id="b177b-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Lisää uusia käyttäjiä-sivun ohjatun toiminnon kuva](media/addnewuserspage.png)

1. <span data-ttu-id="b177b-126">Jos Microsoft 365 Business-tilauksesi on olemassa käyttäjiä (esimerkiksi jos olet käyttänyt AD-Yhdistä Azure), voit määrittää käyttöoikeudet niihin nyt saat.</span><span class="sxs-lookup"><span data-stu-id="b177b-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you get an option to assign licenses to them now.</span></span> <span data-ttu-id="b177b-127">Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="b177b-127">Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="b177b-128">Kun käyttäjät on lisätty, näyttöön tulee vaihtoehto jakaminen on lisätty uusien käyttäjien tunnistetiedot.</span><span class="sxs-lookup"><span data-stu-id="b177b-128">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="b177b-129">Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.</span><span class="sxs-lookup"><span data-stu-id="b177b-129">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="b177b-130">Ohita sähköpostiviestien siirtäminen valitsemalla **Siirrä sähköpostiviestejä** -sivulla **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="b177b-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="b177b-131">Jos siirrät toisen sähköpostin tarjoajalta ja haluat kopioida tiedot myöhemmin, voit [Siirtyminen sähköpostin ja yhteystietojen Office 365: ssä](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="b177b-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="b177b-132">Toimialueen yhdistäminen</span><span class="sxs-lookup"><span data-stu-id="b177b-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="b177b-133">Jos haluat käyttää toimialueen .onmicrosoft tai määrittää käyttäjille Azure AD-yhteyden avulla, et näe tässä vaiheessa.</span><span class="sxs-lookup"><span data-stu-id="b177b-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="b177b-134">Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.</span><span class="sxs-lookup"><span data-stu-id="b177b-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="b177b-135">Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa.</span><span class="sxs-lookup"><span data-stu-id="b177b-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="b177b-136">Jos näin ei ole, [Muuta nameservers määrittäminen Office 365: ssä registrar mahdollisesti toimialueen kanssa](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="b177b-136">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="b177b-137">Olemassa olevan DNS-tietueet, esimerkiksi web-sivuston, jos haluat hallita oman DNS-tietueet, varmista, että voit pysyä olemassa oleviin palveluihin.</span><span class="sxs-lookup"><span data-stu-id="b177b-137">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="b177b-138">Katso lisätietoja [toimialueen perusteet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .</span><span class="sxs-lookup"><span data-stu-id="b177b-138">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Yhteyttä toimialueen-sivu, jossa voin hallita omaa DNS-tietueet.](media/connectyourdomainpage.png)

2. <span data-ttu-id="b177b-140">Noudata ohjatun toiminnon ohjeita ja sähköpostin ja muita palveluita määritetään puolestasi.</span><span class="sxs-lookup"><span data-stu-id="b177b-140">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="b177b-141">Käytännöt ja laitteiston määritysten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="b177b-141">Set up security policies and device configurations</span></span> 

<span data-ttu-id="b177b-142">Ohjattu toiminto määrittää käytäntöjä käytetään automaattisesti *Kaikki*käyttäjät [suojausryhmään](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) .</span><span class="sxs-lookup"><span data-stu-id="b177b-142">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="b177b-143">Voit myös luoda uusia ryhmiä määrittelemään hallintakeskukseen käytäntöjä.</span><span class="sxs-lookup"><span data-stu-id="b177b-143">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="b177b-144">**Mobiililaitteiden työn tiedostojen suojaaminen** vaihtoehto **Suojaa Työtiedostojen kun laitteita katoaa tai varastetaan** on oletusarvon mukaan valittuna.</span><span class="sxs-lookup"><span data-stu-id="b177b-144">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="b177b-145">Voit valita, **miten käyttäjät voivat käyttää mobiililaitteiden Office-tiedostojen hallinta**käyttöön ja tämä on suositeltavaa.</span><span class="sxs-lookup"><span data-stu-id="b177b-145">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Kuva on suojata Työtiedostojen matkaviestimet-sivulla.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="b177b-147">Laajenna **Suojaa Työtiedostojen kun laitteita katoaa tai varastetaan** [oletusarvot](protect-work-files-on-lost-or-stolen-device.md):</span><span class="sxs-lookup"><span data-stu-id="b177b-147">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![Kuva laitteet menettää tiedostojen suojaaminen oletusarvot.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="b177b-149">**Miten käyttäjät voivat käyttää mobiililaitteiden Office-tiedostojen hallinta** Valitse ja laajenna se näyttää [oletusarvot](manage-user-access-on-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="b177b-149">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="b177b-150">Suosittelemme, että hyväksyt Sovelluskäytännöt Luo Android, iOS ja Windows 10-asennuksen aikana oletusarvot, jotka koskevat kaikkia käyttäjiä.</span><span class="sxs-lookup"><span data-stu-id="b177b-150">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="b177b-151">Voit luoda lisää käytäntöjä asennuksen päätyttyä.</span><span class="sxs-lookup"><span data-stu-id="b177b-151">You can create more policies after setup completes.</span></span>

        ![Kuva-mobile Office-tiedostojen asetukset.](media/useraccessonmobile.png)

2. <span data-ttu-id="b177b-153">Viimeinen vaihe Valitse suojaa tiedot ja laitteet mahdollistaa käytäntöjen määrittäminen Windows 10-laitteiden suojaamiseen.</span><span class="sxs-lookup"><span data-stu-id="b177b-153">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="b177b-154">Näitä asetuksia käytetään automaattisesti käyttäjän Windows-10 muodostaa yhteyden organisaatiossasi.</span><span class="sxs-lookup"><span data-stu-id="b177b-154">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="b177b-155">Voit laajentaa **suojattua Windows-10 laitteet** ja muokkaa [oletusarvoja](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="b177b-155">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="b177b-156">Voit myös [asentaa automaattisesti Officen](install-office-on-windows-10-during-setup.md) Windows 10-laitteissa.</span><span class="sxs-lookup"><span data-stu-id="b177b-156">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Kuva Aseta laitteen Windows 10-määrityssivulla.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="b177b-158">Ottaa käyttöön Office 365-asiakassovellukset</span><span class="sxs-lookup"><span data-stu-id="b177b-158">Deploy Office 365 client apps</span></span>

<span data-ttu-id="b177b-159">Jos päätit asentaa Office-sovellukset automaattisesti joukon aikana ylös, apps asennetaan Windows 10-laitteet, kun käyttäjiä on kirjautuneena Azure AD laitteiden kanssa työtä tunnistetietonsa Windows.</span><span class="sxs-lookup"><span data-stu-id="b177b-159">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="b177b-160">Jos haluat asentaa Office mobile iOS tai Android-laitteet, kohdassa [Mobiililaitteiden käyttäjille Microsoft 365 Business määrittäminen](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="b177b-160">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="b177b-161">Voit asentaa Officen myös erikseen.</span><span class="sxs-lookup"><span data-stu-id="b177b-161">You can also install Office individually.</span></span> <span data-ttu-id="b177b-162">Katso ohjeet [asentaa PC-tai Mac Office](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .</span><span class="sxs-lookup"><span data-stu-id="b177b-162">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>
