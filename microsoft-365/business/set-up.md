---
title: Microsoft 365 Businessin määrittäminen
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Tutustu Microsoft 365 Businessin asennusvaiheisiin, kuten toimialueen ja käyttäjien lisäämiseen, suojauskäytäntöjen määrittämiseen ja masennukseen.
ms.openlocfilehash: 4535a32b579b91b6c2bb0e64ec95904be6c08fce
ms.sourcegitcommit: 6c8edbc54b193e964cf93aec48c51cb79231f1d9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2020
ms.locfileid: "42543935"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="7ec8e-103">Microsoft 365 Businessin määrittäminen ohjatussa asennustoiminnossa</span><span class="sxs-lookup"><span data-stu-id="7ec8e-103">Set up Microsoft 365 Business in the setup wizard</span></span>

<span data-ttu-id="7ec8e-104">Tämä video on yleiskuvaus Microsoft 365 Businessin asennuksesta.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-104">Watch this video for an overview of Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

<span data-ttu-id="7ec8e-105">Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="7ec8e-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="7ec8e-106">Toimialueen, käyttäjien ja käytäntöjen määrittäminen</span><span class="sxs-lookup"><span data-stu-id="7ec8e-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="7ec8e-107">[![Selite, jossa ilmoitetaan, että hallintakeskus muuttuu. Lisätietoja löytyy osoitteesta aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="7ec8e-107">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="7ec8e-108">Kun ostat Microsoft 365 Businessin, voit käyttää omistamaasi toimialuetta tai ostaa sen [rekisteröitymisen](sign-up.md)aikana.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-108">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="7ec8e-109">Jos ostit uuden toimialueen rekisteröityessäsi, toimialueesi on määritetty ja voit siirtyä [Lisää käyttäjiä -kohtaan ja määrittää käyttöoikeuksia](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="7ec8e-109">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="7ec8e-110">Toimialueen lisääminen kirjautumisen mukauttamiseksi</span><span class="sxs-lookup"><span data-stu-id="7ec8e-110">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="7ec8e-111">Kirjaudu [Microsoft 365 -hallintakeskukseen](https://admin.microsoft.com) käyttämällä yleisiä järjestelmänvalvojan tunnistetietoja.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-111">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="7ec8e-112">Käynnistä ohjattu toiminto valitsemalla **Siirry asennukseen.**</span><span class="sxs-lookup"><span data-stu-id="7ec8e-112">Choose **Go to setup** to start the wizard.</span></span>

    ![Valitse Siirry asennukseen.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="7ec8e-114">Asenna **Office-sovellukset -sivulla** voit halutessasi asentaa sovellukset omaan tietokoneeseesi.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-114">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="7ec8e-115">Kirjoita **Lisää toimialue** -vaiheeseen haluamasi toimialueen nimi (kuten contoso.com).</span><span class="sxs-lookup"><span data-stu-id="7ec8e-115">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="7ec8e-116">Jos ostit toimialueen rekisteröitymisen aikana, lisää **toimialuevaihe** ei näy tässä.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-116">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="7ec8e-117">Siirry sen sijaan [kohtaan Käyttäjien lisääminen.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="7ec8e-117">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Näyttökuva Mukauta kirjautumista -sivusta.](../media/adddomain.png)

    
4. <span data-ttu-id="7ec8e-119">Luo [DNS-tietueita missä tahansa Office 365:n DNS-isännöintipalvelussa](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) ohjatun toiminnon ohjeiden mukaisesti, mikä tarkistaa toimialueen omistavan.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="7ec8e-120">Jos tunnet verkkotunnuksen isännän, katso myös [isäntäkohtaiset ohjeet](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="7ec8e-120">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="7ec8e-121">Jos isännöintipalvelusi on GoDaddy tai toinen isäntä, joka on otettu käyttöön [toimialueen yhteyden muodostamisen](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)yhteydessä , prosessi on helppo ja sinua pyydetään kirjautumaan sisään ja antamaan Microsoftin todentaa henkilöllisyytesi puolestasi.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-121">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Valitse GoDaddyConfirm Access (Vahvista käyttöoikeus) -sivulla Valtuuta.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="7ec8e-123">Lisää käyttäjiä ja määritä käyttöoikeuksia</span><span class="sxs-lookup"><span data-stu-id="7ec8e-123">Add users and assign licenses</span></span>

<span data-ttu-id="7ec8e-124">Voit lisätä käyttäjiä ohjattuun toimintoon, mutta voit [myös lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallintakeskukseen.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-124">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="7ec8e-125">Lisäksi jos sinulla on paikallinen toimialueen ohjauskone, voit lisätä käyttäjiä [Azure AD Connectin](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)avulla.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-125">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="7ec8e-126">Käyttäjien lisääminen ohjattuun toimintoon</span><span class="sxs-lookup"><span data-stu-id="7ec8e-126">Add users in the wizard</span></span>

<span data-ttu-id="7ec8e-127">Kaikki ohjatussa toiminnossa lisäämäsi käyttäjät saavat automaattisesti Microsoft 365 Business -käyttöoikeuden.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-127">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Näyttökuva ohjatun toiminnon Lisää uusia käyttäjiä -sivusta](../media/addnewuserspage.png)

1. <span data-ttu-id="7ec8e-129">Jos Microsoft 365 Business -tilauksessasi on olemassa olevia käyttäjiä (esimerkiksi jos käytit Azure AD Connectia), voit määrittää heille käyttöoikeudet nyt.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-129">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="7ec8e-130">Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-130">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="7ec8e-131">Kun olet lisännyt käyttäjät, voit myös jakaa tunnistetiedot lisäämäsi uusien käyttäjien kanssa.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-131">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="7ec8e-132">Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-132">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="7ec8e-133">Toimialueen yhdistäminen</span><span class="sxs-lookup"><span data-stu-id="7ec8e-133">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="7ec8e-134">Jos valitsit .onmicrosoft-toimialueen käyttämisen tai käytät Azure AD Connectia käyttäjien määrittämiseen, et näe tätä vaihetta.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="7ec8e-135">Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="7ec8e-136">Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-136">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="7ec8e-137">Jos näin ei ole, [Muuta nimipalvelimia niin, että Office 365 määritetään minkä tahansa toimialueen rekisteröintipalvelun kanssa.](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2)</span><span class="sxs-lookup"><span data-stu-id="7ec8e-137">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="7ec8e-138">Jos sinulla on aiemmin luotuja DNS-tietueita, esimerkiksi aiemmin luotu web-sivusto, mutta DNS-isäntä on käytössä [toimialueen yhdistämisessä](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), valitse **Lisää tietueita minulle**.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-138">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="7ec8e-139">Hyväksy **Valitse verkkopalvelut** -sivulla kaikki oletusarvot ja valitse **Seuraava**ja valitse DNS-isännän sivulla **Valtuuta.**</span><span class="sxs-lookup"><span data-stu-id="7ec8e-139">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="7ec8e-140">Jos sinulla on aiemmin luotuja DNS-tietueita muiden DNS-isäntien kanssa (ei otettu käyttöön toimialueen yhdistämisessä), sinun kannattaa hallita omia DNS-tietueitasi ja varmistaa, että olemassa olevat palvelut pysyvät yhteydessä toisiinsa.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-140">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="7ec8e-141">Lisätietoja on [verkkotunnuksen perustiedoissa.](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics)</span><span class="sxs-lookup"><span data-stu-id="7ec8e-141">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Aktivoi tietuesivu.](../media/activaterecords.png)

2. <span data-ttu-id="7ec8e-143">Noudata ohjatun toiminnon ohjeita, ja sähköposti ja muut palvelut määritetään puolestasi.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-143">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="7ec8e-144">Suojaa organisaatiosi</span><span class="sxs-lookup"><span data-stu-id="7ec8e-144">Protect your organization</span></span> 

<span data-ttu-id="7ec8e-145">Ohjatussa toiminnossa määritetyt käytännöt otetaan automaattisesti käyttöön *Kaikki käyttäjät* [-suojausryhmässä.](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups)</span><span class="sxs-lookup"><span data-stu-id="7ec8e-145">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="7ec8e-146">Voit myös luoda muita ryhmiä, joihin käytännöt määritetään hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-146">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="7ec8e-147">**Lisäsuojaa kehittyneiltä kyberuhkilta**-kohdassa on suositeltavaa hyväksyä oletusarvot, joiden avulla [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) voi skannata tiedostoja ja linkkejä Office-sovelluksissa.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-147">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Näyttökuva Lisää suojaus -sivusta.](../media/increasetreatprotection.png)


2. <span data-ttu-id="7ec8e-149">Hyväksy **Estä arkaluonteisten tietojen vuodot** -sivulla oletukset, joiden mukaan Office 365 Data Loss Prevention (DLP) ottaa käyttöön arkaluonteisten tietojen seuraamiseksi Office-sovelluksissa ja estääksesi niiden tahattoman jakamisen organisaation ulkopuolella.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-149">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="7ec8e-150">Jätä **Suojaa tiedot Office mobiililaitteille -sivulla** mobiilisovellusten hallinta päälle, laajenna asetukset ja tarkista ne ja valitse sitten **Luo mobiilisovellusten hallintakäytäntö**.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-150">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Näyttökuva Suojaa tiedot Office mobiililaitteille -sivulla.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="7ec8e-152">Suojaa Windows 10 -tietokoneet</span><span class="sxs-lookup"><span data-stu-id="7ec8e-152">Secure Windows 10 PCs</span></span>

<span data-ttu-id="7ec8e-153">Valitse vasemmassa siirtymisruudussa **Asetukset** ja valitse sitten **Sing-in ja security (Suojaa** **Windows 10 -tietokoneet)**-kohdasta.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-153">On the left nav, select **Setup** and then, under **Sing-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="7ec8e-154">Aloita valitsemalla **Näytä.**</span><span class="sxs-lookup"><span data-stu-id="7ec8e-154">Choose **View** to get started.</span></span> <span data-ttu-id="7ec8e-155">Katso täydelliset ohjeet [noudattamalla Windows 10 -tietokoneiden suojaaminen.](secure-win-10-pcs.md)</span><span class="sxs-lookup"><span data-stu-id="7ec8e-155">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="7ec8e-156">Office 365 -asiakassovellusten käyttöönotto</span><span class="sxs-lookup"><span data-stu-id="7ec8e-156">Deploy Office 365 client apps</span></span>

<span data-ttu-id="7ec8e-157">Jos valitsit Office-sovellusten automaattisen asennuksen asennuksen aikana, sovellukset asennetaan Windows 10 -laitteisiin, kun käyttäjät ovat kirjautuneet Azure AD:hen Windows-laitteistaan käyttämällä työtunnistetietojaan.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-157">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="7ec8e-158">Lisätietoja Officen asentamisesta mobiili-iOS- tai Android-laitteisiin on ohjeaiheessa [Mobiililaitteiden määrittäminen Microsoft 365 Business -käyttäjille](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="7ec8e-158">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="7ec8e-159">Voit asentaa Officen myös yksitellen.</span><span class="sxs-lookup"><span data-stu-id="7ec8e-159">You can also install Office individually.</span></span> <span data-ttu-id="7ec8e-160">Katso ohjeet [artikkelista Officen asentaminen PC- tai Mac-tietokoneeseen.](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658)</span><span class="sxs-lookup"><span data-stu-id="7ec8e-160">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="7ec8e-161">Tutustu myös seuraaviin ohjeaiheisiin</span><span class="sxs-lookup"><span data-stu-id="7ec8e-161">See also</span></span>

[<span data-ttu-id="7ec8e-162">Microsoft 365 Business -koulutusvideot</span><span class="sxs-lookup"><span data-stu-id="7ec8e-162">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
