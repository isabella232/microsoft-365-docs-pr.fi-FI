---
title: Microsoft 365 for Businessin hallitseman toimialueeseen liitettyjen Windows 10 -laitteiden hallinnan ottaminen käyttöön
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
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Lue, miten voit antaa Microsoft 365:n suojata paikallisia Active-Directoryyn liitettyjä Windows 10 -laitteita muutamassa vaiheessa.
ms.openlocfilehash: adc125c32fe5aa56be8c17c07f28316602a36594
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165805"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-for-business"></a><span data-ttu-id="9caa2-103">Microsoft 365 for Businessin hallitseman toimialueeseen liitettyjen Windows 10 -laitteiden hallinnan ottaminen käyttöön</span><span class="sxs-lookup"><span data-stu-id="9caa2-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 for business</span></span>

<span data-ttu-id="9caa2-104">Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 for Businessin suojaamaan Windows 10 -laitteita ja säilyttämään silti paikallisen todennuksen edellyttävien paikallisten resurssien käytön.</span><span class="sxs-lookup"><span data-stu-id="9caa2-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 for business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="9caa2-105">Voit määrittää tämän suojauksen käyttöön **hybridiazure AD-liitetyillä laitteilla.**</span><span class="sxs-lookup"><span data-stu-id="9caa2-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="9caa2-106">Nämä laitteet on liitetty sekä paikalliseen Active Directoryyn että Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="9caa2-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="9caa2-107">Tässä videossa kuvataan, miten tämä määritetään yleisimpää skenaariota varten, joka on kuvattu myös seuraavissa vaiheissa.</span><span class="sxs-lookup"><span data-stu-id="9caa2-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="9caa2-108">1. Valmistele hakemistosynkronointiin</span><span class="sxs-lookup"><span data-stu-id="9caa2-108">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="9caa2-109">Ennen kuin synkronoit käyttäjät ja tietokoneet paikallisesta Active Directory -toimialueesta, tutustu artikkeliin [Hakemistosynkronoinnin valmisteleminen Office 365:een](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="9caa2-109">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="9caa2-110">Erityisesti:</span><span class="sxs-lookup"><span data-stu-id="9caa2-110">In particular:</span></span>

   - <span data-ttu-id="9caa2-111">Varmista, että hakemistossa ei ole kaksoiskappaleita seuraaville määritteille: **mail**, **proxyAddresses**ja **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="9caa2-111">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="9caa2-112">Näiden arvojen on oltava yksilöllisiä, ja kaksoiskappaleet on poistettava.</span><span class="sxs-lookup"><span data-stu-id="9caa2-112">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="9caa2-113">Suosittelemme, että määrität kullekin paikalliselle käyttäjätilille **upn (userPrincipalName)** -määritteen vastaamaan ensisijaista sähköpostiosoitetta, joka vastaa lisensoitua Microsoft 365 -käyttäjää.</span><span class="sxs-lookup"><span data-stu-id="9caa2-113">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="9caa2-114">Esimerkki: *mary.shelley@contoso.com* mary@contoso *sijaan.local*</span><span class="sxs-lookup"><span data-stu-id="9caa2-114">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="9caa2-115">Jos Active Directory -toimialue päättyy ei-reititettävään jälkiliitteeseen, kuten *.local* tai *.lan*, voit muuttaa internetin reititettävän liitteen, kuten *.com* tai *.org*, sijaan paikallisten käyttäjätilien UPN-liitettä ensin kohdassa [Ei-reititettävän toimialueen valmisteleminen hakemistosynkronointia varten](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="9caa2-115">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="9caa2-116">2. Azure AD Connectin asentaminen ja määrittäminen</span><span class="sxs-lookup"><span data-stu-id="9caa2-116">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="9caa2-117">Jos haluat synkronoida käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directoryyn, asenna Azure Active Directory Connect ja määritä hakemistosynkronointi.</span><span class="sxs-lookup"><span data-stu-id="9caa2-117">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> <span data-ttu-id="9caa2-118">Lisätietoja on [ohjeaiheessa Hakemistosynkronoinnin määrittäminen Office 365:tä varten.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)</span><span class="sxs-lookup"><span data-stu-id="9caa2-118">See [Set up directory synchronization for Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

> [!NOTE]
> <span data-ttu-id="9caa2-119">Vaiheet ovat täsmälleen samat Microsoft 365 for Businessille.</span><span class="sxs-lookup"><span data-stu-id="9caa2-119">The steps are exactly the same for Microsoft 365 for business.</span></span> 

<span data-ttu-id="9caa2-120">Kun määrität Azure AD Connect -asetuksia, suosittelemme, että otat käyttöön **salasanan synkronoinnin,** **saumattoman kertakirjautumisen**ja **salasanan takaisinkirjoitusominaisuuden,** jota tuetaan myös Microsoft 365 for Businessissa.</span><span class="sxs-lookup"><span data-stu-id="9caa2-120">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="9caa2-121">Azure AD Connectin valintaruudun lisäksi salasanan takaisinkirjoitukselle on joitakin lisävaiheita.</span><span class="sxs-lookup"><span data-stu-id="9caa2-121">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="9caa2-122">Lisätietoja on [ohjeaiheessa Toimintaohjeet: salasanan takaisinkirjoituksen määrittäminen](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="9caa2-122">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

## <a name="3-configure-hybrid-azure-ad-join"></a><span data-ttu-id="9caa2-123">3. Määritä Hybrid Azure AD Join</span><span class="sxs-lookup"><span data-stu-id="9caa2-123">3. Configure Hybrid Azure AD Join</span></span>

<span data-ttu-id="9caa2-124">Ennen kuin otat Windows 10 -laitteiden käyttöön Hybrid Azure AD-versioon liittyen, varmista, että täytät seuraavat edellytykset:</span><span class="sxs-lookup"><span data-stu-id="9caa2-124">Before you enable Windows 10 devices to be Hybrid Azure AD joined, make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="9caa2-125">Käytössäsi on Azure AD Connectin uusin versio.</span><span class="sxs-lookup"><span data-stu-id="9caa2-125">You're running the latest version of Azure AD Connect.</span></span>

   - <span data-ttu-id="9caa2-126">Azure AD connect on synkronoinut kaikki sellaisten laitteiden tietokoneobjektit, jotka haluat yhdistää Azure AD:hen.</span><span class="sxs-lookup"><span data-stu-id="9caa2-126">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="9caa2-127">Jos tietokoneobjektit kuuluvat tiettyihin organisaatioyksiköihin, varmista, että nämä organisaatioyksiköt on määritetty synkronoitavia varten myös Azure AD connect -yhteyden yhteydessä.</span><span class="sxs-lookup"><span data-stu-id="9caa2-127">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>

<span data-ttu-id="9caa2-128">Jos haluat rekisteröidä olemassa olevat toimialueeseen liitetyt Windows 10 -laitteet Hybrid Azure AD -palveluksi, noudata [opetusohjelman Azure Active Directory -hybridiliitoksen määrittäminen hallituille toimialueille](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join)ohjeita.</span><span class="sxs-lookup"><span data-stu-id="9caa2-128">To register existing domain-joined Windows 10 devices as Hybrid Azure AD joined, follow the steps in the [Tutorial: Configure hybrid Azure Active Directory join for managed domains](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="9caa2-129">Tämä yhdistelmämahdollistaa nykyisen paikallisen Active Directoryn liitettyjen Windows 10 -tietokoneiden kanssa ja pilvipalvelun valmiiksi.</span><span class="sxs-lookup"><span data-stu-id="9caa2-129">This hybrid-enables your existing on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a><span data-ttu-id="9caa2-130">4. Ota automaattinen rekisteröinti Käyttöön Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="9caa2-130">4. Enable automatic enrollment for Windows 10</span></span>

 <span data-ttu-id="9caa2-131">Jos haluat rekisteröidä Windows 10 -laitteet automaattisesti mobiililaitteiden hallintaa varten Intunen käyttöön, katso Windows [10 -laitteen rekisteröiminen automaattisesti ryhmäkäytännön avulla](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span><span class="sxs-lookup"><span data-stu-id="9caa2-131">To automatically enroll Windows 10 devices for mobile device management in Intune, see [Enroll a Windows 10 device automatically using Group Policy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span></span> <span data-ttu-id="9caa2-132">Voit määrittää ryhmäkäytännön paikalliselle tietokonetasolle tai joukkotoiminnoille käyttämällä ryhmäkäytäntöjen hallintakonsolia ja ADMX-malleja tämän ryhmäkäytäntöasetuksen luomiseen toimialueen ohjauskoneeseen.</span><span class="sxs-lookup"><span data-stu-id="9caa2-132">You can set the Group Policy at a local computer level, or for bulk operations, you can use the Group Policy Management Console and ADMX templates to create this Group Policy setting on your Domain Controller.</span></span>

## <a name="5-configure-seamless-single-sign-on"></a><span data-ttu-id="9caa2-133">5. Määritä saumaton kertakirjautuminen</span><span class="sxs-lookup"><span data-stu-id="9caa2-133">5. Configure Seamless Single Sign-On</span></span>

  <span data-ttu-id="9caa2-134">Saumaton SSO kirjaa käyttäjät automaattisesti Microsoft 365 -pilviresursseihinsa, kun he käyttävät yritystietokoneita.</span><span class="sxs-lookup"><span data-stu-id="9caa2-134">Seamless SSO automatically signs users into their Microsoft 365 cloud resources when they use corporate computers.</span></span> <span data-ttu-id="9caa2-135">Ota käyttöön jompaakumpaa [azure Active Directoryn saumaton tavasta Single Sign-On: Quick start -kohdassa](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature)kuvatuista kahdesta ryhmäkäytäntövaihtoehdosta.</span><span class="sxs-lookup"><span data-stu-id="9caa2-135">Simply deploy one of the two Group Policy options described in [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span></span> <span data-ttu-id="9caa2-136">**Ryhmäkäytäntö-asetus** ei salli käyttäjien muuttaa asetuksiaan, kun taas **Ryhmäkäytäntöasetukset-asetus** määrittää arvot, mutta jättää heidät myös käyttäjän määritettäviksi.</span><span class="sxs-lookup"><span data-stu-id="9caa2-136">The **Group Policy** option doesn't allow users to change their settings, while the **Group Policy Preference** option sets the values but also leaves them user-configurable.</span></span>

## <a name="6-set-up-windows-hello-for-business"></a><span data-ttu-id="9caa2-137">6. Windows Hello for Businessin määrittäminen</span><span class="sxs-lookup"><span data-stu-id="9caa2-137">6. Set up Windows Hello for Business</span></span>

 <span data-ttu-id="9caa2-138">Windows Hello for Business korvaa salasanat vahvalla kaksivaiheisella todennuksella (2FA) paikalliseen tietokoneeseen kirjautumista varten.</span><span class="sxs-lookup"><span data-stu-id="9caa2-138">Windows Hello for Business replaces passwords with strong two-factor authentication (2FA) for signing into a local computer.</span></span> <span data-ttu-id="9caa2-139">Yksi tekijä on epäsymmetrinen avainpari ja toinen PIN-koodi tai muu paikallinen ele, kuten sormenjälki tai kasvojentunnistus, jos laite tukee sitä.</span><span class="sxs-lookup"><span data-stu-id="9caa2-139">One factor is an asymmetric key pair, and the other is a PIN or other local gesture such as fingerprint or facial recognition if your device supports it.</span></span> <span data-ttu-id="9caa2-140">Suosittelemme, että korvaat salasanat 2FA: lla ja Windows Hello for Businessilla, jos mahdollista.</span><span class="sxs-lookup"><span data-stu-id="9caa2-140">We recommend that you replace passwords with 2FA and Windows Hello for Business where possible.</span></span>

<span data-ttu-id="9caa2-141">Voit määrittää Windows Hello for Businessin yhdistelmätoiminnon [tutustuessa hybridiavaimeen, joka luottaa Windows Hello for Business -edellytyksiin](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span><span class="sxs-lookup"><span data-stu-id="9caa2-141">To configure Hybrid Windows Hello for Business, review the [Hybrid Key trust Windows Hello for Business Prerequisites](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span></span> <span data-ttu-id="9caa2-142">Noudata sitten ohjeaiheen [Systematistisen Windows Hello for Business -näppäinluottamusasetusten määrittäminen](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings)ohjeita.</span><span class="sxs-lookup"><span data-stu-id="9caa2-142">Then follow the instructions in [Configure Hybrid Windows Hello for Business key trust settings](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings).</span></span> 
