---
title: Yleistietoja määrityksestä
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
description: Opi ohjeet esimerkiksi Microsoft 365 Business Premium tilaamiseen, toimialueen ja käyttäjien lisäämiseen, suojauskäytäntöjen määrittämiseen ja paljon muuta.
ms.openlocfilehash: 008a5c51698589667acc0d01649f67dab33b4c58
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245060"
---
# <a name="overview-of-setup"></a><span data-ttu-id="8cc24-103">Yleistietoja määrityksestä</span><span class="sxs-lookup"><span data-stu-id="8cc24-103">Overview of setup</span></span>

<span data-ttu-id="8cc24-104">Katso lyhyt video Microsoft 365 Business Premium määrityksestä.</span><span class="sxs-lookup"><span data-stu-id="8cc24-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="8cc24-105">Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](../business-video/index.yml).</span><span class="sxs-lookup"><span data-stu-id="8cc24-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](../business-video/index.yml).</span></span>

<span data-ttu-id="8cc24-106">Useimmat määritysvaiheet voidaan tehdä ohjatussa määrityksessä, mutta myös muut vaihtoehdot on lueteltu.</span><span class="sxs-lookup"><span data-stu-id="8cc24-106">Most of the setup steps can be done in the guided setup, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="8cc24-107">Vaihe 1: Toimialueen ja käyttäjien lisääminen</span><span class="sxs-lookup"><span data-stu-id="8cc24-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="8cc24-108">**[Lisää toimialue](set-up.md#add-your-domain-to-personalize-sign-in)** (jos ostit toimialueen [rekisteröitymisen aikana,](sign-up.md)tämä vaihe on jo valmis.)</span><span class="sxs-lookup"><span data-stu-id="8cc24-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

   - <span data-ttu-id="8cc24-109">**Käyttäjien lisääminen**.</span><span class="sxs-lookup"><span data-stu-id="8cc24-109">**Add users**.</span></span> <span data-ttu-id="8cc24-110">Voit lisätä käyttäjiä kolmella tavalla:</span><span class="sxs-lookup"><span data-stu-id="8cc24-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="8cc24-111">Ohjatussa [määrityksessä](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="8cc24-111">In the [guided setup](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="8cc24-112">Hakemistosynkronoinnin [avulla voit lisätä käyttäjiä Azure AD Näyttöyhteys,](../enterprise/set-up-directory-synchronization.md) jos käytössäsi on paikallinen Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8cc24-112">Use directory synchronization to [add users by using Azure AD Connect](../enterprise/set-up-directory-synchronization.md) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="8cc24-113">Voit myös [lisätä käyttäjiä myöhemmin](../admin/add-users/add-users.md) hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="8cc24-113">You can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="8cc24-114">Vaihe 2: Suojauskäytäntöjen määrittäminen ja laitteiden määrittäminen</span><span class="sxs-lookup"><span data-stu-id="8cc24-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="8cc24-115">Voit määrittää [laitekäytännöt ohjatun](set-up.md#protect-your-organization) asennuksen avulla.</span><span class="sxs-lookup"><span data-stu-id="8cc24-115">Use the [guided setup](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="8cc24-116">Voit myös lisätä tai muokata niitä myöhemmin [hallintakeskuksessa ja](view-policies-and-devices.md) [Intune-portaalissa.](/intune/tutorial-walkthrough-intune-portal)</span><span class="sxs-lookup"><span data-stu-id="8cc24-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="8cc24-117">Ohjattu määritystoiminto määrittää myös uhkien ja tietojen menetyksen estämisen perusasetukset.</span><span class="sxs-lookup"><span data-stu-id="8cc24-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="8cc24-118">Ohjatun määritystoiminnon suojausasetusten lisäksi voit parantaa suojaustasi lisäämällä seuraavat asetukset:</span><span class="sxs-lookup"><span data-stu-id="8cc24-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="8cc24-119">**Sähköpostin haittaohjelmien torjunta**</span><span class="sxs-lookup"><span data-stu-id="8cc24-119">**Email malware protection**</span></span>
- <span data-ttu-id="8cc24-120">**Defender for Office 365**</span><span class="sxs-lookup"><span data-stu-id="8cc24-120">**Anti-phishing in Defender for Office 365**</span></span>
- <span data-ttu-id="8cc24-121">**Exchange Online Archiving**</span><span class="sxs-lookup"><span data-stu-id="8cc24-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="8cc24-122">**Azure Information Protection (Palvelupaketti1)**</span><span class="sxs-lookup"><span data-stu-id="8cc24-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="8cc24-123">Aloita tutustumaan [uhkien uhkien suojauksen](increase-threat-protection.md) [lisäämis- ja yhteensopivuusominaisuuksien määritettyihin ominaisuuksiin.](set-up-compliance.md)</span><span class="sxs-lookup"><span data-stu-id="8cc24-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="8cc24-124">Katso myös [10 tapaa suojata Microsoft 365 Business Premium,](/office365/admin/security-and-compliance/secure-your-business-data) joissa on parhaat suojauskäytännöt.</span><span class="sxs-lookup"><span data-stu-id="8cc24-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](/office365/admin/security-and-compliance/secure-your-business-data) for a road-map of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="8cc24-125">Vaihe 3: Laitteiden Windows 10 hallinta</span><span class="sxs-lookup"><span data-stu-id="8cc24-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="8cc24-126">Kun olet suorittanut ohjatun määrityksen, haluat suojata Windows 10 tietokoneita organisaatiossasi.</span><span class="sxs-lookup"><span data-stu-id="8cc24-126">After you complete the guided setup, you will want to protect all the Windows 10 computers in your organization.</span></span>
  
