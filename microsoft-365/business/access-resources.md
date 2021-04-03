---
title: Paikallisen resurssien käyttö Azure AD:stä yhdistetystä laitteesta Microsoft 365 Businessissa
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Lue, miten voit käyttää paikallisia resursseja, kuten yrityssovellusten riviä, jaetut tiedostot ja tulostimet Azure Active Directoryyn yhdistetystä Windows 10 -laitteesta.
ms.openlocfilehash: 27549d6c3b03413f2f05c69845caad155333ca97
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580310"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="9a2af-103">Käytä paikallisia resursseja Azure AD:llä yhdistetystä laitteesta Microsoft 365 Business Premiumissa</span><span class="sxs-lookup"><span data-stu-id="9a2af-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="9a2af-104">Tämä artikkeli koskee Microsoft 365 Business Premiumia.</span><span class="sxs-lookup"><span data-stu-id="9a2af-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="9a2af-105">Kaikki Azure Active Directoryyn yhdistetyt Windows 10 -laitteet voivat käyttää kaikkia pilvipohjaisia resursseja, kuten Microsoft 365 -sovelluksia, ja ne voidaan suojata Microsoft 365 Business Premiumilla.</span><span class="sxs-lookup"><span data-stu-id="9a2af-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="9a2af-106">Voit myös sallia pääsyn paikallisiin resursseihin, kuten liiketoiminta-sovelluksiin, jaekkeisiin ja tulostimien.</span><span class="sxs-lookup"><span data-stu-id="9a2af-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="9a2af-107">Jos haluat sallia käytön, synkronoi paikallinen Active Directory Azure Active Directoryn kanssa Azure [AD Connectin](/azure/active-directory/connect/active-directory-aadconnect) avulla.</span><span class="sxs-lookup"><span data-stu-id="9a2af-107">To allow access, use [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="9a2af-108">Lisätietoja on ohjeaiheessa Johdanto Azure [Active Directoryn laitehallintaan.](/azure/active-directory/device-management-introduction)</span><span class="sxs-lookup"><span data-stu-id="9a2af-108">To learn more, see [Introduction to device management in Azure Active Directory](/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="9a2af-109">Vaiheiden yhteenveto on myös seuraavissa osissa.</span><span class="sxs-lookup"><span data-stu-id="9a2af-109">The steps are also summarized in the following sections.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="9a2af-110">Azure AD Connectin käyttö</span><span class="sxs-lookup"><span data-stu-id="9a2af-110">Run Azure AD Connect</span></span>

<span data-ttu-id="9a2af-111">Suorita seuraavat vaiheet, jotta organisaatiosi Azure AD:ssä olevat laitteet voivat käyttää paikallisia resursseja.</span><span class="sxs-lookup"><span data-stu-id="9a2af-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="9a2af-112">Jos haluat synkronoida käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directoryyn, suorita ohjattu hakemistosynkronointitoiminto ja Azure AD Connect artikkelissa Hakemistosynkronoinnin määrittäminen [Office 365:lle kuvatulla tavalla.](../enterprise/set-up-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="9a2af-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](../enterprise/set-up-directory-synchronization.md).</span></span>
    
