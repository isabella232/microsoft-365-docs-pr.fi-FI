---
title: Microsoft 365 Businessin määrittäminen
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
ms.openlocfilehash: e635b828609fc47cd8b92bb179a25bcc43cb0a1a
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660765"
---
# <a name="set-up-microsoft-365-business"></a><span data-ttu-id="412a0-103">Microsoft 365 Businessin määrittäminen</span><span class="sxs-lookup"><span data-stu-id="412a0-103">Set up Microsoft 365 Business</span></span>

<span data-ttu-id="412a0-104">Ennen kuin aloitat, lisätietoja [Saat Microsoft 365 Business](get-microsoft-365-business.md) ilmoittautuminen.</span><span class="sxs-lookup"><span data-stu-id="412a0-104">Before you get started, see [Get Microsoft 365 Business](get-microsoft-365-business.md) for sign-up details.</span></span>

<span data-ttu-id="412a0-105">Katso [lyhyt video siitä, miten määritetään Microsoft 365 liiketoiminnan](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) määrittäminen ohjatun ja kun ei ole paikallisen Active Directoryn avulla</span><span class="sxs-lookup"><span data-stu-id="412a0-105">Watch a [short video on how to set up Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) by using the set up wizard, and when you don't have an on-premises Active Directory</span></span>
  

## <a name="overview"></a><span data-ttu-id="412a0-106">Yleistä</span><span class="sxs-lookup"><span data-stu-id="412a0-106">Overview</span></span>

<span data-ttu-id="412a0-107">Ohjattu asennus voidaan tehdä suurimman osan vaiheiden määrittäminen, mutta luetellaan myös muita vaihtoehtoja.</span><span class="sxs-lookup"><span data-stu-id="412a0-107">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>

