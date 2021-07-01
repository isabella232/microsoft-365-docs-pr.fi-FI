---
title: Määritä Microsoft 365 Business Premium
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Tutustu määritykseen, Microsoft 365 Business Premium, kuten toimialueen ja käyttäjien lisääminen, suojauskäytäntöjen määrittäminen ja paljon muuta.
ms.openlocfilehash: 74a98e915577cf86ec32a706bd3b8f558f49db95
ms.sourcegitcommit: 48195345b21b409b175d68acdc25d9f2fc4fc5f1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/30/2021
ms.locfileid: "53227635"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="9f9a7-103">Asetusten Microsoft 365 Business Premium määrittäminen ohjatussa määritystoiminnossa</span><span class="sxs-lookup"><span data-stu-id="9f9a7-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

## <a name="watch-overview-of-microsoft-365-setup"></a><span data-ttu-id="9f9a7-104">Katso: Yleiskatsaus Microsoft 365 asetuksiin</span><span class="sxs-lookup"><span data-stu-id="9f9a7-104">Watch: Overview of Microsoft 365 setup</span></span>

<span data-ttu-id="9f9a7-105">Tässä videossa on yleiskatsaus Microsoft 365 Business Premium määrityksestä.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-105">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="9f9a7-106">Toimialueen, käyttäjien ja käytännöt lisääminen</span><span class="sxs-lookup"><span data-stu-id="9f9a7-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="9f9a7-107">Kun ostat Microsoft 365 Business Premium, voit käyttää omaa toimialuetta tai ostaa sellaisen [rekisteröitymisen yhteydessä.](sign-up.md)</span><span class="sxs-lookup"><span data-stu-id="9f9a7-107">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="9f9a7-108">Jos ostit uuden toimialueen rekisteröityessäsi, toimialueesi on kaikki määritetty ja voit siirtyä Lisää käyttäjiä -alueeseen [ja määrittää käyttöoikeuksia.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="9f9a7-108">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="9f9a7-109">Toimialueen lisääminen sisäänkirjautumista varten</span><span class="sxs-lookup"><span data-stu-id="9f9a7-109">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="9f9a7-110">Kirjaudu sisään [Microsoft 365 -hallintakeskus](https://admin.microsoft.com) yleisen järjestelmänvalvojan tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-110">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="9f9a7-111">Käynnistä **ohjattu toiminto valitsemalla** Siirry asennukseen.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-111">Choose **Go to setup** to start the wizard.</span></span>

    ![Valitse Siirry asennukseen.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="9f9a7-113">Voit **halutessasi asentaa Office sovellukset** omaan tietokoneeseesi Asenna omat sovellukset -sivulla.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-113">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="9f9a7-114">Kirjoita **Lisää toimialue -vaiheessa** toimialuenimi, jota haluat käyttää (kuten contoso.com).</span><span class="sxs-lookup"><span data-stu-id="9f9a7-114">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="9f9a7-115">Jos olet ostanut toimialueen rekisteröitymisen aikana, Lisää toimialue -vaihetta **ei ole** tässä.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-115">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="9f9a7-116">Siirry sen sijaan Lisää käyttäjiä -ylle. [](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="9f9a7-116">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Näyttökuva Mukauta kirjautumista -sivusta.](../media/adddomain.png)

    
4. <span data-ttu-id="9f9a7-118">Noudata ohjatun toiminnon ohjeita kohdassa DNS-tietueiden luominen missä tahansa [DNS-isännöintipalvelussa Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) vahvistaa, että omistat toimialueen.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-118">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="9f9a7-119">Jos tiedät toimialueen isännän, katso lisätietoja myös kohdassa [Toimialueen lisääminen Microsoft 365.](/microsoft-365/admin/setup/add-domain)</span><span class="sxs-lookup"><span data-stu-id="9f9a7-119">If you know your domain host, see also [Add a domain to Microsoft 365](/microsoft-365/admin/setup/add-domain).</span></span>

    <span data-ttu-id="9f9a7-120">Jos isännöintipalvelusi on GoDaddy [](/office365/admin/get-help-with-domains/domain-connect)tai jokin muu isännöintipalvelu, jossa on käytössä toimialue, prosessi on helppo, ja sinua pyydetään automaattisesti kirjautumaan sisään ja antamaan Microsoftin todentaa puolestasi.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-120">If your hosting provider is GoDaddy or another host enabled with [domain connect](/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Valitse GoDaddyn Vahvista käyttö -sivulla Valtuuta.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="9f9a7-122">Lisää käyttäjiä ja määritä käyttöoikeuksia</span><span class="sxs-lookup"><span data-stu-id="9f9a7-122">Add users and assign licenses</span></span>

<span data-ttu-id="9f9a7-123">Voit lisätä käyttäjiä ohjatussa toiminnossa, mutta voit myös [lisätä käyttäjiä myöhemmin](../admin/add-users/add-users.md) hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-123">You can add users in the wizard, but you can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span> <span data-ttu-id="9f9a7-124">Lisäksi jos sinulla on paikallinen toimialueen ohjauskone, voit lisätä käyttäjiä, joilla on [Azure AD Näyttöyhteys.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="9f9a7-124">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="9f9a7-125">Käyttäjien lisääminen ohjatussa toiminnossa</span><span class="sxs-lookup"><span data-stu-id="9f9a7-125">Add users in the wizard</span></span>

<span data-ttu-id="9f9a7-126">Kaikki ohjatussa toiminnossa lisäät käyttäjät saavat automaattisesti Microsoft 365 Business Premium käyttöoikeuden.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-126">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Näyttökuva ohjatun toiminnon Lisää uusia käyttäjiä -sivusta](../media/addnewuserspage.png)

1. <span data-ttu-id="9f9a7-128">Jos Microsoft 365 Business Premium on olemassa olevia käyttäjiä (jos esimerkiksi käytit Azure AD Näyttöyhteys:tä), voit määrittää heille käyttöoikeudet nyt.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-128">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="9f9a7-129">Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-129">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="9f9a7-130">Kun olet lisännyt käyttäjät, voit myös jakaa tunnistetiedot lisäämisen uusien käyttäjien kanssa.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-130">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="9f9a7-131">Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-131">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="9f9a7-132">Toimialueen yhdistäminen</span><span class="sxs-lookup"><span data-stu-id="9f9a7-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="9f9a7-133">Jos päätit käyttää .onmicrosoft-toimialuetta tai määrittää Näyttöyhteys Azure AD:llä, et näe tätä vaihetta.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="9f9a7-134">Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="9f9a7-135">Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="9f9a7-136">Jos näin ei ole, muuta nimipalvelimia niin, että [ne Microsoft 365 toimialuerekisteröijän kanssa.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md)</span><span class="sxs-lookup"><span data-stu-id="9f9a7-136">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md).</span></span> 

    - <span data-ttu-id="9f9a7-137">Jos sinulla on olemassa olevia DNS-tietueita, esimerkiksi olemassa oleva sivusto, mutta DNS-isännöintipalvelusi on otettu käyttöön toimialueen [yhteydessä](/office365/admin/get-help-with-domains/domain-connect), valitse **Lisää tietueet minulle**.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-137">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="9f9a7-138">Hyväksy **Valitse verkkopalvelut -sivulla** kaikki oletusasetukset, valitse Seuraava ja **valitse** DNS-isännöintipalvelun sivulla Valtuuta.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-138">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="9f9a7-139">Jos sinulla on aiemmin luotuja DNS-tietueita muiden DNS-isännöintipalvelujen kanssa (ei otettu käyttöön toimialueen yhdistettynä), sinun on hallittava omia DNS-tietueitasi ja varmistaa, että olemassa olevat palvelut ovat yhteydessä toisiinsa.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-139">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="9f9a7-140">Lisätietoja on toimialueen perustoimialueissa. [](/office365/admin/get-help-with-domains/dns-basics)</span><span class="sxs-lookup"><span data-stu-id="9f9a7-140">See [domain basics](/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Aktivoi tietueet -sivu.](../media/activaterecords.png)

2. <span data-ttu-id="9f9a7-142">Noudata ohjatun toiminnon ohjeita, niin sähköposti ja muut palvelut määritetään sinulle.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-142">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="9f9a7-143">Suojaa organisaatiosi</span><span class="sxs-lookup"><span data-stu-id="9f9a7-143">Protect your organization</span></span> 

<span data-ttu-id="9f9a7-144">Ohjatussa toiminnossa määrittänyt käytännöt otetaan [](/office365/admin/create-groups/compare-groups#security-groups) automaattisesti käyttöön Kaikki käyttäjät *-käyttöoikeusryhmässä.*</span><span class="sxs-lookup"><span data-stu-id="9f9a7-144">The policies you set up in the wizard are applied automatically to a [Security group](/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="9f9a7-145">Voit myös luoda muita ryhmiä, joissa käytäntöjä määritetään hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-145">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="9f9a7-146">Paranna **kehittyneiden kyberuhkien** suojausta -sivulla on suositeltavaa hyväksyä oletusasetukset, jotta [Office 365 Advance Threat Protectionin](../security/office-365-security/defender-for-office-365.md) tarkistustiedostot ja linkit Office sovelluksissa.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-146">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](../security/office-365-security/defender-for-office-365.md) scan files and links in Office apps.</span></span>

    ![Näyttökuva Lisää suojausta -sivusta.](../media/increasetreatprotection.png)


2. <span data-ttu-id="9f9a7-148">Hyväksy **Estä** luottamuksellisten tietojen vuodot -sivulla oletusarvot, jotka Office 365 Tietojen menetyksen estäminen (DLP) -asetuksen käyttöön, jotta voit seurata luottamuksellisia tietoja Office-sovelluksissa ja estää niiden tahattoman jakamisen organisaation ulkopuolelle.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-148">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="9f9a7-149">Jätä **Mobiilisovellusten Office** -sivulla Mobiilisovellusten hallinta käyttöön, laajenna asetukset, tarkista ne ja valitse sitten Luo **mobiilisovellusten hallintakäytäntö**.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-149">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Näyttökuva Suojaa Office mobiiliversiossa -sivusta.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="9f9a7-151">Suojattu Windows 10 tietokoneet</span><span class="sxs-lookup"><span data-stu-id="9f9a7-151">Secure Windows 10 PCs</span></span>

<span data-ttu-id="9f9a7-152">Valitse vasemmassa siirtymisruudussa **Asetukset** ja valitse sitten **Kirjautumis-** ja suojaus -kohdassa **Suojaa Windows 10 tietokoneet**.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-152">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="9f9a7-153">Aloita **valitsemalla** Näytä.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-153">Choose **View** to get started.</span></span> <span data-ttu-id="9f9a7-154">Katso [Windows 10 tietokoneen suojaaminen.](secure-win-10-pcs.md)</span><span class="sxs-lookup"><span data-stu-id="9f9a7-154">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="9f9a7-155">Asiakassovellusten Office 365 käyttöönotto</span><span class="sxs-lookup"><span data-stu-id="9f9a7-155">Deploy Office 365 client apps</span></span>

<span data-ttu-id="9f9a7-156">Jos päätit asentaa Office-sovellukset automaattisesti asennuksen aikana, sovellukset asennetaan Windows 10-laitteisiin, kun käyttäjät ovat kirjautuneet Sisään Azure AD:iin Windows-laitteistaan työtunnuksilla.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-156">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="9f9a7-157">Jos haluat asentaa Office iOS- tai Android-laitteisiin, katso mobiililaitteiden [Microsoft 365 Business Premium käyttöön.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="9f9a7-157">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="9f9a7-158">Voit myös asentaa Office erikseen.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-158">You can also install Office individually.</span></span> <span data-ttu-id="9f9a7-159">Katso [Office PC: lle tai Macille](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) asennusohjeet.</span><span class="sxs-lookup"><span data-stu-id="9f9a7-159">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="related-content"></a><span data-ttu-id="9f9a7-160">Aiheeseen liittyvä sisältö</span><span class="sxs-lookup"><span data-stu-id="9f9a7-160">Related content</span></span>

<span data-ttu-id="9f9a7-161">[Microsoft 365 yrityksille 2010 -koulutusvideoita](../business-video/index.yml) (linkkisivu)</span><span class="sxs-lookup"><span data-stu-id="9f9a7-161">[Microsoft 365 for business training videos](../business-video/index.yml) (link page)</span></span>
