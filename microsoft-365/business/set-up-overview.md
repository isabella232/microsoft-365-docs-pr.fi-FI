---
title: Asennuksen yleiskatsaus
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
description: Tutustu Microsoft 365 Business Premiumin määritysvaiheisiin, kuten tilaamiseen, toimialueen ja käyttäjien lisäämiseen, suojauskäytäntöjen määrittämiseen ja paljon muuta.
ms.openlocfilehash: 749acbfdbde92ad97b09dc720c85dd850b76c9cf
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579930"
---
# <a name="overview-of-setup"></a><span data-ttu-id="c6c71-103">Asennuksen yleiskatsaus</span><span class="sxs-lookup"><span data-stu-id="c6c71-103">Overview of setup</span></span>

<span data-ttu-id="c6c71-104">Katso lyhyt video Microsoft 365 Business Premiumin määrityksestä.</span><span class="sxs-lookup"><span data-stu-id="c6c71-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="c6c71-105">Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="c6c71-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="c6c71-106">Useimmat määritysvaiheet voidaan tehdä ohjatussa määrityksessä, mutta myös muut vaihtoehdot on lueteltu.</span><span class="sxs-lookup"><span data-stu-id="c6c71-106">Most of the setup steps can be done in the guided setup, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="c6c71-107">Vaihe 1: Toimialueen ja käyttäjien lisääminen</span><span class="sxs-lookup"><span data-stu-id="c6c71-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="c6c71-108">**[Lisää toimialue](set-up.md#add-your-domain-to-personalize-sign-in)** (jos ostit toimialueen rekisteröitymisen [aikana,](sign-up.md)tämä vaihe on jo valmis.)</span><span class="sxs-lookup"><span data-stu-id="c6c71-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

   - <span data-ttu-id="c6c71-109">**Lisää käyttäjiä.**</span><span class="sxs-lookup"><span data-stu-id="c6c71-109">**Add users**.</span></span> <span data-ttu-id="c6c71-110">Voit lisätä käyttäjiä kolmella tavalla:</span><span class="sxs-lookup"><span data-stu-id="c6c71-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="c6c71-111">Ohjatussa [määrityksessä.](set-up.md#add-users-in-the-wizard)</span><span class="sxs-lookup"><span data-stu-id="c6c71-111">In the [guided setup](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="c6c71-112">Hakemistosynkronoinnin [avulla voit lisätä käyttäjiä Azure AD Connectin](../enterprise/set-up-directory-synchronization.md) avulla, jos käytössäsi on paikallinen Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c6c71-112">Use directory synchronization to [add users by using Azure AD Connect](../enterprise/set-up-directory-synchronization.md) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="c6c71-113">Voit myös [lisätä käyttäjiä myöhemmin](../admin/add-users/add-users.md) hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="c6c71-113">You can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="c6c71-114">Vaihe 2: Suojauskäytäntöjen määrittäminen ja laitteiden määrittäminen</span><span class="sxs-lookup"><span data-stu-id="c6c71-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="c6c71-115">Määritä [laitekäytännöt ohjatun](set-up.md#protect-your-organization) asennuksen avulla.</span><span class="sxs-lookup"><span data-stu-id="c6c71-115">Use the [guided setup](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="c6c71-116">Voit myös lisätä tai muokata niitä myöhemmin [hallintakeskuksessa ja](view-policies-and-devices.md) [Intune-portaalissa.](/intune/tutorial-walkthrough-intune-portal)</span><span class="sxs-lookup"><span data-stu-id="c6c71-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="c6c71-117">Ohjattu määritystoiminto määrittää myös uhkien ja tietojen menetyksen estämisen perusasetukset.</span><span class="sxs-lookup"><span data-stu-id="c6c71-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="c6c71-118">Ohjatun määritystoiminnon suojausasetusten lisäksi voit parantaa suojausta lisäämällä seuraavat asetukset:</span><span class="sxs-lookup"><span data-stu-id="c6c71-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="c6c71-119">**Sähköpostin haittaohjelmasuojaus**</span><span class="sxs-lookup"><span data-stu-id="c6c71-119">**Email malware protection**</span></span>
- <span data-ttu-id="c6c71-120">**Tietojen kalastelun esto Office 365:n Defenderissä**</span><span class="sxs-lookup"><span data-stu-id="c6c71-120">**Anti-phishing in Defender for Office 365**</span></span>
- <span data-ttu-id="c6c71-121">**Exchange Online Archiving**</span><span class="sxs-lookup"><span data-stu-id="c6c71-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="c6c71-122">**Azure Information Protection (Plan1)**</span><span class="sxs-lookup"><span data-stu-id="c6c71-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="c6c71-123">Aloita tutustumaan [uhkien suojauksen lisäämis-](increase-threat-protection.md) [ja yhteensopivuusominaisuuksien ominaisuuksiin.](set-up-compliance.md)</span><span class="sxs-lookup"><span data-stu-id="c6c71-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="c6c71-124">Katso myös [10 parasta tapaa suojata Microsoft 365 Business Premium](/office365/admin/security-and-compliance/secure-your-business-data) parhaat suojauskäytännöt.</span><span class="sxs-lookup"><span data-stu-id="c6c71-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](/office365/admin/security-and-compliance/secure-your-business-data) for a road-map of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="c6c71-125">Vaihe 3: Windows 10 -laitteiden määritäminen ja hallinta</span><span class="sxs-lookup"><span data-stu-id="c6c71-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="c6c71-126">Kun olet suorittanut ohjatun määrityksen, haluat suojata kaikki organisaatiosi Windows 10 -tietokoneet.</span><span class="sxs-lookup"><span data-stu-id="c6c71-126">After you complete the guided setup, you will want to protect all the Windows 10 computers in your organization.</span></span>
  
