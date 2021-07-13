---
title: Käytä paikallisia resursseja Azure AD:llä yhdistetystä laitteesta Microsoft 365 Businessissa
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
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Opi käyttämään yrityksen sovelluksia, jaetut tiedostoresurssit ja tulostimet tai muut paikallisen Azure Active Directory Windows 10 avulla.
ms.openlocfilehash: 71d60e0187c917dffb7390afcedf22dc73f44008
ms.sourcegitcommit: 00f001019c653269d85718d410f970887d904304
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/12/2021
ms.locfileid: "53393455"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="c30f2-103">Käytä paikallisia resursseja Azure AD:llä yhdistetystä laitteesta Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="c30f2-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="c30f2-104">Tämä artikkeli koskee Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c30f2-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="c30f2-105">Kaikki Windows 10, Azure Active Directory liitettyihin sovelluksiin, voivat käyttää kaikkia pilvipohjaisia resursseja, kuten Microsoft 365-sovelluksia, ja ne voidaan suojata Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c30f2-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="c30f2-106">Voit myös sallia pääsyn paikallisiin resursseihin, kuten liiketoiminta-sovelluksiin, jaekkeisiin ja tulostimien.</span><span class="sxs-lookup"><span data-stu-id="c30f2-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="c30f2-107">Salli käyttö käyttämällä [Azure AD Näyttöyhteys:tä](/azure/active-directory/connect/active-directory-aadconnect) paikallisen Active Directoryn synkronoinnissa Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c30f2-107">To allow access, use [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span>

