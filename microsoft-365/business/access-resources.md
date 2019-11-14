---
title: Paikallisten resurssien käyttö Azure AD-liitetystä laitteesta Microsoft 365 Business
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
description: Opi, miten voit käyttää paikallisia resursseja, kuten yritys sovelluksia, tiedosto resursseja ja tulostimia Azure Active Directorysta, liittyi Windows 10-laitteeseen.
ms.openlocfilehash: fdc1eca6913ba6af4f6b65691fdee2165e7c827e
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/14/2019
ms.locfileid: "38323391"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="256e8-103">Paikallisten resurssien käyttö Azure AD-liitetystä laitteesta Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="256e8-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="256e8-104">Kaikissa Windows 10-laitteilla, joihin on liitetty Azure Active Directory, on pääsy kaikkiin pilvipohjaisiin resursseihin, kuten Office 365-sovelluksiin, ja ne voidaan suojata Microsoft 365 Businessin avulla.</span><span class="sxs-lookup"><span data-stu-id="256e8-104">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Office 365 apps, and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="256e8-105">Voit myös sallia paikallisten resurssien, kuten Business Line (LOB)-sovellusten, jaettujen tiedostojen ja tulostimien, käytön.</span><span class="sxs-lookup"><span data-stu-id="256e8-105">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="256e8-106">Jos haluat sallia Accessin, synkronoi paikallinen Active Directory Azure Active Directoryn kanssa [Azure AD Connectin](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) avulla.</span><span class="sxs-lookup"><span data-stu-id="256e8-106">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="256e8-107">Lisä tietoja on kohdassa [laitteen hallinnan esittely Azure Active Directoryssa](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="256e8-107">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="256e8-108">Vaiheet on myös tiivistetty seuraavissa osissa.</span><span class="sxs-lookup"><span data-stu-id="256e8-108">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="256e8-109">Suorita Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="256e8-109">Run Azure AD Connect</span></span>

<span data-ttu-id="256e8-110">Suorita seuraavat vaiheet, jotta organisaatiosi Azure AD-liitetyt laitteet voivat käyttää paikallisia resursseja.</span><span class="sxs-lookup"><span data-stu-id="256e8-110">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="256e8-111">Jos haluat synkronoida käyttäjät, ryhmät ja yhteys tiedot paikallisesta Active Directorysta Azure Active Directoryyn, suorita ohjattu hakemiston synkronointi ja Azure AD Connect kohdassa [Office 365 Directory-synkronoinnin määrittäminen](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)kuvatulla tavalla.</span><span class="sxs-lookup"><span data-stu-id="256e8-111">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="256e8-112">Kun hakemiston synkronointi on valmis, varmista, että organisaatiosi Windows 10-laitteet on liitetty Azure AD-palveluun.</span><span class="sxs-lookup"><span data-stu-id="256e8-112">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="256e8-113">Tämä vaihe tehdään erikseen kussakin Windows 10-laitteessa.</span><span class="sxs-lookup"><span data-stu-id="256e8-113">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="256e8-114">Lisä tietoja on kohdassa [Windows-laitteiden määrittäminen Microsoft 365-yritys käyttäjille](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="256e8-114">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="256e8-115">Kun Windows 10-laitteet ovat liittyneet Azure AD, jokaisen käyttäjän on käynnistettävä laitteensa uudelleen ja kirjauduttava sisään Microsoft 365-yrityksen tunniste tiedoilla.</span><span class="sxs-lookup"><span data-stu-id="256e8-115">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="256e8-116">Kaikki laitteet voivat nyt käyttää myös paikallisia resursseja.</span><span class="sxs-lookup"><span data-stu-id="256e8-116">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="256e8-117">Azure AD-liitettyjen laitteiden paikallisten resurssien käyttö oikeuksia ei tarvita lisä toimia.</span><span class="sxs-lookup"><span data-stu-id="256e8-117">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="256e8-118">Tämä toiminnallisuus on rakennettu Windows 10.</span><span class="sxs-lookup"><span data-stu-id="256e8-118">This functionality is built into Windows 10.</span></span> 
  
<span data-ttu-id="256e8-119">Jos organisaatiosi ei ole valmis ottamaan käyttöön yllä kuvattua Azure AD-laitteen kokoonpanoa, harkitse [hybridi Azure AD-laitteen kokoonpanon](manage-windows-devices.md)määrittämistä.</span><span class="sxs-lookup"><span data-stu-id="256e8-119">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="256e8-120">Huomioitavaa, kun liityt Windows-laitteisiin Azure ADIIN</span><span class="sxs-lookup"><span data-stu-id="256e8-120">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="256e8-121">Jos Azure-AD-liittyneen Windows-laite on aiemmin liittynyt toimi alueeseen tai työryhmään, harkitse seuraavia rajoituksia:</span><span class="sxs-lookup"><span data-stu-id="256e8-121">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="256e8-122">Kun laite Azure AD liittyy, se luo uuden käyttäjän viittaamatta olemassa olevaan profiiliin.</span><span class="sxs-lookup"><span data-stu-id="256e8-122">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="256e8-123">Profiilit on siirrettävä manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="256e8-123">Profiles must be manually migrated.</span></span> <span data-ttu-id="256e8-124">Käyttäjä profiili sisältää tietoja, kuten Suosikit, paikalliset tiedostot, selaimen asetukset ja Käynnistä-valikon asetukset.</span><span class="sxs-lookup"><span data-stu-id="256e8-124">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="256e8-125">Paras tapa on löytää kolmannen osapuolen työkalu, jolla voit yhdistää olemassa olevat tiedostot ja asetukset uuteen profiiliin.</span><span class="sxs-lookup"><span data-stu-id="256e8-125">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="256e8-126">Jos laite käyttää ryhmä käytäntö objekteja, joissakin GPOs-sovelluksessa ei ehkä ole vastaavaa [määritys palvelun toimittajaa](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) Intune-kohteessa.</span><span class="sxs-lookup"><span data-stu-id="256e8-126">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="256e8-127">Suorita [mmat-työkalu](https://www.microsoft.com/download/details.aspx?id=45520) löytääksesi vertailukelpoisia csps-virheitä olemassa oleville ryhmä käytäntö objekteja varten.</span><span class="sxs-lookup"><span data-stu-id="256e8-127">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="256e8-128">Käyttäjät eivät voi todentaa Active Directory-todennuksesta riippuvaisia sovelluksia.</span><span class="sxs-lookup"><span data-stu-id="256e8-128">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="256e8-129">Arvioi vanha sovellus ja harkitse päivittämistä sovellukseen, joka käyttää modernia auth-sovellusta, jos mahdollista.</span><span class="sxs-lookup"><span data-stu-id="256e8-129">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="256e8-130">Active Directory-tulostimien etsiminen ei toimi.</span><span class="sxs-lookup"><span data-stu-id="256e8-130">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="256e8-131">Voit tarjota suoria tulostin polkuja kaikille käyttäjille tai käyttää [Hybrid Cloud Print-palvelun](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)käyttöä.</span><span class="sxs-lookup"><span data-stu-id="256e8-131">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
