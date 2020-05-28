---
title: Asennuksen yleiskatsaus
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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Lue Tietoja Microsoft 365 Business Premiumin määritysvaiheista, tilaamisesta, toimialueen ja käyttäjien lisäämisestä, suojauskäytäntöjen määrittämisestä ja muusta.
ms.openlocfilehash: 80243fac6ca2efcfca030b6ee1c1113c026a80ce
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/27/2020
ms.locfileid: "44402974"
---
# <a name="overview-of-setup"></a><span data-ttu-id="b1ed6-103">Asennuksen yleiskatsaus</span><span class="sxs-lookup"><span data-stu-id="b1ed6-103">Overview of setup</span></span>

<span data-ttu-id="b1ed6-104">Katso lyhyt video Microsoft 365 Business Premiumin asennuksesta.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="b1ed6-105">Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="b1ed6-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="b1ed6-106">Useimmat asennusvaiheet voidaan tehdä ohjatussa asennustoiminnossa, mutta myös muut asetukset on lueteltu.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-106">Most of the setup steps can be done in the setup wizard, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="b1ed6-107">Vaihe 1: Toimialueen ja käyttäjien lisääminen</span><span class="sxs-lookup"><span data-stu-id="b1ed6-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="b1ed6-108">**[Lisää toimialue (jos](set-up.md#add-your-domain-to-personalize-sign-in)** ostit verkkotunnuksen [rekisteröityessäsi,](sign-up.md)tämä vaihe on jo tehty.)</span><span class="sxs-lookup"><span data-stu-id="b1ed6-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="b1ed6-109">**Lisää käyttäjiä**.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-109">**Add users**.</span></span> <span data-ttu-id="b1ed6-110">Voit lisätä käyttäjiä millä tahansa seuraavista kolmesta tavasta:</span><span class="sxs-lookup"><span data-stu-id="b1ed6-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="b1ed6-111">[Ohjatussa toiminnossa.](set-up.md#add-users-in-the-wizard)</span><span class="sxs-lookup"><span data-stu-id="b1ed6-111">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="b1ed6-112">Hakemistosynkronoinnin avulla voit [lisätä käyttäjiä Azure AD Connectin avulla,](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) jos käytössäsi on paikallinen Active-hakemisto.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-112">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="b1ed6-113">Voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallintakeskukseen.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="b1ed6-114">Vaihe 2: Suojauskäytäntöjen määrittäminen ja laitteiden määrittäminen</span><span class="sxs-lookup"><span data-stu-id="b1ed6-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="b1ed6-115">Määritä laitekäytännöt [ohjatun asennustoiminnon](set-up.md#protect-your-organization) avulla.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-115">Use the [Setup wizard](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="b1ed6-116">Voit myös lisätä niitä tai muokata niitä myöhemmin [hallintakeskuksessa](view-policies-and-devices.md) ja [Intune-portaalissa.](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)</span><span class="sxs-lookup"><span data-stu-id="b1ed6-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="b1ed6-117">Ohjattu asennustoiminto määrittää myös uhkien suojauksen ja tietojen menetyksen estämisen perusasetukset.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="b1ed6-118">Ohjatun asennustoiminnon suojausasetusten lisäksi voit parantaa suojausta lisäämällä seuraavat asetukset:</span><span class="sxs-lookup"><span data-stu-id="b1ed6-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="b1ed6-119">**Sähköposti haittaohjelmien torjunta**</span><span class="sxs-lookup"><span data-stu-id="b1ed6-119">**Email malware protection**</span></span>
- <span data-ttu-id="b1ed6-120">**ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="b1ed6-120">**ATP anti-phishing**</span></span>
- <span data-ttu-id="b1ed6-121">**Exchange Online Archiving**</span><span class="sxs-lookup"><span data-stu-id="b1ed6-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="b1ed6-122">**Azure-tietojen suojaus (suunnitelma1)**</span><span class="sxs-lookup"><span data-stu-id="b1ed6-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="b1ed6-123">Lisätietoja on ohjeessa [Uhkien suojauksen lisääminen](increase-threat-protection.md) ja [vaatimustenmukaisuusominaisuuksien määrittäminen](set-up-compliance.md).</span><span class="sxs-lookup"><span data-stu-id="b1ed6-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="b1ed6-124">Katso myös [kymmenen parasta tapaa suojata Microsoft 365 Business Premium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) ja tutustu parhaisiin tietoturvakäytäntöihin.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="b1ed6-125">Vaihe 3: Windows 10 -laitteiden määrittäminen ja hallinta</span><span class="sxs-lookup"><span data-stu-id="b1ed6-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="b1ed6-126">Kun olet suorittanut ohjatun määritystoiminnon, haluat proctect kaikki Windwos 10 tietokoneet organisaatiossa.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-126">After you run the set up wizard, you will want to proctect all the Windwos 10 computers in your organization.</span></span>
  
- <span data-ttu-id="b1ed6-127">Windows 10 Pro on Microsoft 365 Business Premiumin [edellytys,](pre-requisites-for-data-protection.md) mutta jos sinulla on Windows 7 Pro, Windows 8 Pro tai Windows 8.1 Pro, tilauksesi oikeuttaa [päivittämään Windows 10 Pro -versioon](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="b1ed6-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
- <span data-ttu-id="b1ed6-128">Määritä Windows [10 -laitteiden käytännöt noudattamalla suojattujen Windows 10 -tietokoneiden](secure-win-10-pcs.md) ohjeita.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="b1ed6-129">Kun liityt Windows 10 -laitteeseen Azure AD:hen, Windows 10 -tietokoneille määrittämäsi käytännöt otetaan käyttöön.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="b1ed6-130">Lisätietoja on ohjeaiheessa [Windows-laitteiden määrittäminen Microsoft 365 -käyttäjille](set-up-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="b1ed6-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="b1ed6-131">Vaihe 4: Asenna Microsoft 365 Apps for Business</span><span class="sxs-lookup"><span data-stu-id="b1ed6-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="b1ed6-132">Voit asentaa Officen automaattisesti Windows-laitteisiin [ohjatun asennustoiminnon](set-up.md#deploy-office-365-client-apps)avulla.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="b1ed6-133">Anna käyttäjien [asentaa Office-sovelluksia](https://docs.microsoft.com/office365/admin/setup/install-applications) Windowsille ja laitteille.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-133">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="b1ed6-134">Kehittynyt</span><span class="sxs-lookup"><span data-stu-id="b1ed6-134">Advanced</span></span>
- <span data-ttu-id="b1ed6-135">**Uusien laitteiden määrittäminen automaattiohjauksen avulla**</span><span class="sxs-lookup"><span data-stu-id="b1ed6-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="b1ed6-136">[Windowsin automaattiohjauksen](add-autopilot-devices-and-profile.md) avulla voit määrittää **käyttäjälle** automaattisesti uudet Windows 10 -laitteet, mutta voi olla helpompaa saada [kumppani,](https://www.microsoft.com/solution-providers/search) joka voi tehdä tämän puolestasi.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="b1ed6-137">Voit myös siirtyä [Microsoft Storeen](https://go.microsoft.com/fwlink/?linkid=874598)ja pyytää pilvitekniikan asiantuntijaa asettamaan ostamasi uudet laitteet.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="b1ed6-138">**Paikallisten resurssien käyttäminen**</span><span class="sxs-lookup"><span data-stu-id="b1ed6-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="b1ed6-139">Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Business Premiumin suojaamaan Windows 10 -laitteita ja säilyttämään silti paikallisen todennuksen edellyttävien paikallisten resurssien käytön.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="b1ed6-140">Määritä tämä noudattamalla kohdan [Microsoft 365 Business Premiumin hallitsemien toimialueeseen liitettyjen Windows 10 -laitteiden ottaminen käyttöön](manage-windows-devices.md) -kohdan ohjeita.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="b1ed6-141">Tämä on ensisijainen menetelmä, ja tämän tilan laitteita kutsutaan Hybrid Azure AD -liitetyiksi laiteiksi.</span><span class="sxs-lookup"><span data-stu-id="b1ed6-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="b1ed6-142">Jos yritykselläsi on paikallinen Active Directory, joka sisältää joitakin paikallisia resursseja (kuten jaettuja tiedostoja ja tulostimia), voit antaa Azure AD:hen liitetyille laitteille näiden resurssien käyttöoikeuden noudattamalla seuraavia ohjeita: [Paikallisten resurssien käyttäminen Azure AD:hen liitetystä laitteesta Microsoft 365 Business Premiumissa](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="b1ed6-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="b1ed6-143">Tutustu myös seuraaviin ohjeartikkeleihin:</span><span class="sxs-lookup"><span data-stu-id="b1ed6-143">See also</span></span>

[<span data-ttu-id="b1ed6-144">Microsoft 365 yrityksille koulutus videoita</span><span class="sxs-lookup"><span data-stu-id="b1ed6-144">Microsoft 365 for business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
