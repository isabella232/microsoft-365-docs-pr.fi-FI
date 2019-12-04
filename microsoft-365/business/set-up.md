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
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Lue lisä tietoja Microsoft 365 Businessin määrittämisestä.
ms.openlocfilehash: 0001c2b9962f6cce0be1f77cbf427c68f9ee3249
ms.sourcegitcommit: c5ca71d6feb0f033b50ccd4de816fd59b0925007
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/04/2019
ms.locfileid: "39831299"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="771f6-103">Microsoft 365-liike toiminnan määrittäminen ohjatussa asennus toiminnossa</span><span class="sxs-lookup"><span data-stu-id="771f6-103">Set up Microsoft 365 Business in the setup wizard</span></span>

<span data-ttu-id="771f6-104">Katso tästä videosta yleiskatsaus Microsoft 365-liike toiminnan asennukseen.</span><span class="sxs-lookup"><span data-stu-id="771f6-104">Watch this video for an overview of Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

<span data-ttu-id="771f6-105">Jos olet löytänyt tämän videon hyödyllisiksi, tutustu [koko koulutus sarjaan pien yrityksille ja niille, jotka ovat Microsoft 365-yrityksen uusia](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="771f6-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="771f6-106">Lisää toimi alue, käyttäjät ja määritä käytännöt</span><span class="sxs-lookup"><span data-stu-id="771f6-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="771f6-107">[![Selite, jossa ilmoitetaan, että hallintakeskus muuttuu. Lisätietoja löytyy osoitteesta aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="771f6-107">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="771f6-108">Kun ostat Microsoft 365 Businessin, sinulla on mahdollisuus käyttää omistamaani verkko tunnusta tai ostaa se [rekisteröityessäsi](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="771f6-108">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="771f6-109">Jos olet hankkinut uuden verkko tunnuksen, kun olet rekisteröitynyt, toimi alueesi on määritetty ja voit siirtyä lisäämään [käyttäjiä ja määrittämään lisenssejä](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="771f6-109">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="771f6-110">Lisää verkko tunnuksesi mukauttamaan sisäänkirjautumista</span><span class="sxs-lookup"><span data-stu-id="771f6-110">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="771f6-111">Kirjaudu sisään [Microsoft 365-hallinta keskukseen](https://admin.microsoft.com) käyttämällä yleisiä järjestelmänvalvojan tunniste tietoja.</span><span class="sxs-lookup"><span data-stu-id="771f6-111">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="771f6-112">Käynnistä ohjattu toiminto valitsemalla **Siirry asennukseen** .</span><span class="sxs-lookup"><span data-stu-id="771f6-112">Choose **Go to setup** to start the wizard.</span></span>

    ![Valitse Siirry asennukseen.](media/gotosetupinadmincenter.png)

3. <span data-ttu-id="771f6-114">Voit vaihtoehtoisesti asentaa sovellukset omaan tieto koneeseesi **Asenna Office-sovellukset** -sivulla.</span><span class="sxs-lookup"><span data-stu-id="771f6-114">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="771f6-115">Kirjoita **Lisää toimi alue** -vaiheeseen toimi alue nimi, jota haluat käyttää (kuten contoso.com).</span><span class="sxs-lookup"><span data-stu-id="771f6-115">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="771f6-116">Jos ostit verkko tunnuksen rekisteröitymistä varten, et näe **Lisää toimi** alue-vaihetta tässä.</span><span class="sxs-lookup"><span data-stu-id="771f6-116">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="771f6-117">Siirry sen sijaan kohtaan [Lisää käyttäjiä](#add-users-and-assign-licenses) .</span><span class="sxs-lookup"><span data-stu-id="771f6-117">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Kuva kaappaus Mukauta kirjautumissivua.](media/adddomain.png)

    
4. <span data-ttu-id="771f6-119">Noudata ohjatun toiminnon ohjeita [luodaksesi DNS-tietueet missä tahansa DNS-isännöinti palvelun tarjoajana (Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) ), joka varmistaa, että omistat toimi alueen.</span><span class="sxs-lookup"><span data-stu-id="771f6-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="771f6-120">Jos tiedät verkko tunnuksesi isäntäsi, Katso myös [isännän erityiset ohjeet](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="771f6-120">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="771f6-121">Jos hosting-palveluntarjoajasi on GoDaddy tai toinen isäntä, joka on otettu käyttöön [Domain Connectin](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)kanssa, prosessi on helppoa ja sinua pyydetään automaattisesti Kirjautu maan sisään ja anna Microsoftin todentaa se puolestasi.</span><span class="sxs-lookup"><span data-stu-id="771f6-121">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Valitse GoDaddy Confirm Access-sivulla Valtuuta.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="771f6-123">Lisää käyttäjiä ja määritä käyttöoikeuksia</span><span class="sxs-lookup"><span data-stu-id="771f6-123">Add users and assign licenses</span></span>

<span data-ttu-id="771f6-124">Voit lisätä käyttäjiä ohjatussa toiminnossa, mutta voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallinta keskukseen.</span><span class="sxs-lookup"><span data-stu-id="771f6-124">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="771f6-125">Lisäksi jos sinulla on paikallinen toimi alueen ohjaus kone, voit lisätä käyttäjiä [Azure AD Connectin](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)avulla.</span><span class="sxs-lookup"><span data-stu-id="771f6-125">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="771f6-126">Lisää käyttäjiä ohjatussa toiminnossa</span><span class="sxs-lookup"><span data-stu-id="771f6-126">Add users in the wizard</span></span>

<span data-ttu-id="771f6-127">Kaikki käyttäjät, jotka lisäät ohjatussa toiminnossa, saavat automaattisesti Microsoft 365-yritys käyttö oikeuden.</span><span class="sxs-lookup"><span data-stu-id="771f6-127">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Ohjatun toiminnon lisää uusia käyttäjiä-sivun kuva kaappaus](media/addnewuserspage.png)

1. <span data-ttu-id="771f6-129">Jos Microsoft 365-liiketoiminta tilauksessasi on aiemmin luotuja käyttäjiä (Jos esimerkiksi käytit Azure AD Connectia), saat mahdollisuuden määrittää heille käyttö oikeudet nyt.</span><span class="sxs-lookup"><span data-stu-id="771f6-129">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="771f6-130">Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="771f6-130">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="771f6-131">Kun olet lisännyt käyttäjät, saat myös mahdollisuuden jakaa tunniste tiedot lisättyjen uusien käyttäjien kanssa.</span><span class="sxs-lookup"><span data-stu-id="771f6-131">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="771f6-132">Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.</span><span class="sxs-lookup"><span data-stu-id="771f6-132">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="771f6-133">Toimialueen yhdistäminen</span><span class="sxs-lookup"><span data-stu-id="771f6-133">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="771f6-134">Jos valitsit. onmicrosoft-toimi alueen tai käytät Azure AD Connectia käyttäjien määrittämisestä, et näe tätä vaihetta.</span><span class="sxs-lookup"><span data-stu-id="771f6-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="771f6-135">Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.</span><span class="sxs-lookup"><span data-stu-id="771f6-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="771f6-136">Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa.</span><span class="sxs-lookup"><span data-stu-id="771f6-136">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="771f6-137">Jos näin ei ole, [Vaihda nimi palvelimet, jotta voit määrittää Office 365-palvelimen minkä tahansa toimi alueen rekisterin pitäjän kanssa](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="771f6-137">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="771f6-138">Jos sinulla on aiemmin luotuja DNS-tietueita, esimerkiksi olemassa oleva Web-sivusto, mutta DNS-isäntä on otettu käyttöön [toimi alueen yhdistämä](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), valitse **Lisää tietueita minulle**.</span><span class="sxs-lookup"><span data-stu-id="771f6-138">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="771f6-139">Hyväksy **Valitse online-palvelut** -sivulla kaikki oletus arvot, valitse **Seuraava** **ja valitse sitten Hyväksy DNS** -isännän sivulla.</span><span class="sxs-lookup"><span data-stu-id="771f6-139">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="771f6-140">Jos sinulla on DNS-tietueita muiden DNS-Isän tien kanssa (ei käytössä toimi alueen yhteydessä), sinun kannattaa hallita omia DNS-tietueita ja varmistaa, että olemassa olevat palvelut ovat yhteydessä toisiinsa.</span><span class="sxs-lookup"><span data-stu-id="771f6-140">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="771f6-141">Lisä tietoja on kohdassa [toimi alueen perusteet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .</span><span class="sxs-lookup"><span data-stu-id="771f6-141">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Aktivoi tietueet-sivu.](media/activaterecords.png)

2. <span data-ttu-id="771f6-143">Noudata ohjatun toiminnon ohjeita, ja Sähkö posti ja muut palvelut määritetään puolestasi.</span><span class="sxs-lookup"><span data-stu-id="771f6-143">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="771f6-144">Organisaation suojaaminen</span><span class="sxs-lookup"><span data-stu-id="771f6-144">Protect your organization</span></span> 

<span data-ttu-id="771f6-145">Ohjatussa toiminnossa käyttöön luomat käytännöt kohdistetaan automaattisesti [Suojaus ryhmään](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) nimeltä *Kaikki käyttäjät*.</span><span class="sxs-lookup"><span data-stu-id="771f6-145">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="771f6-146">Voit myös luoda lisä ryhmiä määrittämään käytäntöjä hallinta keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="771f6-146">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="771f6-147">**Lisä suojaa kehittyneiltä kyberuhkilta**suositellaan, että hyväksyt oletus asetukset, jotta [Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) -tieto turva tarkistus tiedostot ja linkit Office-sovelluksissa hyväksytään.</span><span class="sxs-lookup"><span data-stu-id="771f6-147">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Kuva kaappaus lisää suojausta-sivulta.](media/increasetreatprotection.png)


2. <span data-ttu-id="771f6-149">Hyväksy **arkaluontoisten tietojen vuodot** -sivun oletus asetukset, jos haluat ottaa Office 365-tietojen menetyksen eston (DLP) käyttöön, jotta voit seurata luottamuksellisia tietoja Office-sovelluksissa ja estää niiden tahattoman jakamisen organisaatiosi ulkopuolella.</span><span class="sxs-lookup"><span data-stu-id="771f6-149">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="771f6-150">Jätä Mobile-sovelluksen hallinta päälle, Laajenna asetukset ja tarkista ne ja valitse sitten **Luo mobiilisovelluksen hallinta käytäntö**, jos **haluat suojata Officen mobiiliverdauksen tiedot** -sivulla.</span><span class="sxs-lookup"><span data-stu-id="771f6-150">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Kuva kaappaus Office for Mobile-sivun tietojen suojaamisesta.](media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="771f6-152">Secure Windows 10-tieto koneet</span><span class="sxs-lookup"><span data-stu-id="771f6-152">Secure Windows 10 PCs</span></span>

<span data-ttu-id="771f6-153">Valitse vasemmasta siirtymis kohdasta **Asetukset** ja valitse sitten **Sing-in ja Security**-kohdasta **suojaa Windows 10-tieto koneesi**.</span><span class="sxs-lookup"><span data-stu-id="771f6-153">On the left nav, select **Setup** and then, under **Sing-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="771f6-154">Pääset alkuun valitsemalla **Näytä** .</span><span class="sxs-lookup"><span data-stu-id="771f6-154">Choose **View** to get started.</span></span> <span data-ttu-id="771f6-155">Katso täydelliset ohjeet kohdasta [Windows 10-tieto koneiden suojaaminen](secure-win-10-pcs.md) .</span><span class="sxs-lookup"><span data-stu-id="771f6-155">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="771f6-156">Office 365-asiakas sovellusten käyttöönotto</span><span class="sxs-lookup"><span data-stu-id="771f6-156">Deploy Office 365 client apps</span></span>

<span data-ttu-id="771f6-157">Jos valitsit, että Office-sovellukset asennetaan asennuksen aikana automaattisesti, sovellukset asennetaan Windows 10-laitteisiin sen jälkeen, kun käyttäjät ovat kirjauduneet sisään Azure ADIIN Windows-laitteistaan käyttämällä työn tunniste tietoja.</span><span class="sxs-lookup"><span data-stu-id="771f6-157">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="771f6-158">Jos haluat asentaa Officen mobiililaitteisiin iOS-tai Android-laitteisiin, katso [Microsoft 365-yritys käyttäjien mobiililaitteiden määrittäminen](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="771f6-158">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="771f6-159">Voit myös asentaa Officen yksitellen.</span><span class="sxs-lookup"><span data-stu-id="771f6-159">You can also install Office individually.</span></span> <span data-ttu-id="771f6-160">Katso ohjeet [Officen asentamisesta PC:hen tai Maciin](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .</span><span class="sxs-lookup"><span data-stu-id="771f6-160">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="771f6-161">Katso myös</span><span class="sxs-lookup"><span data-stu-id="771f6-161">See also</span></span>

[<span data-ttu-id="771f6-162">Microsoft 365-liike toiminnan koulutus videot</span><span class="sxs-lookup"><span data-stu-id="771f6-162">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