- <span data-ttu-id="8cc24-127">Windows 10 Pro on edellytys [](pre-requisites-for-data-protection.md) Microsoft 365 Business Premium:lle, mutta jos sinulla on Windows 7 Pro, Windows 8 Pro tai Windows 8.1 Pro, tilauksesi oikeuttaa sinut päivittämään [Windows 10 Pro.](./upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="8cc24-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](./upgrade-to-windows-pro-creators-update.md).</span></span>
- <span data-ttu-id="8cc24-128">Määritä käytännöt [mobiililaitteille Windows 10](secure-win-10-pcs.md) tietokoneissa noudattamalla Windows 10 ohjeita.</span><span class="sxs-lookup"><span data-stu-id="8cc24-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="8cc24-129">Kun liityt Windows 10 Azure AD:iin, Windows 10-tietokoneillesi määrittäjät käytännöt otetaan käyttöön.</span><span class="sxs-lookup"><span data-stu-id="8cc24-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="8cc24-130">Lisätietoja on kohdassa Laitteiden [Windows Microsoft 365 käyttäjille.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="8cc24-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="8cc24-131">Vaihe 4: Microsoft 365 -sovellukset yrityksille</span><span class="sxs-lookup"><span data-stu-id="8cc24-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="8cc24-132">Voit asentaa Office automaattisesti Windows -laitteisiin ohjatun [määritystoiminnon avulla.](set-up.md#deploy-office-365-client-apps)</span><span class="sxs-lookup"><span data-stu-id="8cc24-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="8cc24-133">Anna käyttäjien [asentaa Office sovelluksia](/office365/admin/setup/install-applications) Windows ja laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="8cc24-133">Let users [install Office apps](/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="8cc24-134">Tarkennettu</span><span class="sxs-lookup"><span data-stu-id="8cc24-134">Advanced</span></span>
- <span data-ttu-id="8cc24-135">**Uusien laitteiden määritäminen Autopilotin avulla**</span><span class="sxs-lookup"><span data-stu-id="8cc24-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="8cc24-136">Voit käyttää [Windows Autopilotia](add-autopilot-devices-and-profile.md) uusien **Windows 10** esimääritykseen automaattisesti käyttäjälle, mutta voi olla helpompaa saada [](https://www.microsoft.com/solution-providers/search) kumppani, joka voi tehdä tämän.</span><span class="sxs-lookup"><span data-stu-id="8cc24-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="8cc24-137">Voit myös Microsoft Store [](https://go.microsoft.com/fwlink/?linkid=874598)-sovellukselle ja pyytää pilvitekniikan asiantuntijaa asettamaan uudet laitteet, jotka ostat.</span><span class="sxs-lookup"><span data-stu-id="8cc24-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="8cc24-138">**Käytä paikallisia resursseja**</span><span class="sxs-lookup"><span data-stu-id="8cc24-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="8cc24-139">Jos organisaatiosi käyttää Windows Server Active Directorya paikallisesti, voit määrittää Microsoft 365 Business Premium:n suojaamaan Windows 10-laitteitasi säilyttäen edelleen paikallisen todentamisen edellyttävän paikallisen todentamisen resurssien käyttöoikeuden.</span><span class="sxs-lookup"><span data-stu-id="8cc24-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="8cc24-140">Määritä tämä noudattamalla [ohjeita, jotka Windows 10 toimialueisiin](manage-windows-devices.md) liitettyjen laitteiden Microsoft 365 Business Premium hallitaan.</span><span class="sxs-lookup"><span data-stu-id="8cc24-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="8cc24-141">Tämä on ensisijainen menetelmä, ja tässä tilassa oleetut laitteet ovat Azure AD:n yhdistelmälaitteisiin liitettyjä laitteita.</span><span class="sxs-lookup"><span data-stu-id="8cc24-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="8cc24-142">Jos yritykselläsi on paikallinen Active Directory, joka sisältää paikallisia resursseja (kuten jaetut tiedostoresurssit ja tulostimet), voit antaa Azure AD:lle liitettyjen laitteiden käyttöoikeudet näihin resursseihin noudattamalla seuraavia ohjeita: Paikallisten resurssien käyttäminen Azure AD:llä yhdistetystä [laitteesta Microsoft 365 Business Premium.](access-resources.md)</span><span class="sxs-lookup"><span data-stu-id="8cc24-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="related-content"></a><span data-ttu-id="8cc24-143">Aiheeseen liittyvä sisältö</span><span class="sxs-lookup"><span data-stu-id="8cc24-143">Related content</span></span>

<span data-ttu-id="8cc24-144">[Microsoft 365 yrityksille 2010 -koulutusvideoita](../business-video/index.yml) (linkkisivu)</span><span class="sxs-lookup"><span data-stu-id="8cc24-144">[Microsoft 365 for business training videos](../business-video/index.yml) (link page)</span></span>