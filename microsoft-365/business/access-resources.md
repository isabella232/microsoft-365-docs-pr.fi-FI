---
title: Paikallisten resurssien käyttäminen Azure AD:hen liitetystä laitteesta Microsoft 365 Businessissa
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Lue, miten voit käyttää paikallisia resursseja, kuten liiketoimintasovelluksia, jaettuja tiedostoresursseja ja tulostimia Azure Active Directorysta, joka on liitetty Windows 10 -laitteeseen.
ms.openlocfilehash: 980efbf09349cc0203ac50ae5e028c008d5694ca
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165897"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="13e24-103">Paikallisten resurssien käyttäminen Azure AD:hen liitetystä laitteesta Microsoft 365 Business Premiumissa</span><span class="sxs-lookup"><span data-stu-id="13e24-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="13e24-104">Kaikilla Windows 10 -laitteilla, joihin on liitetty Azure Active Directory, on pääsy kaikkiin pilvipohjaisiin resursseihin, kuten Microsoft 365 -sovelluksiin, ja ne voidaan suojata Microsoft 365 Business Premiumilla.</span><span class="sxs-lookup"><span data-stu-id="13e24-104">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="13e24-105">Voit myös sallia paikallisten resurssien, kuten LOB (Line of Business) -sovellusten, jaettujen tiedostojen ja tulostimien, käytön.</span><span class="sxs-lookup"><span data-stu-id="13e24-105">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="13e24-106">Jos haluat sallia käytön, synkronoi paikallinen Active Directory Azure Active Directoryazure Active Directoryn kanssa [Azure AD Connectin](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) avulla.</span><span class="sxs-lookup"><span data-stu-id="13e24-106">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="13e24-107">Lisätietoja on [ohjeaiheessa Johdanto laitehallintaan Azure Active Directoryssa](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="13e24-107">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="13e24-108">Vaiheet on myös tiivistetty seuraaviin osiin.</span><span class="sxs-lookup"><span data-stu-id="13e24-108">The steps are also summarized in the following sections.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="13e24-109">Tämä menettely koskee vain OAuth- ja NTLM-lukuja.</span><span class="sxs-lookup"><span data-stu-id="13e24-109">This procedure is only applicable to OAuth and NTLM.</span></span> <span data-ttu-id="13e24-110">Kerberos ei ole tuettu.</span><span class="sxs-lookup"><span data-stu-id="13e24-110">Kerberos is not supported.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="13e24-111">Azure AD Connectin suorittaminen</span><span class="sxs-lookup"><span data-stu-id="13e24-111">Run Azure AD Connect</span></span>

<span data-ttu-id="13e24-112">Noudata seuraavia ohjeita, jotta organisaation Azure AD -liitetyt laitteet voivat käyttää paikallisia resursseja.</span><span class="sxs-lookup"><span data-stu-id="13e24-112">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="13e24-113">Jos haluat synkronoida käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directoryyn, suorita ohjattu hakemistosynkronointitoiminto ja Azure AD Connect kohdassa [Hakemistosynkronoinnin määrittäminen Office 365:tä varten](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)kuvatulla tavalla.</span><span class="sxs-lookup"><span data-stu-id="13e24-113">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization).</span></span>
    
