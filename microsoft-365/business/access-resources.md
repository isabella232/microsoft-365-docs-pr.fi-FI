---
title: Paikallisten resurssien käyttäminen Azure AD-liitetyissä laitteissa Microsoft 365 Business-sovelluksessa
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Opi, miten voit käyttää paikallisia resursseja, kuten yritys sovelluksia, jaettuja tiedostoja ja tulostimia Azure Active Directorysta, jotka liittyivät Windows 10-laitteeseen.
ms.openlocfilehash: 9b83781afee746b06bbdf90962de0f55ffbcb118
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/29/2020
ms.locfileid: "47307489"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="b5737-103">Paikallisten resurssien käyttäminen Azure AD-liitetyissä laitteissa Microsoft 365 Business Premiumissa</span><span class="sxs-lookup"><span data-stu-id="b5737-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="b5737-104">Tämä artikkeli koskee Microsoft 365 Business Premiumia.</span><span class="sxs-lookup"><span data-stu-id="b5737-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="b5737-105">Mikä tahansa Windows 10-laite, joka on Azure Active Directory liitetty, voi käyttää kaikkia pilvipohjaisia resursseja, kuten Microsoft 365-sovelluksia, ja se on suojattu Microsoft 365 Business Premiumin avulla.</span><span class="sxs-lookup"><span data-stu-id="b5737-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="b5737-106">Voit myös sallia paikallisten resurssien, kuten yritys sovellusten, jaettujen tiedostojen ja tulostimien, käytön.</span><span class="sxs-lookup"><span data-stu-id="b5737-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="b5737-107">Jos haluat sallia käyttö oikeuden, synkronoi paikallinen Active Directory Azure Active Directoryssa Azure [AD Connectin](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) avulla.</span><span class="sxs-lookup"><span data-stu-id="b5737-107">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="b5737-108">Lisä tietoja on artikkelissa [Johdatus laite hallintaan Azure Active Directoryssa](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="b5737-108">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="b5737-109">Vaiheet on koottu myös seuraaviin kohtiin.</span><span class="sxs-lookup"><span data-stu-id="b5737-109">The steps are also summarized in the following sections.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b5737-110">Tämä toiminto on käytettävissä vain OAuth-ja NTLM-muodoissa.</span><span class="sxs-lookup"><span data-stu-id="b5737-110">This procedure is only applicable to OAuth and NTLM.</span></span> <span data-ttu-id="b5737-111">Kerberos-protokollaa ei voi käyttää.</span><span class="sxs-lookup"><span data-stu-id="b5737-111">Kerberos is not supported.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="b5737-112">Azure AD Connectin suorittaminen</span><span class="sxs-lookup"><span data-stu-id="b5737-112">Run Azure AD Connect</span></span>

<span data-ttu-id="b5737-113">Noudata seuraavia vaiheita, jotta organisaatiosi Azure AD-laitteet voivat käyttää paikallisia resursseja.</span><span class="sxs-lookup"><span data-stu-id="b5737-113">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="b5737-114">Synkronoi käyttäjät, ryhmät ja yhteys tiedot paikallisesta Active Directorysta Azure Active Directoryyn suorittamalla ohjattu hakemisto synkronointi ja Azure AD Connect kohdassa [Office 365-hakemisto synkronoinnin määrittäminen](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization)kuvatulla tavalla.</span><span class="sxs-lookup"><span data-stu-id="b5737-114">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization).</span></span>
    
