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
ms.openlocfilehash: 92e8ccb99dfece7687c25db84b81fc7bc7158d71
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/17/2019
ms.locfileid: "37574674"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="7782f-103">Paikallisten resurssien käyttö Azure AD-liitetystä laitteesta Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="7782f-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="7782f-104">Kaikissa Windows 10-laitteilla, joihin on liitetty Azure Active Directory, on pääsy kaikkiin pilvipohjaisiin resursseihin, kuten Office 365-sovelluksiin, ja ne voidaan suojata Microsoft 365 Businessin avulla.</span><span class="sxs-lookup"><span data-stu-id="7782f-104">Any Windows 10 device that is Azure Active Directory joined will have access to all cloud-based resources such as your Office 365 apps and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="7782f-105">Jos haluat sallia myös paikallisten resurssien, kuten Business Line (LOB)-sovellusten, jaettujen tiedostojen ja tulostimien käytön, synkronoi paikallinen Active Directory Azure Active Directoryn kanssa [Azure AD Connectin](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect)avulla.</span><span class="sxs-lookup"><span data-stu-id="7782f-105">To also allow access to on-premises resources like Line Of Business (LOB) apps, file shares, and printers, you must synchronize your on-premises Active Directory with Azure Active Directory by using [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect).</span></span> 

<span data-ttu-id="7782f-106">Lisä tietoja on kohdassa [laitteen hallinnan esittely Azure Active Directoryssa](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) .</span><span class="sxs-lookup"><span data-stu-id="7782f-106">See [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) to learn more.</span></span>
<span data-ttu-id="7782f-107">Vaiheet on myös tiivistetty seuraavissa osissa.</span><span class="sxs-lookup"><span data-stu-id="7782f-107">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="7782f-108">Suorita Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="7782f-108">Run Azure AD Connect</span></span>

