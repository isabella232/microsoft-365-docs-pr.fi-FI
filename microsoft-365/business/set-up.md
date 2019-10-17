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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Lue lisä tietoja Microsoft 365 Businessin määrittämisestä.
ms.openlocfilehash: cd59570cbcb9b027780e160117b44be88770d6b9
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575544"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="06f1b-103">Microsoft 365-liike toiminnan määrittäminen ohjatussa asennus toiminnossa</span><span class="sxs-lookup"><span data-stu-id="06f1b-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="06f1b-104">Lisää toimi alue, käyttäjät ja määritä käytännöt</span><span class="sxs-lookup"><span data-stu-id="06f1b-104">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="06f1b-105">[![Etiketti, jonka avulla voit tietää, että hallinta keskus on muuttumassa ja löydät lisä tietoja osoitteessa aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="06f1b-105">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="06f1b-106">Kun ostat Microsoft 365 Businessin, sinulla on mahdollisuus käyttää omistamaani verkko tunnusta tai ostaa se [rekisteröityessäsi](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="06f1b-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="06f1b-107">Jos olet hankkinut uuden verkko tunnuksen, kun olet rekisteröitynyt, toimi alueesi on määritetty ja voit siirtyä lisäämään [käyttäjiä ja määrittämään lisenssejä](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="06f1b-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="06f1b-108">Lisää verkko tunnuksesi mukauttamaan sisäänkirjautumista</span><span class="sxs-lookup"><span data-stu-id="06f1b-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="06f1b-109">Kirjaudu sisään [Microsoft 365-hallinta keskukseen](https://admin.microsoft.com) käyttämällä yleisiä järjestelmänvalvojan tunniste tietoja.</span><span class="sxs-lookup"><span data-stu-id="06f1b-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="06f1b-110">Käynnistä ohjattu toiminto valitsemalla **Lisää toimi alue** tai **Lisää käyttäjiä** .</span><span class="sxs-lookup"><span data-stu-id="06f1b-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="06f1b-111">Jos ostit verkko tunnuksen rekisteröitymistä varten, et näe **Lisää toimi** alue-vaihetta tässä.</span><span class="sxs-lookup"><span data-stu-id="06f1b-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="06f1b-112">Siirry sen sijaan kohtaan [Lisää käyttäjiä](#add-users-and-assign-licenses) .</span><span class="sxs-lookup"><span data-stu-id="06f1b-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Valitse Siirry asennukseen.](media/gotosetupinadmincenter.png)
    
3. <span data-ttu-id="06f1b-114">Kirjoita ohjatussa toiminnossa haluamasi toimi alueen nimi (kuten contoso.com).</span><span class="sxs-lookup"><span data-stu-id="06f1b-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Kuva kaappaus Mukauta kirjautumissivua.](media/personalizesignin.png)

    
4. <span data-ttu-id="06f1b-116">Noudata ohjatun toiminnon ohjeita [luodaksesi DNS-tietueet missä tahansa DNS-isännöinti palvelun tarjoajana (Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) ), joka varmistaa, että omistat toimi alueen.</span><span class="sxs-lookup"><span data-stu-id="06f1b-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="06f1b-117">Jos tiedät verkko tunnuksesi isäntäsi, Katso myös [isännän erityiset ohjeet](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="06f1b-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="06f1b-118">Jos palveluntarjoajasi on GoDaddy tai toinen isäntä, joka on otettu käyttöön [Domain Connectin](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)kanssa, prosessi on helppoa ja sinua pyydetään automaattisesti Kirjautu maan sisään ja anna Microsoftin todentaa se puolestasi:</span><span class="sxs-lookup"><span data-stu-id="06f1b-118">If your hosting provider is GoDaddy, or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![Valitse GoDaddy Confirm Access-sivulla Valtuuta.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="06f1b-120">Lisää käyttäjiä ja määritä käyttöoikeuksia</span><span class="sxs-lookup"><span data-stu-id="06f1b-120">Add users and assign licenses</span></span>

<span data-ttu-id="06f1b-121">Voit lisätä käyttäjiä ohjatussa toiminnossa, mutta voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallinta keskukseen.</span><span class="sxs-lookup"><span data-stu-id="06f1b-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="06f1b-122">Lisäksi jos sinulla on paikallinen toimi alueen ohjaus kone, voit lisätä käyttäjiä [Azure AD Connectin](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)avulla.</span><span class="sxs-lookup"><span data-stu-id="06f1b-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="06f1b-123">Lisää käyttäjiä ohjatussa toiminnossa</span><span class="sxs-lookup"><span data-stu-id="06f1b-123">Add users in the wizard</span></span>

<span data-ttu-id="06f1b-124">Kaikki käyttäjät, jotka lisäät ohjatussa toiminnossa, saavat automaattisesti Microsoft 365-yritys käyttö oikeuden.</span><span class="sxs-lookup"><span data-stu-id="06f1b-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Ohjatun toiminnon lisää uusia käyttäjiä-sivun kuva kaappaus](media/addnewuserspage.png)

1. <span data-ttu-id="06f1b-126">Jos Microsoft 365-liiketoiminta tilauksessasi on aiemmin luotuja käyttäjiä (Jos esimerkiksi käytit Azure AD Connectia), saat mahdollisuuden määrittää heille käyttö oikeudet nyt.</span><span class="sxs-lookup"><span data-stu-id="06f1b-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you get an option to assign licenses to them now.</span></span> <span data-ttu-id="06f1b-127">Jatka eteenpäin ja lisää käyttäjille myös käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="06f1b-127">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="06f1b-128">Kun olet lisännyt käyttäjät, saat myös mahdollisuuden jakaa tunniste tiedot lisättyjen uusien käyttäjien kanssa.</span><span class="sxs-lookup"><span data-stu-id="06f1b-128">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="06f1b-129">Voit tulostaa ne, lähettää ne sähköpostitse tai ladata ne palvelimesta.</span><span class="sxs-lookup"><span data-stu-id="06f1b-129">You can choose to print them out, email them, or download them.</span></span>

3. <span data-ttu-id="06f1b-130">Voit lisätä ryhmiä organisaatioosi ja lisätä niihin käyttäjiä.</span><span class="sxs-lookup"><span data-stu-id="06f1b-130">On the Create Teams for your organization, you can choose to add Teams and add users to them.</span></span> <span data-ttu-id="06f1b-131">Voit tehdä tämän myös myöhemmin.</span><span class="sxs-lookup"><span data-stu-id="06f1b-131">You can also do this later.</span></span> <span data-ttu-id="06f1b-132">Lisä tietoja on kohdassa [yrityksen laajuisen tiimin luominen](https://support.office.com/article/037bb27a-bcc9-48fe-8d72-44d9482420a3).</span><span class="sxs-lookup"><span data-stu-id="06f1b-132">For more information, see [create a company-wide Team](https://support.office.com/article/037bb27a-bcc9-48fe-8d72-44d9482420a3).</span></span>

4. <span data-ttu-id="06f1b-133">Ohita sähköpostiviestien siirtäminen valitsemalla **Siirrä sähköpostiviestejä** -sivulla **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="06f1b-133">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="06f1b-134">Jos siirryt toisesta Sähkö posti palvelusta ja haluat kopioida tietosi myöhemmin, voit [siirtää sähkö postin ja yhteys tiedot Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e)-palveluun.</span><span class="sxs-lookup"><span data-stu-id="06f1b-134">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="06f1b-135">Toimialueen yhdistäminen</span><span class="sxs-lookup"><span data-stu-id="06f1b-135">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="06f1b-136">Jos valitsit. onmicrosoft-toimi alueen tai käytät Azure AD Connectia käyttäjien määrittämisestä, et näe tätä vaihetta.</span><span class="sxs-lookup"><span data-stu-id="06f1b-136">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="06f1b-137">Kun haluat määrittää palvelut, sinun on päivitettävä joitakin DNS-isännän tai toimialuerekisteröijän tietueita.</span><span class="sxs-lookup"><span data-stu-id="06f1b-137">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="06f1b-138">Ohjattu määritystoiminto yleensä tunnistaa toimialuerekisteröijän ja antaa linkin vaiheittaisiin ohjeisiin, joiden avulla voit päivittää nimipalvelintietueet toimialuerekisteröijän sivustossa.</span><span class="sxs-lookup"><span data-stu-id="06f1b-138">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="06f1b-139">Jos näin ei ole, [Vaihda nimi palvelimet, jotta voit määrittää Office 365-palvelimen minkä tahansa toimi alueen rekisterin pitäjän kanssa](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="06f1b-139">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="06f1b-140">Jos sinulla on aiemmin luotuja DNS-tietueita, esimerkiksi olemassa oleva Web-sivusto, mutta DNS-isäntä on otettu käyttöön [toimi alueen yhdistämä](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), valitse **Lisää tietueita minulle**.</span><span class="sxs-lookup"><span data-stu-id="06f1b-140">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="06f1b-141">Hyväksy **Valitse online-palvelut** -sivulla kaikki oletus arvot, valitse **Seuraava** **ja valitse sitten Hyväksy DNS** -isännän sivulla.</span><span class="sxs-lookup"><span data-stu-id="06f1b-141">On the **Choose your online services** page, accept all the defaults, and choose **Next**,and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="06f1b-142">Jos sinulla on aiemmin luotuja DNS-tietueita muiden DNS-Isän tien kanssa (ei käytössä toimi alueen yhteydessä), haluat hallita omia DNS-tietueita ja varmistaa, että olemassa olevat palvelut ovat yhteydessä toisiinsa.</span><span class="sxs-lookup"><span data-stu-id="06f1b-142">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="06f1b-143">Lisä tietoja on kohdassa [toimi alueen perusteet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .</span><span class="sxs-lookup"><span data-stu-id="06f1b-143">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Yhdistä verkko tunnuksesi sivu, jolla hallitsen omia DNS-tietueita.](media/connectyourdomainpage.png)

2. <span data-ttu-id="06f1b-145">Noudata ohjatun toiminnon ohjeita, ja Sähkö posti ja muut palvelut määritetään puolestasi.</span><span class="sxs-lookup"><span data-stu-id="06f1b-145">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-data-and-devices"></a><span data-ttu-id="06f1b-146">Suojaa tiedot ja laitteet</span><span class="sxs-lookup"><span data-stu-id="06f1b-146">Protect data and devices</span></span> 

<span data-ttu-id="06f1b-147">Ohjatussa toiminnossa käyttöön luomat käytännöt kohdistetaan automaattisesti [Suojaus ryhmään](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) nimeltä *Kaikki käyttäjät*.</span><span class="sxs-lookup"><span data-stu-id="06f1b-147">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="06f1b-148">Voit myös luoda lisä ryhmiä määrittämään käytäntöjä hallinta keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="06f1b-148">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="06f1b-149">**Suojaa työtiedostojasi mobiililaitteilla** -vaihto ehto **suojaa työtiedostot, kun laitteet katoavat tai varastetaan** , valitaan oletusarvoisesti.</span><span class="sxs-lookup"><span data-stu-id="06f1b-149">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="06f1b-150">Sinulla on mahdollisuus ottaa käyttöön Hallitse, **miten käyttäjät voivat käyttää Office-tiedostoja mobiililaitteissa**, ja tätä suositellaan.</span><span class="sxs-lookup"><span data-stu-id="06f1b-150">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Kuva kaappaus suojaa työtiedostot mobiililaitteiden sivulla.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="06f1b-152">Laajenna **suojaa työtiedostot, kun laitteet katoavat tai varastetaan** näyttämään [oletus arvot](protect-work-files-on-lost-or-stolen-device.md):</span><span class="sxs-lookup"><span data-stu-id="06f1b-152">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![Kuva kaappaus oletus arvoista tiedostojen suojaamiseksi kadonneita laitteita.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="06f1b-154">Valitse **Hallitse, miten käyttäjät voivat käyttää Office-tiedostoja mobiililaitteissa** ja laajentaa sitä näyttämään [oletus arvot](manage-user-access-on-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="06f1b-154">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="06f1b-155">Microsoft suosittelee, että hyväksyt oletus arvot asennuksen aikana, jotta voit luoda sovellus käytäntöjä Androidille, iOS:lle ja Windows 10: lle, jotka koskevat kaikkia käyttäjiä.</span><span class="sxs-lookup"><span data-stu-id="06f1b-155">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="06f1b-156">Voit luoda lisää käytäntöjä asennuksen päätyttyä.</span><span class="sxs-lookup"><span data-stu-id="06f1b-156">You can create more policies after setup completes.</span></span>

        ![Kuva kaappaus Office-tiedostojen suojaus asetuksista mobiililaitteilla.](media/useraccessonmobile.png)

2. <span data-ttu-id="06f1b-158">Tieto suojaa koskevien tietojen ja laitteiden viimeisessä vaiheessa voit määrittää käytäntöjä Windows 10-laitteiden suojaamiseksi.</span><span class="sxs-lookup"><span data-stu-id="06f1b-158">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="06f1b-159">Näitä asetuksia käytetään automaattisesti, kun käyttäjän Windows 10 muodostaa yhteyden organisaatioosi.</span><span class="sxs-lookup"><span data-stu-id="06f1b-159">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="06f1b-160">Voit tarkastella ja muokata [oletus arvoja](secure-windows-10-devices.md)laajentamalla **suojatut Windows 10-laitteet** .</span><span class="sxs-lookup"><span data-stu-id="06f1b-160">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="06f1b-161">Voit myös halutessasi [asentaa Officen automaattisesti](install-office-on-windows-10-during-setup.md) Windows 10-laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="06f1b-161">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Kuva kaappaus asetettu Windows 10 laitteen kokoonpano sivu.](media/setwin10config.png)


## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="06f1b-163">Office 365-asiakas sovellusten käyttöönotto</span><span class="sxs-lookup"><span data-stu-id="06f1b-163">Deploy Office 365 client apps</span></span>

<span data-ttu-id="06f1b-164">Jos valitsit, että Office-sovellukset asennetaan automaattisesti asennuksen aikana, sovellukset asennetaan Windows 10-laitteisiin sen jälkeen, kun käyttäjät ovat kirjauduneet Azure ADIIN Windows-laitteistaan työn tunniste tiedoilla.</span><span class="sxs-lookup"><span data-stu-id="06f1b-164">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="06f1b-165">Jos haluat asentaa Officen mobiililaitteisiin iOS-tai Android-laitteisiin, katso [Microsoft 365-yritys käyttäjien mobiililaitteiden määrittäminen](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="06f1b-165">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="06f1b-166">Voit myös asentaa Officen yksitellen.</span><span class="sxs-lookup"><span data-stu-id="06f1b-166">You can also install Office individually.</span></span> <span data-ttu-id="06f1b-167">Katso ohjeet [Officen asentamisesta PC:hen tai Maciin](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .</span><span class="sxs-lookup"><span data-stu-id="06f1b-167">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>
