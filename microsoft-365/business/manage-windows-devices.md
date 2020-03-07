---
title: Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi
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
description: Lue, miten voit ottaa Microsoft 365:n suojaamaan paikallisia Active-Directory-liitettyjä Windows 10 -laitteita muutamassa vaiheessa.
ms.openlocfilehash: 625eb7ac344b060409101d650ff30044d073f5bf
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561456"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="8d56a-103">Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi</span><span class="sxs-lookup"><span data-stu-id="8d56a-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="8d56a-104">Jos organisaatiosi käyttää paikallista Windows Server In Active Directorya, voit määrittää Microsoft 365 Businessin suojaamaan Windows 10 -laitteita säilyttäen samalla paikallisen todennuksen edellyttävien paikallisten resurssien käytön.</span><span class="sxs-lookup"><span data-stu-id="8d56a-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="8d56a-105">Voit määrittää tämän suojauksen ottaaksesi käyttöön **Hybrid Azure AD :n liitetyt laitteet**.</span><span class="sxs-lookup"><span data-stu-id="8d56a-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="8d56a-106">Nämä laitteet on liitetty sekä paikalliseen Active Directoryyn että Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="8d56a-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="8d56a-107">Tässä videossa kuvataan, miten tämä määritetään yleisimmissä tilanteissa, jotka on kuvattu myös seuraavissa vaiheissa.</span><span class="sxs-lookup"><span data-stu-id="8d56a-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="8d56a-108">1. Valmistaudu hakemistosynkronointiin</span><span class="sxs-lookup"><span data-stu-id="8d56a-108">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="8d56a-109">Ennen kuin synkronoit käyttäjät ja tietokoneet paikallisesta Active Directory -toimialueesta, tutustu [artikkeliin Hakemistosynkronoinnin valmisteleminen Office 365:een](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="8d56a-109">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="8d56a-110">Erityisesti:</span><span class="sxs-lookup"><span data-stu-id="8d56a-110">In particular:</span></span>

   - <span data-ttu-id="8d56a-111">Varmista, että hakemistossa ei ole kaksoiskappaleita seuraaville määritteille: **mail**, **proxyAddresses**ja **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="8d56a-111">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="8d56a-112">Näiden arvojen on oltava yksilöllisiä ja kaksoiskappaleet poistettava.</span><span class="sxs-lookup"><span data-stu-id="8d56a-112">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="8d56a-113">Microsoft suosittelee, että määrität **userPrincipalName** (UPN) -määritteen kullekin paikalliselle käyttäjätilille vastaamaan ensisijaista sähköpostiosoitetta, joka vastaa lisensoitua Microsoft 365 -käyttäjää.</span><span class="sxs-lookup"><span data-stu-id="8d56a-113">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="8d56a-114">Esimerkiksi: *mary.shelley@contoso.com* *mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="8d56a-114">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="8d56a-115">Jos Active Directory -toimialue päättyy ei-reititettävään liitteeseen, kuten *.local* tai *.lan*, \*\* säädä ensin -toimialueen \*\* [valmisteleminen hakemistosynkronointia varten"](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)-kohdassa kuvattuun upn-päätettä .</span><span class="sxs-lookup"><span data-stu-id="8d56a-115">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="8d56a-116">2. Azure AD Connectin asentaminen ja määrittäminen</span><span class="sxs-lookup"><span data-stu-id="8d56a-116">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="8d56a-117">Jos haluat synkronoida käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directoryyn, asenna Azure Active Directory Connect ja määritä hakemistosynkronointi.</span><span class="sxs-lookup"><span data-stu-id="8d56a-117">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> <span data-ttu-id="8d56a-118">Lisätietoja [on ohjeaiheessa Hakemistosynkronoinnin määrittäminen Office 365:tä varten.](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)</span><span class="sxs-lookup"><span data-stu-id="8d56a-118">See [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) to learn more.</span></span>

> [!NOTE]
> <span data-ttu-id="8d56a-119">Vaiheet ovat täsmälleen samat Microsoft 365 Businessissa.</span><span class="sxs-lookup"><span data-stu-id="8d56a-119">The steps are exactly the same for Microsoft 365 Business.</span></span> 

<span data-ttu-id="8d56a-120">Kun määrität Azure AD Connectin asetukset, suosittelemme, että otat **käyttöön salasanan synkronoinnin,** **saumattoman kertakirjautumisen**ja **salasanan palautustoiminnon,** jota tuetaan myös Microsoft 365 Businessissa.</span><span class="sxs-lookup"><span data-stu-id="8d56a-120">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 Business.</span></span>

> [!NOTE]
> <span data-ttu-id="8d56a-121">Azure AD Connectin valintaruudun lisäksi on joitakin lisävaiheita salasanan takaisinkirjoittamiseksi.</span><span class="sxs-lookup"><span data-stu-id="8d56a-121">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="8d56a-122">Lisätietoja on [ohjeaiheessa Toimintaohjeet: salasanan takaisinkirjoituksen määrittäminen](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="8d56a-122">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

## <a name="3-configure-hybrid-azure-ad-join"></a><span data-ttu-id="8d56a-123">3. Määritä Hybridi Azure AD -liity</span><span class="sxs-lookup"><span data-stu-id="8d56a-123">3. Configure Hybrid Azure AD Join</span></span>

<span data-ttu-id="8d56a-124">Ennen kuin otat Windows 10 -laitteiden käyttöön, että Ne liitetään Hybridi Azure AD:hen, varmista, että täytät seuraavat edellytykset:</span><span class="sxs-lookup"><span data-stu-id="8d56a-124">Before you enable Windows 10 devices to be Hybrid Azure AD joined, make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="8d56a-125">Käytössäsi on Azure AD Connectin uusin versio.</span><span class="sxs-lookup"><span data-stu-id="8d56a-125">You're running the latest version of Azure AD Connect.</span></span>

   - <span data-ttu-id="8d56a-126">Azure AD connect on synkronoinut kaikki sellaisten laitteiden tietokoneobjektit, joihin haluat liittyä Azure AD:n yhdistelmäksi.</span><span class="sxs-lookup"><span data-stu-id="8d56a-126">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="8d56a-127">Jos tietokoneobjektit kuuluvat tiettyihin organisaatioyksiköihin, varmista, että nämä oUs:t on määritetty synkronoitavia varten myös Azure AD connectissa.</span><span class="sxs-lookup"><span data-stu-id="8d56a-127">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>

<span data-ttu-id="8d56a-128">Jos haluat rekisteröidä aiemmin luodut toimialueuuteen liitetyt Windows 10 -laitteet Hybrid Azure AD -palveluun liittyneenä, noudata [opetusohjelman ohjeita: Määritä azure Active Directory -yhdistelmäliittymä hallituille toimialueille](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span><span class="sxs-lookup"><span data-stu-id="8d56a-128">To register existing domain-joined Windows 10 devices as Hybrid Azure AD joined, follow the steps in the [Tutorial: Configure hybrid Azure Active Directory join for managed domains](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="8d56a-129">Tämä hybridi mahdollistaa nykyisen paikallisen Active Directoryn windows 10 -tietokoneisiin ja tekee niistä pilvivalmiita.</span><span class="sxs-lookup"><span data-stu-id="8d56a-129">This hybrid-enables your existing on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a><span data-ttu-id="8d56a-130">4. Ota automaattinen rekisteröinti käyttöön Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="8d56a-130">4. Enable automatic enrollment for Windows 10</span></span>

 <span data-ttu-id="8d56a-131">Lisätietoja Windows 10 -laitteiden automaattisesta rekisteröimiseksi mobiililaitteiden hallintaa varten Intuniin on ohjeaiheessa [Windows 10 -laitteen rekisteröiminen automaattisesti ryhmäkäytännön avulla](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span><span class="sxs-lookup"><span data-stu-id="8d56a-131">To automatically enroll Windows 10 devices for mobile device management in Intune, see [Enroll a Windows 10 device automatically using Group Policy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span></span> <span data-ttu-id="8d56a-132">Voit määrittää ryhmäkäytäntökäytännön paikalliselle tietokonetasolle tai joukkotoiminnoille, voit luoda tämän ryhmäkäytäntöasetuksen toimialueen ohjauskoneeseen ryhmäkäytäntöjen hallintakonsolin ja ADMX-mallien avulla.</span><span class="sxs-lookup"><span data-stu-id="8d56a-132">You can set the Group Policy at a local computer level, or for bulk operations, you can use the Group Policy Management Console and ADMX templates to create this Group Policy setting on your Domain Controller.</span></span>

## <a name="5-configure-seamless-single-sign-on"></a><span data-ttu-id="8d56a-133">5. Määritä saumaton kertakirjautuminen</span><span class="sxs-lookup"><span data-stu-id="8d56a-133">5. Configure Seamless Single Sign-On</span></span>

  <span data-ttu-id="8d56a-134">Saumaton sso kirjaa käyttäjät automaattisesti Microsoft 365 -pilviresursseihinsa, kun he käyttävät yritystietokoneita.</span><span class="sxs-lookup"><span data-stu-id="8d56a-134">Seamless SSO automatically signs users into their Microsoft 365 cloud resources when they use corporate computers.</span></span> <span data-ttu-id="8d56a-135">Ota käyttöön toinen [Azure Active Directoryseamless Single Sign-On: Quick start -kohdassa](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature)kuvatuista ryhmäkäytäntövaihtoehdoista.</span><span class="sxs-lookup"><span data-stu-id="8d56a-135">Simply deploy one of the two Group Policy options described in [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span></span> <span data-ttu-id="8d56a-136">**Ryhmäkäytäntö-asetus** ei salli käyttäjien muuttaa asetuksiaan, kun taas **Ryhmäkäytäntöasetukset-asetus** määrittää arvot, mutta jättää ne myös käyttäjän määritettäviksi.</span><span class="sxs-lookup"><span data-stu-id="8d56a-136">The **Group Policy** option doesn't allow users to change their settings, while the **Group Policy Preference** option sets the values but also leaves them user-configurable.</span></span>

## <a name="6-set-up-windows-hello-for-business"></a><span data-ttu-id="8d56a-137">6. Windows Hello for Businessin määrittäminen</span><span class="sxs-lookup"><span data-stu-id="8d56a-137">6. Set up Windows Hello for Business</span></span>

 <span data-ttu-id="8d56a-138">Windows Hello for Business korvaa salasanat vahvalla kaksiosaisella todennuksella (2FA), joka liittyy paikalliseen tietokoneeseen kirjautumiseen.</span><span class="sxs-lookup"><span data-stu-id="8d56a-138">Windows Hello for Business replaces passwords with strong two-factor authentication (2FA) for signing into a local computer.</span></span> <span data-ttu-id="8d56a-139">Yksi tekijä on epäsymmetrinen avainpari ja toinen PIN-koodi tai muu paikallinen ele, kuten sormenjälki tai kasvojentunnistus, jos laitteesi tukee sitä.</span><span class="sxs-lookup"><span data-stu-id="8d56a-139">One factor is an asymmetric key pair, and the other is a PIN or other local gesture such as fingerprint or facial recognition if your device supports it.</span></span> <span data-ttu-id="8d56a-140">Suosittelemme, että korvaat salasanat 2FA:lla ja Windows Hello for Businessilla mahdollisuuksien mukaan.</span><span class="sxs-lookup"><span data-stu-id="8d56a-140">We recommend that you replace passwords with 2FA and Windows Hello for Business where possible.</span></span>

<span data-ttu-id="8d56a-141">Jos haluat määrittää Hybridi-Windows Hello for Businessin asetukset, tutustu [Hybridiavaimen luottamus Windows Hello for Business -edellytyksiin](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span><span class="sxs-lookup"><span data-stu-id="8d56a-141">To configure Hybrid Windows Hello for Business, review the [Hybrid Key trust Windows Hello for Business Prerequisites](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span></span> <span data-ttu-id="8d56a-142">Noudata sitten kohdassa [Windows Hello for Business -avainluottamusasetusten määrittäminen](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings)ohjeita.</span><span class="sxs-lookup"><span data-stu-id="8d56a-142">Then follow the instructions in [Configure Hybrid Windows Hello for Business key trust settings](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings).</span></span> 