2. <span data-ttu-id="9a2af-113">Kun hakemistosynkronointi on valmis, varmista, että organisaatiosi Windows 10 -laitteet on liitetty Azure AD:n kanssa.</span><span class="sxs-lookup"><span data-stu-id="9a2af-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="9a2af-114">Tämä vaihe tehdään yksitellen kussakin Windows 10 -laitteessa.</span><span class="sxs-lookup"><span data-stu-id="9a2af-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="9a2af-115">Lisätietoja [on kohdassa Windows-laitteiden määritäminen Microsoft 365 Business Premium](set-up-windows-devices.md) -käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="9a2af-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="9a2af-116">Kun Windows 10 -laitteet on liitetty Azure AD:ssä, kunkin käyttäjän on käynnistettävä laitteensa uudelleen ja kirjauduttava sisään Microsoft 365 Business Premium -tunnistetiedoillaan.</span><span class="sxs-lookup"><span data-stu-id="9a2af-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="9a2af-117">Kaikilla laitteilla on nyt myös pääsy paikallisiin resursseihin.</span><span class="sxs-lookup"><span data-stu-id="9a2af-117">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="9a2af-118">Azure AD:ssä liitettyjen laitteiden paikallisiin resursseihin pääsy ei vaadi lisätoimia.</span><span class="sxs-lookup"><span data-stu-id="9a2af-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="9a2af-119">Tämä toiminto on integroitu Windows 10:ssä.</span><span class="sxs-lookup"><span data-stu-id="9a2af-119">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="9a2af-120">Jos haluat kirjautua AADJ-laitteeseen muulla kuin salasanamenetelmällä, kuten PIN/Bio-metrinen, WHFB-tunnistetietokirjautumisen kautta ja käyttää sitten paikallisia resursseja (jakoresursseja, tulostimia. jne.), seuraa https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="9a2af-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="9a2af-121">Jos organisaatiosi ei ole valmis ottamaan käyttöön edellä kuvattua Azure AD:ssä liitettyä laitemääritystä, harkitse Azure AD:ssä liitettyjen [yhdistelmälaitemääritysten käyttöönottoa.](manage-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="9a2af-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="9a2af-122">Huomioon otettavia seikkoja liittyessäsi Windows-laitteisiin Azure AD:ssä</span><span class="sxs-lookup"><span data-stu-id="9a2af-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="9a2af-123">Jos Azure-AD:llä liitetty Windows-laite on aiemmin liitetty toimialueeseen tai työryhmään, ota huomioon seuraavat rajoitukset:</span><span class="sxs-lookup"><span data-stu-id="9a2af-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="9a2af-124">Kun Azure AD -laite liittyy, se luo uuden käyttäjän viittaamatta aiemmin luotuun profiiliin.</span><span class="sxs-lookup"><span data-stu-id="9a2af-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="9a2af-125">Profiilit on siirrettävä manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="9a2af-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="9a2af-126">Käyttäjäprofiili sisältää tietoja, kuten suosikit, paikalliset tiedostot, selaimen asetukset ja aloitusvalikon asetukset.</span><span class="sxs-lookup"><span data-stu-id="9a2af-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="9a2af-127">Paras tapa on etsiä kolmannen osapuolen työkalu olemassa olevien tiedostojen ja asetusten kartoittamiseen uuteen profiiliin.</span><span class="sxs-lookup"><span data-stu-id="9a2af-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="9a2af-128">Jos laite käyttää ryhmäkäytäntöobjekteja (GPO), joillakin ryhmäkäytäntöobjekteilla ei ehkä ole vastaavaa kokoonpanopalveluntarjoajaa Intunessa. [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers)</span><span class="sxs-lookup"><span data-stu-id="9a2af-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="9a2af-129">Suorita [MMAT-työkalu löytääksesi](https://www.microsoft.com/download/details.aspx?id=45520) vastaavat CSPs:t olemassa oleville ryhmäkäytäntöobjekteille.</span><span class="sxs-lookup"><span data-stu-id="9a2af-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="9a2af-130">Käyttäjät eivät ehkä voi todentaa Sovelluksia, jotka ovat riippuvaisia Active Directory -todennuksista.</span><span class="sxs-lookup"><span data-stu-id="9a2af-130">Users might not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="9a2af-131">Arvioi vanha sovellus ja harkitse päivittämistä sovellukseen, joka käyttää modernia todnttia, jos mahdollista.</span><span class="sxs-lookup"><span data-stu-id="9a2af-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="9a2af-132">Active Directory -tulostimen etsintä ei toimi.</span><span class="sxs-lookup"><span data-stu-id="9a2af-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="9a2af-133">Voit määrittää suoran tulostimen polut kaikille käyttäjille tai käyttää [universaalia tulostusta.](/universal-print/)</span><span class="sxs-lookup"><span data-stu-id="9a2af-133">You can provide direct printer paths for all users or use [Universal Print](/universal-print/).</span></span>

### <a name="related-articles"></a><span data-ttu-id="9a2af-134">Aiheeseen liittyvät artikkelit</span><span class="sxs-lookup"><span data-stu-id="9a2af-134">Related Articles</span></span>

[<span data-ttu-id="9a2af-135">Azure AD Connectin edellytykset</span><span class="sxs-lookup"><span data-stu-id="9a2af-135">Prerequisites for Azure AD Connect</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
