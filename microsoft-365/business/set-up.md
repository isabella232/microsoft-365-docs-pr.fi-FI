---
title: Microsoft 365 Business Premiumin määritäminen
f1.keywords:
- NOCSH
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
description: Tutustu Microsoft 365 Business Premiumin määritysvaiheisiin, kuten toimialueen ja käyttäjien lisäämiseen, suojauskäytäntöjen määrittämiseen ja paljon muuta.
ms.openlocfilehash: 4d49ba7ccdb65691756aaa505d0856deb115595b
ms.sourcegitcommit: 956176ed7c8b8427fdc655abcd1709d86da9447e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/23/2021
ms.locfileid: "51052230"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="e2496-103">Microsoft 365 Business Premiumin määrittäminen ohjatussa määritystoiminnossa</span><span class="sxs-lookup"><span data-stu-id="e2496-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="e2496-104">Tässä videossa on yleiskuvaus Microsoft 365 Business Premiumin määrityksestä.</span><span class="sxs-lookup"><span data-stu-id="e2496-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="e2496-105">Toimialueen, käyttäjien ja toimintakäytäntöjen lisääminen</span><span class="sxs-lookup"><span data-stu-id="e2496-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="e2496-106">Kun ostat Microsoft 365 Business Premiumin, voit käyttää omaa toimialuetta tai ostaa sellaisen [rekisteröitymisen aikana.](sign-up.md)</span><span class="sxs-lookup"><span data-stu-id="e2496-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="e2496-107">Jos ostit uuden toimialueen rekisteröityessäsi, toimialueesi on määritetty ja voit siirtyä Lisää käyttäjiä -alueeseen [ja määrittää käyttöoikeuksia.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="e2496-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="e2496-108">Toimialueen lisääminen sisäänkirjautumista varten</span><span class="sxs-lookup"><span data-stu-id="e2496-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="e2496-109">Kirjaudu [Microsoft 365 -hallintakeskukseen yleisen](https://admin.microsoft.com) järjestelmänvalvojan tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="e2496-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="e2496-110">Käynnistä **ohjattu toiminto valitsemalla** Siirry asennukseen.</span><span class="sxs-lookup"><span data-stu-id="e2496-110">Choose **Go to setup** to start the wizard.</span></span>

    ![Valitse Siirry asennukseen.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="e2496-112">Asenna **Office-sovellukset -sivulla** voit halutessasi asentaa sovellukset omaan tietokoneeseesi.</span><span class="sxs-lookup"><span data-stu-id="e2496-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="e2496-113">Kirjoita **Lisää toimialue -vaiheeseen** toimialuenimi, jota haluat käyttää (kuten contoso.com).</span><span class="sxs-lookup"><span data-stu-id="e2496-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="e2496-114">Jos olet ostanut toimialueen rekisteröitymisen aikana, Lisää toimialue -vaihetta ei **tule** tässä.</span><span class="sxs-lookup"><span data-stu-id="e2496-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="e2496-115">Siirry sen sijaan Lisää käyttäjiä -ylle. [](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="e2496-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Näyttökuva Mukauta kirjautumissivua -ruudusta.](../media/adddomain.png)

    
4. <span data-ttu-id="e2496-117">Luo DNS-tietueet missä tahansa [Microsoft 365:n](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) DNS-isännöintipalvelussa ohjatun toiminnon ohjeiden mukaisesti, joka vahvistaa, että omistat toimialueen.</span><span class="sxs-lookup"><span data-stu-id="e2496-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="e2496-118">Jos tiedät toimialueesi isännän, tutustu myös [isäntäkohtaisiin ohjeisiin.](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)</span><span class="sxs-lookup"><span data-stu-id="e2496-118">If you know your domain host, see also the [host specific instructions](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="e2496-119">Jos isännöintipalvelusi on GoDaddy tai jokin muu isännöintipalvelu on otettu käyttöön toimialueen [yhteydessä,](/office365/admin/get-help-with-domains/domain-connect)prosessi on helppoa, ja sinua pyydetään automaattisesti kirjautumaan sisään ja antamaan Microsoftin todentaa asia puolestasi.</span><span class="sxs-lookup"><span data-stu-id="e2496-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Valitse GoDaddyn Vahvista käyttö -sivulla Valtuuta.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="e2496-121">Lisää käyttäjiä ja määritä käyttöoikeuksia</span><span class="sxs-lookup"><span data-stu-id="e2496-121">Add users and assign licenses</span></span>

<span data-ttu-id="e2496-122">Voit lisätä käyttäjiä ohjatussa toiminnossa, mutta voit myös [lisätä käyttäjiä](../admin/add-users/add-users.md) myöhemmin hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="e2496-122">You can add users in the wizard, but you can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span> <span data-ttu-id="e2496-123">Lisäksi jos sinulla on paikallinen toimialueen ohjauskone, voit lisätä käyttäjiä [Azure AD Connectilla.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="e2496-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="e2496-124">Käyttäjien lisääminen ohjatussa toiminnossa</span><span class="sxs-lookup"><span data-stu-id="e2496-124">Add users in the wizard</span></span>

<span data-ttu-id="e2496-125">Kaikille ohjatussa toiminnossa lisäämiesi käyttäjien käyttöön määritetään automaattisesti Microsoft 365 Business Premium -käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="e2496-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Näyttökuva ohjatun toiminnon Lisää uusia käyttäjiä -sivusta](../media/addnewuserspage.png)

1. <span data-ttu-id="e2496-127">Jos Microsoft 365 Business Premium -tilauksessasi on aiemmin luotuja käyttäjiä (jos olet esimerkiksi käyttänyt Azure AD Connectia), voit määrittää heille käyttöoikeuksia nyt.</span><span class="sxs-lookup"><span data-stu-id="e2496-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="e2496-128">Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="e2496-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="e2496-129">Kun olet lisännyt käyttäjät, voit myös jakaa tunnistetiedot lisäätyille uusille käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="e2496-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="e2496-130">Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.</span><span class="sxs-lookup"><span data-stu-id="e2496-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="e2496-131">Toimialueen yhdistäminen</span><span class="sxs-lookup"><span data-stu-id="e2496-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="e2496-132">Jos päätit käyttää .onmicrosoft-toimialuetta tai määrittänyt käyttäjiä Azure AD Connectin avulla, et näe tätä vaihetta.</span><span class="sxs-lookup"><span data-stu-id="e2496-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="e2496-133">Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.</span><span class="sxs-lookup"><span data-stu-id="e2496-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="e2496-134">Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa.</span><span class="sxs-lookup"><span data-stu-id="e2496-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="e2496-135">Jos näin ei ole, [muuta nimipalvelimet niin, että Microsoft 365 määritetään minkä tahansa toimialuerekisteröijän kanssa.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md)</span><span class="sxs-lookup"><span data-stu-id="e2496-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md).</span></span> 

    - <span data-ttu-id="e2496-136">Jos sinulla on aiemmin luotuja DNS-tietueita, esimerkiksi aiemmin luotu verkkosivusto, mutta DNS-isännöintipalvelusi on otettu käyttöön [toimialueen](/office365/admin/get-help-with-domains/domain-connect)yhteydessä, valitse **Lisää tietueet minulle.**</span><span class="sxs-lookup"><span data-stu-id="e2496-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="e2496-137">Hyväksy **Valitse verkkopalvelut -sivulla** kaikki oletusasetukset, valitse Seuraava  ja valitse DNS-isännöintipalvelun sivulla Valtuuta.</span><span class="sxs-lookup"><span data-stu-id="e2496-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="e2496-138">Jos sinulla on olemassa olevia DNS-tietueita muiden DNS-isännöintipalvelujen kanssa (ei otettu käyttöön toimialueen yhdistettynä), sinun on hallittava omia DNS-tietueitasi ja varmistaa, että olemassa olevat palvelut ovat yhteydessä toisiinsa.</span><span class="sxs-lookup"><span data-stu-id="e2496-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="e2496-139">Lisätietoja on toimialueen perustoimialueissa. [](/office365/admin/get-help-with-domains/dns-basics)</span><span class="sxs-lookup"><span data-stu-id="e2496-139">See [domain basics](/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Aktivoi tietueet -sivu.](../media/activaterecords.png)

2. <span data-ttu-id="e2496-141">Noudata ohjatun toiminnon ohjeita, ja sähköposti ja muut palvelut määritetään sinulle.</span><span class="sxs-lookup"><span data-stu-id="e2496-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="e2496-142">Suojaa organisaatiosi</span><span class="sxs-lookup"><span data-stu-id="e2496-142">Protect your organization</span></span> 

<span data-ttu-id="e2496-143">Ohjatussa toiminnossa määritettyjä käytäntöjä käytetään automaattisesti Kaikki käyttäjät [-käyttöoikeusryhmässä.](/office365/admin/create-groups/compare-groups#security-groups) </span><span class="sxs-lookup"><span data-stu-id="e2496-143">The policies you set up in the wizard are applied automatically to a [Security group](/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="e2496-144">Voit myös luoda muita ryhmiä, jotta voit määrittää käytäntöjä hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="e2496-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="e2496-145">**Edistyneiltä** kyberuhkilta suojauksen lisäämisen osalta on suositeltavaa hyväksyä oletusasetukset, jotta [Office 365 Advance Threat Protection](../security/defender-365-security/defender-for-office-365.md) -sovelluksen tiedostot ja linkit voidaan tarkistaa Office-sovelluksissa.</span><span class="sxs-lookup"><span data-stu-id="e2496-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](../security/defender-365-security/defender-for-office-365.md) scan files and links in Office apps.</span></span>

    ![Näyttökuva Suurenna suojausta -sivusta.](../media/increasetreatprotection.png)


2. <span data-ttu-id="e2496-147">Hyväksy **Estä** luottamuksellisten tietojen vuodot -sivulla oletusarvot, joilla Office 365:n tietojen menetyksen estäminen (DLP) voidaan ottaa käyttöön, jotta voit seurata luottamuksellisia tietoja Office-sovelluksissa ja estää niiden tahattoman jakamisen organisaation ulkopuolelle.</span><span class="sxs-lookup"><span data-stu-id="e2496-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="e2496-148">Jätä Suojaa **tiedot Officen** mobiiliversiossa -sivulla mobiilisovellusten hallinta käyttöön, laajenna asetuksia ja tarkista ne ja valitse sitten Luo **mobiilisovelluksen hallintakäytäntö.**</span><span class="sxs-lookup"><span data-stu-id="e2496-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Näyttökuva Suojaa tiedot Office for Mobile -sivulla.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="e2496-150">Windows 10 -tietokoneiden suojaaminen</span><span class="sxs-lookup"><span data-stu-id="e2496-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="e2496-151">Valitse vasemmassa siirtymisruudussa **Asetukset** ja valitse sitten Sisäänkirjautuminen ja suojaus **-kohdassa** **Suojaa Windows 10 -tietokoneet.**</span><span class="sxs-lookup"><span data-stu-id="e2496-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="e2496-152">Aloita **valitsemalla** Näytä.</span><span class="sxs-lookup"><span data-stu-id="e2496-152">Choose **View** to get started.</span></span> <span data-ttu-id="e2496-153">Katso [täydelliset ohjeet Windows 10 -tietokoneiden](secure-win-10-pcs.md) suojaamista varten.</span><span class="sxs-lookup"><span data-stu-id="e2496-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="e2496-154">Office 365 -asiakassovellusten käyttöönotto</span><span class="sxs-lookup"><span data-stu-id="e2496-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="e2496-155">Jos päätit asentaa Office-sovellukset automaattisesti asennuksen aikana, sovellukset asennetaan Windows 10 -laitteisiin, kun käyttäjät ovat kirjautuneet Azure AD:lle Windows-laitteistaan työtunnuksilla.</span><span class="sxs-lookup"><span data-stu-id="e2496-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="e2496-156">Lisätietoja Officen asentamisesta iOS- tai Android-mobiililaitteisiin on kohdassa Mobiililaitteiden asentaminen [Microsoft 365 Business Premium -käyttäjille.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="e2496-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="e2496-157">Voit asentaa Officen myös yksitellen.</span><span class="sxs-lookup"><span data-stu-id="e2496-157">You can also install Office individually.</span></span> <span data-ttu-id="e2496-158">Katso [ohjeet Officen asentamisesta PC- tai Mac-tietokoneeseen.](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658)</span><span class="sxs-lookup"><span data-stu-id="e2496-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="e2496-159">Tutustu myös seuraaviin ohjeartikkeleihin:</span><span class="sxs-lookup"><span data-stu-id="e2496-159">See also</span></span>

[<span data-ttu-id="e2496-160">Microsoft 365 for Business -koulutusvideot</span><span class="sxs-lookup"><span data-stu-id="e2496-160">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