1. <span data-ttu-id="412a0-108">[Toimialueen lisääminen](#add-your-domain-to-personalize-sign-in) (Jos olet ostanut toimialueen aikana [rekisteröityä](sign-up.md), tässä vaiheessa on jo tehty.)</span><span class="sxs-lookup"><span data-stu-id="412a0-108">[Add your domain](#add-your-domain-to-personalize-sign-in) (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>
2. <span data-ttu-id="412a0-109">Voit lisätä käyttäjiä.</span><span class="sxs-lookup"><span data-stu-id="412a0-109">Add users.</span></span> <span data-ttu-id="412a0-110">Voit tehdä tämän jossakin seuraavista kolmesta tavasta:</span><span class="sxs-lookup"><span data-stu-id="412a0-110">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="412a0-111">[Ohjattu asennus](#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="412a0-111">In the [setup wizard](#add-users-in-the-wizard).</span></span>
    - <span data-ttu-id="412a0-112">Käyttää hakemiston synkronointi [Azure AD-yhteyden avulla käyttäjät](#add-users-by-using-azure-ad-connect) lisätään paikalliseen Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="412a0-112">Use directory synchronization to [add users by using Azure AD Connect](#add-users-by-using-azure-ad-connect) if you have an on-premises Active directory.</span></span>
    - <span data-ttu-id="412a0-113">Voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) admin Centerissä.</span><span class="sxs-lookup"><span data-stu-id="412a0-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
3. <span data-ttu-id="412a0-114">Käytännöt ja laitteiden määrittäminen.</span><span class="sxs-lookup"><span data-stu-id="412a0-114">Set up security policies and configure devices.</span></span> <span data-ttu-id="412a0-115">Voit tehdä tämän jossakin seuraavista kolmesta tavasta:</span><span class="sxs-lookup"><span data-stu-id="412a0-115">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="412a0-116">[Ohjattu asennus](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="412a0-116">In the [setup wizard](#set-up-policies-in-the-wizard).</span></span>  
    - <span data-ttu-id="412a0-117">[Hallintakeskukseen](#modify-or-add-policies-in-the-admin-center).</span><span class="sxs-lookup"><span data-stu-id="412a0-117">In the [admin center](#modify-or-add-policies-in-the-admin-center).</span></span>
    - <span data-ttu-id="412a0-118">[Intune hallintakeskukseen](https://docs.microsoft.com/intune/what-is-device-management).</span><span class="sxs-lookup"><span data-stu-id="412a0-118">In the [Intune admin center](https://docs.microsoft.com/intune/what-is-device-management).</span></span>
4. <span data-ttu-id="412a0-119">Määritä ja Hallitse Windows 10-laitteita.</span><span class="sxs-lookup"><span data-stu-id="412a0-119">Set up and manage Windows 10 devices.</span></span>

    <span data-ttu-id="412a0-120">Kun liität laitteen WIndows 10 Azure AD, kaikki käytännöt tulla otetuiksi siihen.</span><span class="sxs-lookup"><span data-stu-id="412a0-120">When you join a WIndows 10 device to Azure AD, all the policies get applied to it.</span></span>
    - <span data-ttu-id="412a0-121">Määritä [ohjatun asennuksen](#set-up-policies-in-the-wizard)Windows 10 laitteiden määrityksiä.</span><span class="sxs-lookup"><span data-stu-id="412a0-121">Set up Windows 10 device configurations in the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="412a0-122">Liittää [Windows 10 uuden laitteen](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="412a0-122">Join a [new Windows 10 device](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) to Azure AD.</span></span>
    - <span data-ttu-id="412a0-123">[Olemassa Windows 10-laitteen](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) liittäminen Azure AD.</span><span class="sxs-lookup"><span data-stu-id="412a0-123">Join an [existing Windows 10 device](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) to Azure AD.</span></span>
1. <span data-ttu-id="412a0-124">Asenna Office 365: n liiketoiminnan.</span><span class="sxs-lookup"><span data-stu-id="412a0-124">Install Office 365 Business.</span></span>
    - <span data-ttu-id="412a0-125">Voit asentaa Officen Windows-laitteet automaattisesti [ohjatun asennustoiminnon](#set-up-policies-in-the-wizard)avulla.</span><span class="sxs-lookup"><span data-stu-id="412a0-125">You can automatically install Office in the Windows devices by using the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="412a0-126">Automaattisesti [asentaa Officen](auto-install-or-uninstall-office.md) hallintakeskukseen.</span><span class="sxs-lookup"><span data-stu-id="412a0-126">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
    - <span data-ttu-id="412a0-127">Antaa käyttäjien [asentaa Office-sovellukset](https://docs.microsoft.com/office365/admin/setup/install-applications) ja laitteet.</span><span class="sxs-lookup"><span data-stu-id="412a0-127">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
1. <span data-ttu-id="412a0-128">Lisätietoja suojauksen määrittäminen.</span><span class="sxs-lookup"><span data-stu-id="412a0-128">Set up additional security.</span></span>
    - <span data-ttu-id="412a0-129">Ohjattu asennus Lisää politiikan suojaa laitteita, mutta voit myös hyödyntää [suojausta](#additional-security-settings) ominaisuuksia voi auttaa turvallinen tietojen ja tilien ja sähköpostit.</span><span class="sxs-lookup"><span data-stu-id="412a0-129">The setup wizard adds policies to secure your devices, but you can also take advantage of [additional security](#additional-security-settings) capabilities to helps secure your data, accounts, and emails.</span></span> 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="412a0-130">Lisää toimialueen, käyttäjiä ja määrittämällä käytännöt</span><span class="sxs-lookup"><span data-stu-id="412a0-130">Add your domain, users and set up policies</span></span>

![Nauha, joka osoittaa https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="412a0-132">Kun ostat Microsoft 365 Business, voit halutessasi toimialue omistat tai ostaa yksi aikana [ilmoittautuminen](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="412a0-132">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="412a0-133">Jos olet ostanut uuden toimialueen Kun rekisteröidyit, toimialueesi on kaikki ylös ja voit siirtää [Lisää käyttäjät](#add-users-and-assign-licenses)ja määrittää käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="412a0-133">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="412a0-134">Voit mukauttaa sisään toimialueen lisääminen</span><span class="sxs-lookup"><span data-stu-id="412a0-134">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="412a0-135">Kirjautuminen [hallintakeskukseen Microsoft 365](https://admin.microsoft.com) yleisen järjestelmänvalvojan tunnuksilla.</span><span class="sxs-lookup"><span data-stu-id="412a0-135">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="412a0-136">Valitse Käynnistä ohjattu **Lisää toimialueeseen** .</span><span class="sxs-lookup"><span data-stu-id="412a0-136">Choose **Add a domain** to start the wizard.</span></span>

    ![Valitse Lisää toimialueeseen.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="412a0-138">Ohjatun toiminnon Kirjoita toimialuenimi, jota haluat käyttää (esimerkiksi contoso.com).</span><span class="sxs-lookup"><span data-stu-id="412a0-138">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Kuva Mukauta sivusi sisään.](media/personalizesignin.png)

    
4. <span data-ttu-id="412a0-140">Noudata ohjatun toiminnon [luoda DNS-tietueet on mahdollisesti DNS Office 365 videopalvelujen tarjoajan](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , joka tarkistaa, että omistat toimialueen.</span><span class="sxs-lookup"><span data-stu-id="412a0-140">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="412a0-141">Jos tiedät toimialueen isäntä, katso myös [tarkemmat ohjeet isäntä](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="412a0-141">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="412a0-142">Jos videopalvelujen tarjoajan on GoDaddy, on helppo prosessi ja sinua pyydetään automaattisesti kirjautua sisään ja anna Microsoft todentaa käyttäjän puolesta:</span><span class="sxs-lookup"><span data-stu-id="412a0-142">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![GoDaddy Vahvista sivun Valitse Hyväksy.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="412a0-144">Lisää käyttäjiä ja määritä käyttöoikeuksia</span><span class="sxs-lookup"><span data-stu-id="412a0-144">Add users and assign licenses</span></span>

<span data-ttu-id="412a0-145">Ohjatussa toiminnossa voit lisätä käyttäjiä, mutta voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) admin Centerissä.</span><span class="sxs-lookup"><span data-stu-id="412a0-145">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="412a0-146">Lisäksi jos paikalliseen toimialueen ohjauskoneeseen, voit lisätä käyttäjät, joilla on [Azure AD-muodosta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="412a0-146">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="412a0-147">Ohjatun käyttäjien lisääminen</span><span class="sxs-lookup"><span data-stu-id="412a0-147">Add users in the wizard</span></span>

<span data-ttu-id="412a0-148">Lisättävien käyttäjien ohjatun toiminnon Hae automaattisesti määritetty Microsoft 365 Business käyttöoikeuden.</span><span class="sxs-lookup"><span data-stu-id="412a0-148">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>
<span data-ttu-id="412a0-149">Jos paikallisen toimialueen ohjauskonetta ja Active Directoryn avulla on kohdassa [ddd Azure AD-yhteyden avulla käyttäjät](#add-users-by-using-azure-ad-connect).</span><span class="sxs-lookup"><span data-stu-id="412a0-149">If you have a local domain controller, and are using Active Directory, see [how to ddd users by using Azure AD Connect](#add-users-by-using-azure-ad-connect).</span></span>

![Lisää uusia käyttäjiä-sivun ohjatun toiminnon kuva](media/addnewuserspage.png)

1. <span data-ttu-id="412a0-p106">Jos Microsoft 365 Business-tilauksessasi on aiemmin luotuja käyttäjiä (jos esimerkiksi olet käyttänyt Azure AD Connectia), näkyviin tulee vaihtoehto, jolla voit määrittää heille käyttöoikeudet. Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="412a0-p106">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you will get an option to assign licenses to them now. Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="412a0-153">Kun käyttäjät on lisätty, näyttöön tulee vaihtoehto jakaminen on lisätty uusien käyttäjien tunnistetiedot.</span><span class="sxs-lookup"><span data-stu-id="412a0-153">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="412a0-154">Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.</span><span class="sxs-lookup"><span data-stu-id="412a0-154">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="412a0-155">Ohita sähköpostiviestien siirtäminen valitsemalla **Siirrä sähköpostiviestejä** -sivulla **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="412a0-155">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="412a0-156">Jos siirrät toisen sähköpostin tarjoajalta ja haluat kopioida tiedot myöhemmin, voit [Siirtyminen sähköpostin ja yhteystietojen Office 365: ssä](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="412a0-156">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>

#### <a name="add-users-by-using-azure-ad-connect"></a><span data-ttu-id="412a0-157">Lisää käyttäjät Azure AD-yhteyden avulla</span><span class="sxs-lookup"><span data-stu-id="412a0-157">Add users by using Azure AD Connect</span></span>

 <span data-ttu-id="412a0-158">Jos paikallisen toimialueohjaimen Active Directory-hakemistopalvelun kanssa, voit synkronoida käyttäjien kanssa Microsoft 365 Business [Azure AD-yhteyden](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)avulla.</span><span class="sxs-lookup"><span data-stu-id="412a0-158">If you have a local domain controller with Active Directory, you synchronize your users with Microsoft 365 Business by using [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span> <span data-ttu-id="412a0-159">Suorita tämä loppuun, ennen kuin käynnistät ohjatun asennuksen.</span><span class="sxs-lookup"><span data-stu-id="412a0-159">Complete this before you start the setup wizard.</span></span> <span data-ttu-id="412a0-160">Voit ladata sen admin Centerissä:</span><span class="sxs-lookup"><span data-stu-id="412a0-160">You can download it in the admin center:</span></span>

- <span data-ttu-id="412a0-161">Siirry **käyttäjät** \> **aktiivisia käyttäjiä**kolmea pistettä sivun yläosassa ja valitse sitten Lataa AD Azure Yhdistä **hakemiston synkronointi** .</span><span class="sxs-lookup"><span data-stu-id="412a0-161">Go to **Users** \> **Active users**, select the ellipses on the top of the page and then select **Directory synchronization** to download Azure AD Connect.</span></span>

    ![Aktiiviset käyttäjät-sivulla Valitse kolme pistettä > hakemiston snchronization.](media/setupdirsync.png)

    > [!IMPORTANT]
    > <span data-ttu-id="412a0-163">Jos luot käyttäjiä tällä tavalla, joudut silti liittää käyttöoikeudet niihin admin Centerissä.</span><span class="sxs-lookup"><span data-stu-id="412a0-163">If you create users this way, you will still have to assign licenses to them in the admin center.</span></span>

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a><span data-ttu-id="412a0-164">Jatkossakin käyttää toimialueeseen liittymistä apps ja laitteita</span><span class="sxs-lookup"><span data-stu-id="412a0-164">Continue to access domain-joined apps and devices</span></span>

<span data-ttu-id="412a0-165">Jos haluat edelleen käyttää toimialueeseen liittymistä apps ja laitteita, lue seuraavista artikkeleista käyttöönoton, kahdella eri tavalla:</span><span class="sxs-lookup"><span data-stu-id="412a0-165">If you want to continue to access domain-joined apps and devices, read the following articles for two different way of enabling that:</span></span>
  
- [<span data-ttu-id="412a0-166">Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi</span><span class="sxs-lookup"><span data-stu-id="412a0-166">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>](manage-windows-devices.md)
    - <span data-ttu-id="412a0-167">Tämä on suositeltava tapa.</span><span class="sxs-lookup"><span data-stu-id="412a0-167">This is the recommended way.</span></span>

- [<span data-ttu-id="412a0-168">Käyttää tiloissa Azure AD liitetty laite 365 Microsoft Business resurssit</span><span class="sxs-lookup"><span data-stu-id="412a0-168">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>](access-resources.md)

### <a name="connect-your-domain"></a><span data-ttu-id="412a0-169">Toimialueen yhdistäminen</span><span class="sxs-lookup"><span data-stu-id="412a0-169">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="412a0-170">Jos haluat käyttää toimialueen .onmicrosoft tai määrittää käyttäjille Azure AD-yhteyden avulla, et näe tässä vaiheessa.</span><span class="sxs-lookup"><span data-stu-id="412a0-170">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="412a0-171">Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.</span><span class="sxs-lookup"><span data-stu-id="412a0-171">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="412a0-172">Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa.</span><span class="sxs-lookup"><span data-stu-id="412a0-172">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="412a0-173">Jos näin ei ole, [Muuta nameservers määrittäminen Office 365: ssä registrar mahdollisesti toimialueen kanssa](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="412a0-173">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="412a0-174">Olemassa olevan DNS-tietueet, esimerkiksi web-sivuston, jos haluat hallita oman DNS-tietueet, varmista, että voit pysyä olemassa oleviin palveluihin.</span><span class="sxs-lookup"><span data-stu-id="412a0-174">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="412a0-175">Katso lisätietoja [toimialueen perusteet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .</span><span class="sxs-lookup"><span data-stu-id="412a0-175">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Yhteyttä toimialueen-sivu, jossa voin hallita omaa DNS-tietueet.](media/connectyourdomainpage.png)

2. <span data-ttu-id="412a0-177">Noudata ohjatun toiminnon ohjeita ja sähköpostin ja muita palveluita määritetään puolestasi.</span><span class="sxs-lookup"><span data-stu-id="412a0-177">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="412a0-178">Käytännöt ja laitteiston määritysten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="412a0-178">Set up security policies and device configurations</span></span> 

<span data-ttu-id="412a0-179">Näitä käytäntöjä sovelletaan käyttäjien annat käyttöoikeuden, tai käyttäjäryhmä, jos päätät määrittää eri käytäntöjä joukolle käyttäjiä.</span><span class="sxs-lookup"><span data-stu-id="412a0-179">These policies apply to every user you give a license to, or to a group of users if you decide to assign different policies to a set of users.</span></span>

#### <a name="set-up-policies-in-the-wizard"></a><span data-ttu-id="412a0-180">Määritä ohjatun toiminnon käytännöt</span><span class="sxs-lookup"><span data-stu-id="412a0-180">Set up policies in the wizard</span></span>

<span data-ttu-id="412a0-181">Ohjattu toiminto määrittää käytäntöjä käytetään automaattisesti *Kaikki*käyttäjät [suojausryhmään](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) .</span><span class="sxs-lookup"><span data-stu-id="412a0-181">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span>

1. <span data-ttu-id="412a0-182">**Mobiililaitteiden työn tiedostojen suojaaminen** vaihtoehto **Suojaa Työtiedostojen kun laitteita katoaa tai varastetaan** on oletusarvon mukaan valittuna.</span><span class="sxs-lookup"><span data-stu-id="412a0-182">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="412a0-183">Voit valita, **miten käyttäjät voivat käyttää mobiililaitteiden Office-tiedostojen hallinta**käyttöön ja tämä on suositeltavaa.</span><span class="sxs-lookup"><span data-stu-id="412a0-183">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Kuva on suojata Työtiedostojen matkaviestimet-sivulla.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="412a0-185">Jos laajennat **Suojaa Työtiedostojen kun laitteita katoaa tai varastetaan**, [oletusarvot](protect-work-files-on-lost-or-stolen-device.md) ovat ennalta valitut:</span><span class="sxs-lookup"><span data-stu-id="412a0-185">If you expand **Protect work files when devices are lost or stolen**, the [default values](protect-work-files-on-lost-or-stolen-device.md) are pre-selected:</span></span>

        ![Kuva laitteet menettää tiedostojen suojaaminen oletusarvot.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="412a0-187">Valitse, **miten käyttäjät voivat käyttää mobiililaitteiden Office-tiedostojen hallinta** ja laajentaa sitä, jos [oletusarvot](manage-user-access-on-mobile-devices.md) näkyvät.</span><span class="sxs-lookup"><span data-stu-id="412a0-187">If you select **Manage how users access Office files on mobile devices** and expand it, the [default values](manage-user-access-on-mobile-devices.md) are shown.</span></span> <span data-ttu-id="412a0-188">On suositeltavaa hyväksyä oletusarvot asennuksen aikana kaikkia käyttäjiä koskevien sovelluskäytäntöjen luomiseksi Androidille, iOS:lle ja Windows 10:lle.</span><span class="sxs-lookup"><span data-stu-id="412a0-188">We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="412a0-189">Voit luoda lisää käytäntöjä asennuksen päätyttyä.</span><span class="sxs-lookup"><span data-stu-id="412a0-189">You can create more policies after setup completes.</span></span>

        ![Kuva-mobile Office-tiedostojen asetukset.](media/useraccessonmobile.png)

2. <span data-ttu-id="412a0-191">Viimeinen vaihe Valitse suojaa tiedot ja laitteet mahdollistaa käytäntöjen määrittäminen Windows 10-laitteiden suojaamiseen.</span><span class="sxs-lookup"><span data-stu-id="412a0-191">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="412a0-192">Näitä asetuksia käytetään automaattisesti käyttäjän Windows-10 muodostaa yhteyden organisaatiossasi.</span><span class="sxs-lookup"><span data-stu-id="412a0-192">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="412a0-193">Voit laajentaa **suojattua Windows-10 laitteet** ja muokkaa [oletusarvoja](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="412a0-193">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="412a0-194">Voit myös [asentaa automaattisesti Officen](install-office-on-windows-10-during-setup.md) Windows 10-laitteissa.</span><span class="sxs-lookup"><span data-stu-id="412a0-194">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Kuva Aseta laitteen Windows 10-määrityssivulla.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a><span data-ttu-id="412a0-196">Muokkaa tai Lisää käytännöt-hallintakeskukseen</span><span class="sxs-lookup"><span data-stu-id="412a0-196">Modify or add policies in the admin center</span></span>

<span data-ttu-id="412a0-197">Katso [Microsoft 365 liiketoiminnan hallinnassa](manage.md) on linkkejä ohjeaiheisiin siitä, kuinka voit tarkastella ja muokata laitteiden ja sovellusten suojaus-käytäntöjä, ja tietojen poistamisesta tai Palauta käyttäjän laitteita.</span><span class="sxs-lookup"><span data-stu-id="412a0-197">See [manage Microsoft 365 Business](manage.md) for links to topics on how to view and modify device and app protection polices, and how to remove data from, or reset user devices.</span></span>

## <a name="deploy-and-manage-windows-10"></a><span data-ttu-id="412a0-198">Käyttöönotto ja hallinta Windows-10</span><span class="sxs-lookup"><span data-stu-id="412a0-198">Deploy and manage Windows 10</span></span>
<span data-ttu-id="412a0-199">Lisätietoja Azure AD, joko uusia tietokoneita tai vaihtamalla kirjautuminen profiilin käytössä asennuksen aikana muodostettava [määrittäminen Microsoft 365 yrityskäyttäjille Windows-laitteet](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="412a0-199">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) to manually connect to Azure AD, either during setup for new computers, or by changing sign-in profile for existing computers.</span></span> 

### <a name="use-autopilot-to-set-up-new-devices"></a><span data-ttu-id="412a0-200">Automaattiohjauksen avulla voit määrittää uusia laitteita</span><span class="sxs-lookup"><span data-stu-id="412a0-200">Use Autopilot to set up new devices</span></span>

<span data-ttu-id="412a0-201">[Windows automaattiohjauksen](add-autopilot-devices-and-profile.md) avulla voit määrittää käyttäjän **Uusi** Windows 10-laitteet automaattisesti ennalta, mutta voi olla helpompi saada [kumppani](https://www.microsoft.com/solution-providers/search) , jolla voit tehdä tämän sinulle.</span><span class="sxs-lookup"><span data-stu-id="412a0-201">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="412a0-202">Voit myös siirtyä [Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) ja pyytää asiantuntija pilvi tekniikka määrittää, ostaa uusia laitteita.</span><span class="sxs-lookup"><span data-stu-id="412a0-202">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

### <a name="access-on-premises-resources"></a><span data-ttu-id="412a0-203">Käyttää tiloissa resursseja</span><span class="sxs-lookup"><span data-stu-id="412a0-203">Access on-premises resources</span></span>

<span data-ttu-id="412a0-204">Jos organisaatiossa käytetään Windows Server Active Directory tiloissa, voit määrittää Microsoft 365 liiketoiminnan suojaamaan Windows 10-laitteet, säilyttäen kuitenkin edellyttää paikallista todennusta tiloissa resurssien käytön.</span><span class="sxs-lookup"><span data-stu-id="412a0-204">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="412a0-205">Voit määrittää [toimialueeseen liittymistä Windows 10 laitteita voi hallita Microsoft 365 Business käyttöön](manage-windows-devices.md) noudattamalla.</span><span class="sxs-lookup"><span data-stu-id="412a0-205">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="412a0-206">Tämä on ensisijainen menetelmä, ja tässä tilassa laitteita kutsutaan hybridi Azure AD liitetyt laitteet.</span><span class="sxs-lookup"><span data-stu-id="412a0-206">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

<span data-ttu-id="412a0-207">Jos yrityksesi on paikallista Active Directory, joka sisältää joitakin tiloissa (kuten jaettujen tiedostoresurssien ja tulostinten), voit antaa Azure AD liittynyt laitteiden käyttöä noudattamalla tässä nämä resurssit: [käyttö paikalliset resurssit Microsoft 365 Business AD liitetty laite Azure](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="412a0-207">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="412a0-208">Ottaa käyttöön Office 365-asiakassovellukset</span><span class="sxs-lookup"><span data-stu-id="412a0-208">Deploy Office 365 client apps</span></span>

<span data-ttu-id="412a0-209">Jos päätit asentaa Office-sovellukset automaattisesti joukon aikana ylös, apps asennetaan Windows 10-laitteet, kun käyttäjiä on kirjautuneena Azure AD laitteiden kanssa työtä tunnistetietonsa Windows.</span><span class="sxs-lookup"><span data-stu-id="412a0-209">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="412a0-210">Jos haluat asentaa Office mobile iOS tai Android-laitteet, kohdassa [Mobiililaitteiden käyttäjille Microsoft 365 Business määrittäminen](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="412a0-210">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="412a0-211">Voit asentaa Officen myös erikseen.</span><span class="sxs-lookup"><span data-stu-id="412a0-211">You can also install Office individually.</span></span> <span data-ttu-id="412a0-212">Katso ohjeet [asentaa PC-tai Mac Office](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) .</span><span class="sxs-lookup"><span data-stu-id="412a0-212">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for instructions.</span></span>

## <a name="additional-security-settings"></a><span data-ttu-id="412a0-213">Muita tietoturva-asetuksia</span><span class="sxs-lookup"><span data-stu-id="412a0-213">Additional security settings</span></span>

<span data-ttu-id="412a0-214">Suojaus ja yhteensopivuus-asetus ohjatun asennuksen lisäksi voit määrittää myös seuraavia lisäasetuksia:</span><span class="sxs-lookup"><span data-stu-id="412a0-214">In addition to the security and compliance setting in the setup wizard, you can also set up the following additional settings:</span></span>
  
- <span data-ttu-id="412a0-215">**Sähköposti Suojaus haittaohjelmilta**</span><span class="sxs-lookup"><span data-stu-id="412a0-215">**Email malware protection**</span></span>
- <span data-ttu-id="412a0-216">**Kehittyneen uhkien suojaa (ATP) Turvalliset liitetiedostot**</span><span class="sxs-lookup"><span data-stu-id="412a0-216">**Advanced Threat Protection (ATP) Safe Attachments**</span></span>
- <span data-ttu-id="412a0-217">**ATP-Safe-linkit**</span><span class="sxs-lookup"><span data-stu-id="412a0-217">**ATP Safe Links**</span></span>
- <span data-ttu-id="412a0-218">**PIHARAKENNUS anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="412a0-218">**APT anti-phishing**</span></span>
- <span data-ttu-id="412a0-219">**Exchange Online Archiving**</span><span class="sxs-lookup"><span data-stu-id="412a0-219">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="412a0-220">**Tietojen menetyksen estäminen (DLP)**</span><span class="sxs-lookup"><span data-stu-id="412a0-220">**Data loss prevention (DLP)**</span></span>
- <span data-ttu-id="412a0-221">**Azure-tietojen suojaaminen** (1 aio)</span><span class="sxs-lookup"><span data-stu-id="412a0-221">**Azure Information Protection** (Plan 1)</span></span>
- <span data-ttu-id="412a0-222">**Portaalin käytettävyyttä Intune**</span><span class="sxs-lookup"><span data-stu-id="412a0-222">**Intune portal availability**</span></span>

<span data-ttu-id="412a0-223">Aloita ks- [käytäntöjen suojauksen lisäasetusten määrittäminen](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="412a0-223">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

<span data-ttu-id="412a0-224">Katso myös suojauksen parhaiden käytäntöjen opas [top 10 tapoja suojata yrityksen Microsoft 365](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) .</span><span class="sxs-lookup"><span data-stu-id="412a0-224">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>