2. <span data-ttu-id="13e24-114">Kun hakemistosynkronointi on valmis, varmista, että organisaation Windows 10 -laitteet on liitetty Azure AD:hen.</span><span class="sxs-lookup"><span data-stu-id="13e24-114">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="13e24-115">Tämä vaihe tehdään erikseen jokaisessa Windows 10 -laitteessa.</span><span class="sxs-lookup"><span data-stu-id="13e24-115">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="13e24-116">Lisätietoja on ohjeaiheessa [Windows-laitteiden määrittäminen Microsoft 365 Business Premium -käyttäjille.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="13e24-116">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="13e24-117">Kun Windows 10 -laitteet on liitetty Azure AD:hen, jokaisen käyttäjän on käynnistettävä laitteensa uudelleen ja kirjauduttava sisään Microsoft 365 Business Premium -tunnistetiedoillaan.</span><span class="sxs-lookup"><span data-stu-id="13e24-117">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="13e24-118">Kaikilla laitteilla on nyt myös käytettävissään paikallisia resursseja.</span><span class="sxs-lookup"><span data-stu-id="13e24-118">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="13e24-119">Azure AD:n liitettyjen laitteiden paikallisten resurssien käyttäminen ei edellytä lisätoimia.</span><span class="sxs-lookup"><span data-stu-id="13e24-119">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="13e24-120">Tämä toiminto sisältyy Windows 10:hen.</span><span class="sxs-lookup"><span data-stu-id="13e24-120">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="13e24-121">Jos aiot kirjautua AADJ-laitteeseen muulla kuin salasanamenetelmällä Kuten PIN/Bio-metric WHFB-tunnistetietojen kirjautumisen kautta ja käyttää sitten paikallisia resursseja (osakkeita, tulostimia.. jne.), seuraahttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="13e24-121">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="13e24-122">Jos organisaatiosi ei ole valmis ottamaan käyttöön edellä kuvatussa Azure AD:n liitetyssä laitemäärityksessä, harkitse [Hybrid Azure AD Joined -laitekokoonpanon](manage-windows-devices.md)määrittämistä.</span><span class="sxs-lookup"><span data-stu-id="13e24-122">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="13e24-123">Huomioitavaa, kun liityt Windows-laitteisiin Azure AD:hen</span><span class="sxs-lookup"><span data-stu-id="13e24-123">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="13e24-124">Jos Azure-AD:hen liitetty Windows-laite oli aiemmin liittynyt toimialueeseen tai työryhmään, ota huomioon seuraavat rajoitukset:</span><span class="sxs-lookup"><span data-stu-id="13e24-124">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="13e24-125">Kun laite Azure AD liittyy, se luo uuden käyttäjän viittaamatta aiemmin luotuun profiiliin.</span><span class="sxs-lookup"><span data-stu-id="13e24-125">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="13e24-126">Profiilit on siirrettävä manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="13e24-126">Profiles must be manually migrated.</span></span> <span data-ttu-id="13e24-127">Käyttäjäprofiili sisältää tietoja, kuten suosikkeja, paikallisia tiedostoja, selaimen asetuksia ja Käynnistä-valikon asetuksia.</span><span class="sxs-lookup"><span data-stu-id="13e24-127">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="13e24-128">Paras tapa on löytää kolmannen osapuolen työkalu, jolla voit yhdistää olemassa olevat tiedostot ja asetukset uuteen profiiliin.</span><span class="sxs-lookup"><span data-stu-id="13e24-128">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="13e24-129">Jos laite käyttää ryhmäkäytäntöobjekteja, joillakin ryhmäkäytäntöobjekteilla ei ehkä ole vastaavaa [määrityspalvelun tarjoajaa](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) Intuessa.</span><span class="sxs-lookup"><span data-stu-id="13e24-129">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="13e24-130">Suorita [MMAT-työkalu](https://www.microsoft.com/download/details.aspx?id=45520) löytääksesi vertailukelpoisia csps-organisaatioita olemassa oleville ryhmäkäytäntöobjekteille.</span><span class="sxs-lookup"><span data-stu-id="13e24-130">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="13e24-131">Käyttäjät eivät voi todentaa active directory -todennuksesta riippuvaisiin sovelluksiin.</span><span class="sxs-lookup"><span data-stu-id="13e24-131">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="13e24-132">Arvioi vanha sovellus ja harkitse päivittämistä sovellukseen, joka käyttää nykyaikaista auth-toimintoa, jos mahdollista.</span><span class="sxs-lookup"><span data-stu-id="13e24-132">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="13e24-133">Active Directory -tulostimen etsintä ei toimi.</span><span class="sxs-lookup"><span data-stu-id="13e24-133">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="13e24-134">Voit määrittää suoria tulostinpolkuja kaikille käyttäjille tai käyttää [Hybrid Cloud Print -palvelua.](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)</span><span class="sxs-lookup"><span data-stu-id="13e24-134">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