<span data-ttu-id="c30f2-108">Lisätietoja on ohjeaiheessa Johdanto [laitehallintaan Azure Active Directory.](/azure/active-directory/device-management-introduction)</span><span class="sxs-lookup"><span data-stu-id="c30f2-108">To learn more, see [Introduction to device management in Azure Active Directory](/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="c30f2-109">Vaiheiden yhteenveto on myös seuraavissa osissa.</span><span class="sxs-lookup"><span data-stu-id="c30f2-109">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="c30f2-110">Azure AD -Näyttöyhteys</span><span class="sxs-lookup"><span data-stu-id="c30f2-110">Run Azure AD Connect</span></span>

<span data-ttu-id="c30f2-111">Suorita seuraavat vaiheet, jotta organisaatiosi Azure AD:llä yhdistetyt laitteet voivat käyttää paikallisia resursseja.</span><span class="sxs-lookup"><span data-stu-id="c30f2-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>

1. <span data-ttu-id="c30f2-112">Jos haluat synkronoida käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directory, suorita ohjattu hakemistosynkronointitoiminto ja Azure AD Näyttöyhteys artikkelissa Hakemistosynkronoinnin määrittäminen [Office 365.](../enterprise/set-up-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="c30f2-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](../enterprise/set-up-directory-synchronization.md).</span></span>

2. <span data-ttu-id="c30f2-113">Kun hakemistosynkronointi on valmis, varmista, että organisaation Windows 10 Azure AD:n liittäminen.</span><span class="sxs-lookup"><span data-stu-id="c30f2-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="c30f2-114">Tämä vaihe tehdään yksitellen kussakin Windows 10 laitteessa.</span><span class="sxs-lookup"><span data-stu-id="c30f2-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="c30f2-115">Lisätietoja [on Windows laitteiden Microsoft 365 Business Premium käyttäjille.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="c30f2-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span>

3. <span data-ttu-id="c30f2-116">Kun Windows 10 Azure AD:iin, jokaisen käyttäjän on käynnistettävä laitteensa uudelleen ja kirjauduttava Microsoft 365 Business Premium tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="c30f2-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="c30f2-117">Kaikilla laitteilla on nyt myös paikallisen resurssin käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="c30f2-117">All devices now have access to on-premises resources as well.</span></span>

<span data-ttu-id="c30f2-118">Azure AD:ssä liitettyjen laitteiden paikallisen resurssien käyttö ei vaadi lisätoimia.</span><span class="sxs-lookup"><span data-stu-id="c30f2-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="c30f2-119">Tämä toiminto on integroitu Windows 10.</span><span class="sxs-lookup"><span data-stu-id="c30f2-119">This functionality is built into Windows 10.</span></span>

<span data-ttu-id="c30f2-120">Jos haluat kirjautua AADJ-laitteeseen muulla kuin salasanamenetelmällä, kuten PIN-/Bio-metrijärjestelmän kanssa WHFB-tunnistetietokirjautumisen kautta ja käyttää sitten paikallisia resursseja (jakoresursseja, tulostimia jne.), noudata tätä [artikkelia.](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)</span><span class="sxs-lookup"><span data-stu-id="c30f2-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares, printers, etc.), please follow [this article](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="c30f2-121">Jos organisaatiosi ei ole valmis ottamaan käyttöön edellä kuvatun Azure AD:n liitettyjen laitteiden määrityksessä, harkitse [Azure AD:llä yhdistetyn laitteen yhdistelmäkokoonpanon käyttöönottoa.](manage-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="c30f2-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>

### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="c30f2-122">Huomioon otettavia asioita, kun Windows laitteisiin Azure AD:ssä</span><span class="sxs-lookup"><span data-stu-id="c30f2-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="c30f2-123">Jos Windows laite, jonka kanssa Azure-AD on liitetty, oli aiemmin liitetty toimialueeseen tai työryhmään, ota seuraavat rajoitukset huomioon:</span><span class="sxs-lookup"><span data-stu-id="c30f2-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>

- <span data-ttu-id="c30f2-124">Kun azure AD -laite liittyy, se luo uuden käyttäjän viittaamatta aiemmin luotuun profiiliin.</span><span class="sxs-lookup"><span data-stu-id="c30f2-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="c30f2-125">Profiilit on siirrettävä manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="c30f2-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="c30f2-126">Käyttäjäprofiili sisältää tietoja, kuten suosikit, paikalliset tiedostot, selaimen asetukset ja aloitusvalikko asetukset.</span><span class="sxs-lookup"><span data-stu-id="c30f2-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="c30f2-127">Paras tapa on etsiä kolmannen osapuolen työkalu, jolla olemassa olevat tiedostot ja asetukset voidaan yhdistää uuteen profiiliin.</span><span class="sxs-lookup"><span data-stu-id="c30f2-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="c30f2-128">Jos laite käyttää ryhmäkäytäntöobjekteja (GPO), joillakin ryhmäkäytäntöobjekteilla ei välttämättä ole vastaavaa kokoonpanopalveluntarjoajaa Intunessa. [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers)</span><span class="sxs-lookup"><span data-stu-id="c30f2-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="c30f2-129">Suorita [MMAT-työkalu löytääksesi](https://www.microsoft.com/download/details.aspx?id=45520) vastaavat CSPs olemassa oleville ryhmäkäytäntöobjekteille.</span><span class="sxs-lookup"><span data-stu-id="c30f2-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="c30f2-130">Käyttäjät eivät ehkä voi todentaa Sovelluksia, jotka ovat riippuvaisia Active Directory -todennuksista.</span><span class="sxs-lookup"><span data-stu-id="c30f2-130">Users might not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="c30f2-131">Arvioi vanha sovellus ja harkitse päivitystä sovellukseen, joka käyttää modernia todnttia, jos mahdollista.</span><span class="sxs-lookup"><span data-stu-id="c30f2-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="c30f2-132">Active Directory -tulostimen etsintä ei toimi.</span><span class="sxs-lookup"><span data-stu-id="c30f2-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="c30f2-133">Voit määrittää suoran tulostimen polut kaikille käyttäjille tai käyttää [universaalia tulostusta.](/universal-print/)</span><span class="sxs-lookup"><span data-stu-id="c30f2-133">You can provide direct printer paths for all users or use [Universal Print](/universal-print/).</span></span>

### <a name="related-articles"></a><span data-ttu-id="c30f2-134">Aiheeseen liittyvät artikkelit</span><span class="sxs-lookup"><span data-stu-id="c30f2-134">Related Articles</span></span>

[<span data-ttu-id="c30f2-135">Azure AD :n käytön edellytykset Näyttöyhteys</span><span class="sxs-lookup"><span data-stu-id="c30f2-135">Prerequisites for Azure AD Connect</span></span>](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