<span data-ttu-id="7782f-109">Suorita seuraavat vaiheet, jotta organisaatiosi Azure AD-liitetyt laitteet voivat käyttää paikallisia resursseja.</span><span class="sxs-lookup"><span data-stu-id="7782f-109">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="7782f-110">Jos haluat synkronoida käyttäjät, ryhmät ja yhteys tiedot paikallisesta Active Directorysta Azure Active Directoryyn, suorita ohjattu hakemiston synkronointi ja Azure AD Connect kuvatulla tavalla kohdassa [Office 365 Directory-synkronointi](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="7782f-110">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="7782f-111">Kun hakemiston synkronointi on suoritettu, varmista, että organisaatiosi Windows 10-laitteet on liitetty Azure AD-palveluun.</span><span class="sxs-lookup"><span data-stu-id="7782f-111">After the directory synchronization has completed, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="7782f-112">Tämä vaihe tehdään erikseen kussakin Windows 10-laitteessa.</span><span class="sxs-lookup"><span data-stu-id="7782f-112">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="7782f-113">Lisä tietoja on kohdassa [Windows-laitteiden määrittäminen Microsoft 365-yritys käyttäjille](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="7782f-113">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="7782f-114">Kun Windows 10-laitteet ovat liittyneet Azure AD, jokaisen käyttäjän tulee käynnistää laitteensa uudelleen ja kirja utua sisään Microsoft 365-yrityksen tunniste tiedoilla.</span><span class="sxs-lookup"><span data-stu-id="7782f-114">Once the Windows 10 devices are Azure AD joined, each user should reboot their devices and login with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="7782f-115">Kaikki laitteet saavat nyt käyttöönsä myös paikallisia resursseja.</span><span class="sxs-lookup"><span data-stu-id="7782f-115">All devices will now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="7782f-116">Azure AD-liitettyjen laitteiden paikallisten resurssien käyttö oikeuksia ei tarvita lisä toimia.</span><span class="sxs-lookup"><span data-stu-id="7782f-116">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="7782f-117">Tämä on Windows 10: ssä käytettävissä oleva sisäänrakennettu toiminto.</span><span class="sxs-lookup"><span data-stu-id="7782f-117">This is built-in functionality available in Windows 10.</span></span> 
  
<span data-ttu-id="7782f-118">Jos organisaatiosi ei ole valmis ottamaan käyttöön yllä kuvattua Azure AD Joined-laitteen kokoonpanoa, harkitse [hybridi Azure AD-laitteen kokoonpanon](manage-windows-devices.md)määrittämistä.</span><span class="sxs-lookup"><span data-stu-id="7782f-118">If your organization is not ready to deploy in the Azure AD Joined Device Configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a><span data-ttu-id="7782f-119">Windows-laitteisiin Azure ADIIN liittyessään liittyvät seikat</span><span class="sxs-lookup"><span data-stu-id="7782f-119">Considerations when joining your Windows devices to Azure AD</span></span>

<span data-ttu-id="7782f-120">Jos olet Azure AD, joka liittyy sellaiseen Windows-laitteeseen, joka on aiemmin ollut toimi alueeseen liitetty tai työryhmässä, sinun on otettava huomioon seuraavat rajoitukset:</span><span class="sxs-lookup"><span data-stu-id="7782f-120">If you are Azure AD joining a Windows device that has previously been domain-joined or in a workgroup, you need to consider the following limitations:</span></span>
  
- <span data-ttu-id="7782f-121">Kun laite Azure AD liittyy, se luo uuden käyttäjän viittaamatta olemassa olevaan profiiliin.</span><span class="sxs-lookup"><span data-stu-id="7782f-121">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="7782f-122">Profiilien korjaaminen edellyttää, että profiilit siirretään manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="7782f-122">To fix this, profiles need to be manually migrated.</span></span> <span data-ttu-id="7782f-123">Käyttäjä profiili sisältää tietoja, kuten Suosikit, paikalliset tiedostot, selaimen asetukset, Käynnistä-valikon asetukset jne. Paras tapa on löytää kolmannen osapuolen työkalu, jolla voit yhdistää olemassa olevat tiedostot ja asetukset uuteen profiiliin</span><span class="sxs-lookup"><span data-stu-id="7782f-123">A user profile contains information like favorites, local files, browser settings, Start menu settings, etc. A best approach is to find a third-party tool to map existing files and settings to the new profile</span></span>

- <span data-ttu-id="7782f-124">Jos laite käyttää ryhmä käytäntö objekteja, joissakin GPOs-sovelluksessa ei ehkä ole vastaavaa [määritys palvelun toimittajaa](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) Intune-kohteessa.</span><span class="sxs-lookup"><span data-stu-id="7782f-124">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="7782f-125">Suorita [mmat-työkalu](https://www.microsoft.com/download/details.aspx?id=45520) löytääksesi vertailukelpoisia csps-virheitä olemassa oleville ryhmä käytäntö objekteja varten.</span><span class="sxs-lookup"><span data-stu-id="7782f-125">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="7782f-126">Käyttäjät eivät voi todentaa Active Directory-todennuksesta riippuvaisia sovelluksia.</span><span class="sxs-lookup"><span data-stu-id="7782f-126">Users will not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="7782f-127">Voit käsitellä tätä arvioida vanhan sovelluksen avulla ja harkita päivittämistä sovellukseen, joka käyttää modernia auth jos mahdollista.</span><span class="sxs-lookup"><span data-stu-id="7782f-127">To deal with this evaluate using a legacy app and consider updating to an app that uses modern Auth if possible.</span></span>

- <span data-ttu-id="7782f-128">Active Directory-tulostimien etsiminen ei toimi.</span><span class="sxs-lookup"><span data-stu-id="7782f-128">Active Directory printer discovery will not work.</span></span> <span data-ttu-id="7782f-129">Voit korjata tämän, tarjota suorat tulostus polut kaikille käyttäjille tai hyödyntää [Hybrid Cloud Print-palvelun](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="7782f-129">To fix this, provide direct printer paths for all users or leverage [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