- <span data-ttu-id="c6c71-127">Windows 10 Pro [](pre-requisites-for-data-protection.md) on Microsoft 365 Business Premiumin edellytys, mutta jos sinulla on Windows 7 Pro, Windows 8 Pro tai Windows 8.1 Pro, tilauksesi oikeuttaa sinut päivittämään [Windows 10 Pro -versioon.](./upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="c6c71-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](./upgrade-to-windows-pro-creators-update.md).</span></span>
- <span data-ttu-id="c6c71-128">Määritä Windows [10 -laitteiden käytännöt](secure-win-10-pcs.md) noudattamalla suojattujen Windows 10 -tietokoneiden ohjeita.</span><span class="sxs-lookup"><span data-stu-id="c6c71-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="c6c71-129">Kun liityt Windows 10 -laitteeseen Azure AD:ssä, Windows 10 -tietokoneille määritettyjä käytäntöjä sovelletaan siihen.</span><span class="sxs-lookup"><span data-stu-id="c6c71-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="c6c71-130">Lisätietoja on kohdassa [Windows-laitteiden asennus Microsoft 365 -käyttäjille.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="c6c71-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="c6c71-131">Vaihe 4: Microsoft 365 -sovellusten asentaminen yrityksille</span><span class="sxs-lookup"><span data-stu-id="c6c71-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="c6c71-132">Voit asentaa Officen automaattisesti Windows-laitteisiin [ohjatun määritystoiminnon avulla.](set-up.md#deploy-office-365-client-apps)</span><span class="sxs-lookup"><span data-stu-id="c6c71-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="c6c71-133">Anna käyttäjien [asentaa Office-sovelluksia](/office365/admin/setup/install-applications) Windowsille ja laitteille.</span><span class="sxs-lookup"><span data-stu-id="c6c71-133">Let users [install Office apps](/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="c6c71-134">Tarkennettu</span><span class="sxs-lookup"><span data-stu-id="c6c71-134">Advanced</span></span>
- <span data-ttu-id="c6c71-135">**Uusien laitteiden määritäminen Autopilotilla**</span><span class="sxs-lookup"><span data-stu-id="c6c71-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="c6c71-136">Voit käyttää [Windows Autopilotia](add-autopilot-devices-and-profile.md) uusien **Windows** 10 -laitteiden automaattiseen esimääritykseen käyttäjälle, mutta voi olla helpompaa saada kumppani, joka voi tehdä tämän. [](https://www.microsoft.com/solution-providers/search)</span><span class="sxs-lookup"><span data-stu-id="c6c71-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="c6c71-137">Voit myös mennä [Microsoft Storeen](https://go.microsoft.com/fwlink/?linkid=874598)ja pyytää pilvitekniikan asiantuntijaa asettamaan ostamiesi uusien laitteiden ylle.</span><span class="sxs-lookup"><span data-stu-id="c6c71-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="c6c71-138">**Käytä paikallisia resursseja**</span><span class="sxs-lookup"><span data-stu-id="c6c71-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="c6c71-139">Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Business Premiumin suojaamaan Windows 10 -laitteitasi säilyttäen edelleen paikallisen todentamisen edellyttävän paikallisen todentamisen resurssien käyttöoikeuden.</span><span class="sxs-lookup"><span data-stu-id="c6c71-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="c6c71-140">Määritä tämä asetus noudattamalla ohjeita, jotka on annettu microsoft [365 Business Premiumin](manage-windows-devices.md) hallitsemaan toimialueisiin liitettyjen Windows 10 -laitteiden käyttöönotto.</span><span class="sxs-lookup"><span data-stu-id="c6c71-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="c6c71-141">Tämä on ensisijainen menetelmä, ja tässä tilassa laitteita kutsutaan Azure AD:n yhdistelmäympäristön laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="c6c71-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="c6c71-142">Jos yritykselläsi on paikallinen Active Directory, joka sisältää paikallisia resursseja (kuten jaetut tiedostot ja tulostimet), voit antaa Azure AD:lle liitettyjen laitteiden käyttöoikeudet näihin resursseihin seuraavasti: Käytä paikallisia resursseja Azure AD:llä yhdistetystä laitteesta [Microsoft 365 Business Premiumissa.](access-resources.md)</span><span class="sxs-lookup"><span data-stu-id="c6c71-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="c6c71-143">Tutustu myös seuraaviin ohjeartikkeleihin:</span><span class="sxs-lookup"><span data-stu-id="c6c71-143">See also</span></span>

[<span data-ttu-id="c6c71-144">Microsoft 365 for Business -koulutusvideot</span><span class="sxs-lookup"><span data-stu-id="c6c71-144">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)