2. <span data-ttu-id="b5737-115">Kun hakemisto synkronointi on valmis, varmista, että organisaatiosi Windows 10-laitteet on liitetty Azure AD:hen.</span><span class="sxs-lookup"><span data-stu-id="b5737-115">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="b5737-116">Tämä vaihe suoritetaan yksitellen kaikissa Windows 10-laitteissa.</span><span class="sxs-lookup"><span data-stu-id="b5737-116">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="b5737-117">Lisä tietoja on Ohje aiheessa [Windows-laitteiden määrittäminen Microsoft 365 Business Premium-käyttäjille](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="b5737-117">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="b5737-118">Kun Windows 10-laitteet on liitetty Azure AD:hen, jokaisen käyttäjän on käynnistettävä laitteensa uudelleen ja kirjauduttava sisään Microsoft 365 Business Premium-tunniste tiedoillaan.</span><span class="sxs-lookup"><span data-stu-id="b5737-118">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="b5737-119">Kaikki laitteet voivat nyt käyttää myös paikallisia resursseja.</span><span class="sxs-lookup"><span data-stu-id="b5737-119">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="b5737-120">Muita vaiheita ei tarvita, jotta voit käyttää paikallisia resursseja Azure AD-laitteeseen liitetyissä laitteissa.</span><span class="sxs-lookup"><span data-stu-id="b5737-120">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="b5737-121">Tämä toiminto on sisällytetty Windows 10: een.</span><span class="sxs-lookup"><span data-stu-id="b5737-121">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="b5737-122">Jos haluat kirja utua AADJ-laitteeseen, joka ei ole sama kuin salasana menetelmä, kuten PIN/Bio-metric WHFB-tunniste tietojen kirjautumistoiminnolla, ja sitten käyttää paikallisia resursseja (osakkeita, tulostimia... jne.), noudata seuraavia ohjeita. https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="b5737-122">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="b5737-123">Jos organisaatiosi ei ole valmis ottamaan käyttöön edellä kuvattua Azuren Active Device-määritystä, harkitse [yhdistelmä Azure AD-liitetyn laite kokoonpanon](manage-windows-devices.md)määrittämistä.</span><span class="sxs-lookup"><span data-stu-id="b5737-123">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="b5737-124">Huomioitavaa, kun liityt Windows-laitteisiin Azure AD:hen</span><span class="sxs-lookup"><span data-stu-id="b5737-124">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="b5737-125">Jos Windows-laite, jonka Azure-AD on liittynyt aiemmin toimi alueen mukaan tai työryhmään, huomioi seuraavat rajoitukset:</span><span class="sxs-lookup"><span data-stu-id="b5737-125">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="b5737-126">Kun laite Azure AD liittyy, se luo uuden käyttäjän viittaamatta olemassa olevaan profiiliin.</span><span class="sxs-lookup"><span data-stu-id="b5737-126">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="b5737-127">Profiilit on siirrettävä manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="b5737-127">Profiles must be manually migrated.</span></span> <span data-ttu-id="b5737-128">Käyttäjä profiili sisältää tietoja, kuten Suosikit, paikalliset tiedostot, selaimen asetukset ja aloitus valikon asetukset.</span><span class="sxs-lookup"><span data-stu-id="b5737-128">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="b5737-129">Paras tapa on löytää kolmannen osapuolen työkalu, jonka avulla voit yhdistää nykyiset tiedostot ja asetukset uuteen profiiliin.</span><span class="sxs-lookup"><span data-stu-id="b5737-129">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="b5737-130">Jos laite käyttää ryhmä käytäntö objekteja, joillakin ryhmä käytäntö objekteilla ei ehkä ole vastaavaa [määritys palveluiden tarjoajaa](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) Intunella.</span><span class="sxs-lookup"><span data-stu-id="b5737-130">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="b5737-131">Jos haluat etsiä olemassa olevia ryhmä käytäntö objekteja, käytä [mmat-työkalua](https://www.microsoft.com/download/details.aspx?id=45520) .</span><span class="sxs-lookup"><span data-stu-id="b5737-131">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="b5737-132">Käyttäjät eivät pysty todentamaan sovelluksia, jotka ovat riippuvaisia Active Directory-todennuksesta.</span><span class="sxs-lookup"><span data-stu-id="b5737-132">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="b5737-133">Voit arvioida vanhaa sovellusta ja päivittää sitä sovellukseen, joka käyttää modernia todennus ohjelmaa, jos se on mahdollista.</span><span class="sxs-lookup"><span data-stu-id="b5737-133">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="b5737-134">Active Directory-tulostimen etsintä ei toimi.</span><span class="sxs-lookup"><span data-stu-id="b5737-134">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="b5737-135">Voit määrittää kaikille käyttäjille suorat tulostus polut tai käyttää [yhdistelmä pilvi tulostusta](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="b5737-135">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
