---
title: Microsoft 365 Business Premiumin määrittäminen
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
description: Tutustu Microsoft 365 Business Premiumin määritys vaiheisiin, joita ovat esimerkiksi toimi alueen ja käyttäjien lisääminen, tieto turva käytäntöjen määrittäminen ja paljon muuta.
ms.openlocfilehash: cc20637d7a78bd34ecb61a4ed46eb06d564d63df
ms.sourcegitcommit: 25afc0c34edc7f8a5eb389d8c701175256c58ec8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/01/2020
ms.locfileid: "47324492"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="01dab-103">Microsoft 365 Business Premiumin määrittäminen ohjatussa määritys toiminnossa</span><span class="sxs-lookup"><span data-stu-id="01dab-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="01dab-104">Katsomalla tämän videon saat yleiskatsauksen Microsoft 365 Business Premium-asennuksesta.</span><span class="sxs-lookup"><span data-stu-id="01dab-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="01dab-105">Toimi alueen, käyttäjien ja käytäntöjen määrittäminen</span><span class="sxs-lookup"><span data-stu-id="01dab-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="01dab-106">Kun ostat Microsoft 365 Business Premiumin, sinulla on mahdollisuus käyttää omaa toimi aluettasi tai ostaa se [rekisteröitymisen](sign-up.md)yhteydessä.</span><span class="sxs-lookup"><span data-stu-id="01dab-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="01dab-107">Jos olet ostanut uuden toimi alueen rekisteröityessäsi, toimi alueesi on määritetty ja voit siirtyä [käyttäjien lisäämiseen ja käyttö oikeuksien määrittämiseen](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="01dab-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="01dab-108">Toimi alueen lisääminen kirjautumisen mukauttamiseen</span><span class="sxs-lookup"><span data-stu-id="01dab-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="01dab-109">Kirjaudu sisään [Microsoft 365-hallinta keskukseen](https://admin.microsoft.com) käyttämällä yleisiä järjestelmänvalvojan tunniste tietoja.</span><span class="sxs-lookup"><span data-stu-id="01dab-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="01dab-110">Käynnistä ohjattu toiminto valitsemalla **Siirry asetuksiin** .</span><span class="sxs-lookup"><span data-stu-id="01dab-110">Choose **Go to setup** to start the wizard.</span></span>

    ![Valitse Siirry asetuksiin.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="01dab-112">**Asenna Office-sovellukset** -sivulla voit halutessasi asentaa sovellukset omaan tieto koneeseesi.</span><span class="sxs-lookup"><span data-stu-id="01dab-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="01dab-113">Kirjoita **Lisää toimi alue** -vaiheeseen haluamasi toimi alueen nimi (esimerkiksi contoso.com).</span><span class="sxs-lookup"><span data-stu-id="01dab-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="01dab-114">Jos ostit toimi alueen rekisteröitymisen aikana, et näe **Lisää toimi alue** vaihetta tässä.</span><span class="sxs-lookup"><span data-stu-id="01dab-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="01dab-115">Siirry kohtaan [Lisää käyttäjiä](#add-users-and-assign-licenses) .</span><span class="sxs-lookup"><span data-stu-id="01dab-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Näyttö kuva Mukauta kirjautumissivusi-sivusta.](../media/adddomain.png)

    
4. <span data-ttu-id="01dab-117">Noudattamalla ohjatun toiminnon ohjeita voit [luoda DNS-tietueita missä tahansa Microsoft 365-palvelun DNS-isännöinti palvelussa](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , joka vahvistaa, että omistat toimi alueen.</span><span class="sxs-lookup"><span data-stu-id="01dab-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="01dab-118">Jos tiedät toimi alueen isännältä, Katso myös [tarkat isännöinti ohjeet](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="01dab-118">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="01dab-119">Jos isännöinti palvelusi on GoDaddy tai jokin muu palvelin, jossa on käytössä [Domain Connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), prosessi on helppo, ja sinua pyydetään automaattisesti Kirjautu maan sisään ja päästämään Microsoft todennetaan puolestasi.</span><span class="sxs-lookup"><span data-stu-id="01dab-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Valitse GoDaddy-vahvistuksen käyttäminen-sivulla Valtuuta.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="01dab-121">Lisää käyttäjiä ja määritä käyttöoikeuksia</span><span class="sxs-lookup"><span data-stu-id="01dab-121">Add users and assign licenses</span></span>

<span data-ttu-id="01dab-122">Voit lisätä käyttäjiä ohjatussa toiminnossa, mutta voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallinta keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="01dab-122">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="01dab-123">Lisäksi jos sinulla on paikallinen toimi alueen ohjaus kone, voit lisätä käyttäjiä [Azure AD Connectin](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)avulla.</span><span class="sxs-lookup"><span data-stu-id="01dab-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="01dab-124">Käyttäjien lisääminen ohjatussa toiminnossa</span><span class="sxs-lookup"><span data-stu-id="01dab-124">Add users in the wizard</span></span>

<span data-ttu-id="01dab-125">Kaikki ohjatussa toiminnossa lisättävät käyttäjät saavat automaattisesti Microsoft 365 Business Premium-käyttö oikeuden.</span><span class="sxs-lookup"><span data-stu-id="01dab-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Näyttö kuva ohjatun toiminnon lisää uusia käyttäjiä-sivusta](../media/addnewuserspage.png)

1. <span data-ttu-id="01dab-127">Jos Microsoft 365 Business Premium-tilauksessasi on olemassa olevia käyttäjiä (jos olet esimerkiksi käyttänyt Azure AD Connectia), saat vaihto ehdon määrittää heille käyttö oikeuksia nyt.</span><span class="sxs-lookup"><span data-stu-id="01dab-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="01dab-128">Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="01dab-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="01dab-129">Kun olet lisännyt käyttäjät, saat myös mahdollisuuden jakaa tunniste tiedot lisäämiesi uusien käyttäjien kanssa.</span><span class="sxs-lookup"><span data-stu-id="01dab-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="01dab-130">Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.</span><span class="sxs-lookup"><span data-stu-id="01dab-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="01dab-131">Toimialueen yhdistäminen</span><span class="sxs-lookup"><span data-stu-id="01dab-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="01dab-132">Jos päätät käyttää. oMicrosoft-toimi aluetta tai käyttää Azure AD Connectia käyttäjien määrittämiseen, et näe tätä vaihetta.</span><span class="sxs-lookup"><span data-stu-id="01dab-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="01dab-133">Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.</span><span class="sxs-lookup"><span data-stu-id="01dab-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="01dab-134">Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa.</span><span class="sxs-lookup"><span data-stu-id="01dab-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="01dab-135">Jos näin ei tapahdu, [Muuta nimi palvelimia, jotta voit määrittää Microsoft 365 minkä tahansa toimi alueen rekisteröinti palvelun avulla](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span><span class="sxs-lookup"><span data-stu-id="01dab-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span></span> 

    - <span data-ttu-id="01dab-136">Jos sinulla on aiemmin luotuja DNS-tietueita, kuten aiemmin luotua sivustoa, mutta DNS-isäntä on otettu käyttöön [toimi alueen yhteydessä](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), valitse **Lisää tietueet**.</span><span class="sxs-lookup"><span data-stu-id="01dab-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="01dab-137">Hyväksy **Valitse online-palvelut** -sivulla kaikki oletus asetukset ja valitse sitten **Seuraava**ja valitse **Valtuuta** DNS-isännän sivulla.</span><span class="sxs-lookup"><span data-stu-id="01dab-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="01dab-138">Jos sinulla on aiemmin luotuja DNS-tietueita muiden DNS-Isän tien kanssa (ei otettu käyttöön toimi alueen yhteydessä), sinun kannattaa hallita omia DNS-tietueitasi ja varmistaa, että olemassa olevat palvelut pysyvät yhteydessä.</span><span class="sxs-lookup"><span data-stu-id="01dab-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="01dab-139">Lisä tietoja on kohdassa [toimi alueen perusteet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .</span><span class="sxs-lookup"><span data-stu-id="01dab-139">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Aktivoi tietueet-sivu.](../media/activaterecords.png)

2. <span data-ttu-id="01dab-141">Noudata ohjatun toiminnon ohjeita ja Sähkö posti ja muut palvelut määritetään puolestasi.</span><span class="sxs-lookup"><span data-stu-id="01dab-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="01dab-142">Organisaation suojaaminen</span><span class="sxs-lookup"><span data-stu-id="01dab-142">Protect your organization</span></span> 

<span data-ttu-id="01dab-143">Ohjatussa toiminnossa määritetyt käytännöt otetaan automaattisesti käyttöön *kaikille käyttäjille*- [käyttö oikeus ryhmälle](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) .</span><span class="sxs-lookup"><span data-stu-id="01dab-143">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="01dab-144">Voit myös luoda lisää ryhmiä, joiden avulla käytäntöjä voi määrittää hallinta keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="01dab-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="01dab-145">**Kehittyneiden cyber-uhkien lisä suojauksen**ansiosta on suositeltavaa, että hyväksyt oletus asetukset, joiden avulla voit antaa [Office 365 Advance Threat Protectionin](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) etsiä tiedostoja ja linkkejä Office-sovelluksissa.</span><span class="sxs-lookup"><span data-stu-id="01dab-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Näyttö kuva lisää suojaus-sivusta.](../media/increasetreatprotection.png)


2. <span data-ttu-id="01dab-147">Hyväksy luottamuksellisten tietojen **estäminen** -sivulla oletus asetukset, jotta voit ottaa Office 365-tietojen menetyksen estämisen (DLP) käyttöön, jotta voit jäljittämään luottamukselliset tiedot Office-sovelluksissa ja estää niiden tahattoman jakamisen organisaation ulkopuolelta.</span><span class="sxs-lookup"><span data-stu-id="01dab-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="01dab-148">**Jos haluat suojata tietoja Office mobiililaitteille** -sivulla, poistu mobiilisovellusten Hallin nasta, Laajenna asetukset ja tarkista ne ja valitse sitten **Luo mobiilisovelluksen hallinta käytännön**.</span><span class="sxs-lookup"><span data-stu-id="01dab-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Näyttö kuva tietojen suojaamisesta Office for Mobile-sivulla.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="01dab-150">Windows 10-tieto koneiden suojaaminen</span><span class="sxs-lookup"><span data-stu-id="01dab-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="01dab-151">Valitse vasemmanpuoleisessa siirtymis ruudussa **määritys** ja valitse sitten **Kirjautuminen ja suojaus**-kohdassa **suojaa Windows 10-tieto koneet**.</span><span class="sxs-lookup"><span data-stu-id="01dab-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="01dab-152">Aloita valitsemalla **Näytä** .</span><span class="sxs-lookup"><span data-stu-id="01dab-152">Choose **View** to get started.</span></span> <span data-ttu-id="01dab-153">Katso täydelliset ohjeet artikkelista [Windows 10-tieto koneen suojaaminen](secure-win-10-pcs.md) .</span><span class="sxs-lookup"><span data-stu-id="01dab-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="01dab-154">Office 365-asiakas sovellusten käyttöönotto</span><span class="sxs-lookup"><span data-stu-id="01dab-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="01dab-155">Jos valitsit Office-sovellusten automaattisen asentamisen asennuksen aikana, sovellukset asennetaan Windows 10-laitteisiin, kun käyttäjät ovat kirjautuneet Azure AD:hen Windows-laitteistaan heidän työtunniste tiedoillaan.</span><span class="sxs-lookup"><span data-stu-id="01dab-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="01dab-156">Jos haluat asentaa Officen mobiililaitteeseen iOS-tai Android-laitteisiin, Katso lisä tietoja artikkelista [mobiililaitteiden määrittäminen Microsoft 365 Business Premium-käyttäjille](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="01dab-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="01dab-157">Voit myös asentaa Officen yksitellen.</span><span class="sxs-lookup"><span data-stu-id="01dab-157">You can also install Office individually.</span></span> <span data-ttu-id="01dab-158">Katso ohjeet artikkelista [Officen asentaminen PC-tai Mac-tieto koneeseen](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) .</span><span class="sxs-lookup"><span data-stu-id="01dab-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="01dab-159">Tutustu myös seuraaviin ohjeartikkeleihin:</span><span class="sxs-lookup"><span data-stu-id="01dab-159">See also</span></span>

[<span data-ttu-id="01dab-160">Microsoft 365 for Business-koulutus videot</span><span class="sxs-lookup"><span data-stu-id="01dab-160">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
