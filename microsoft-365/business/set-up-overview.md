---
title: Yleiskatsaus määrittämisestä
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Yleiskatsaus Microsoft 365 Businessin asetus vaiheista.
ms.openlocfilehash: 4be0a8aa1b050ee3e20a045eb2c07666765118ed
ms.sourcegitcommit: cbf117a4cd92a907115c9f10752f3c557361e586
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/10/2019
ms.locfileid: "37440533"
---
# <a name="overview-of-setup"></a><span data-ttu-id="b7454-103">Yleiskatsaus asennuksesta</span><span class="sxs-lookup"><span data-stu-id="b7454-103">Overview of setup</span></span>

<span data-ttu-id="b7454-104">Suurin osa määritys vaiheista voidaan tehdä ohjatussa asennus toiminnossa, mutta muut vaihto ehdot luetellaan myös.</span><span class="sxs-lookup"><span data-stu-id="b7454-104">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>


## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="b7454-105">Vaihe 1: Lisää verkko tunnuksesi ja käyttäjät</span><span class="sxs-lookup"><span data-stu-id="b7454-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="b7454-106">**[Lisää verkko tunnuksesi](set-up.md#add-your-domain-to-personalize-sign-in)** (jos ostit verkko tunnuksesi [rekisteröitymistä](sign-up.md)varten, tämä vaihe on jo tehty.)</span><span class="sxs-lookup"><span data-stu-id="b7454-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="b7454-107">**Lisää käyttäjiä**.</span><span class="sxs-lookup"><span data-stu-id="b7454-107">**Add users**.</span></span> <span data-ttu-id="b7454-108">Voit tehdä tämän jollakin kolmella tavalla:</span><span class="sxs-lookup"><span data-stu-id="b7454-108">You can do this in any of the three ways:</span></span>
        - <span data-ttu-id="b7454-109">[Ohjatussa toiminnossa](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="b7454-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="b7454-110">Käytä hakemiston synkronointia [lisätäksesi käyttäjiä Azure AD Connectin avulla](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) , jos sinulla on paikallinen Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b7454-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="b7454-111">Voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallinta keskukseen.</span><span class="sxs-lookup"><span data-stu-id="b7454-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="b7454-112">Vaihe 2: suojaus käytäntöjen määrittäminen ja laitteiden määrittäminen</span><span class="sxs-lookup"><span data-stu-id="b7454-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="b7454-113">Määritä laite-ja suojaus käytännöt [ohjatun asennus toiminnon](set-up.md#protect-data-and-devices) avulla.</span><span class="sxs-lookup"><span data-stu-id="b7454-113">Use the [Setup wizard](set-up.md#protect-data-and-devices) to configure device and security policies.</span></span> 
  - <span data-ttu-id="b7454-114">Voit myös lisätä tai muokata niitä myöhemmin [hallinta keskuksessa](view-policies-and-devices.md) ja [Intune-portaalissa](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="b7454-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="b7454-115">Ohjatun asennus toiminnon suojaus asetusten lisäksi voit lisätä suojausta lisäämällä seuraavat asetukset:</span><span class="sxs-lookup"><span data-stu-id="b7454-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="b7454-116">**Sähkö postin haitta ohjelmien torjunta**</span><span class="sxs-lookup"><span data-stu-id="b7454-116">**Email malware protection**</span></span>
      - <span data-ttu-id="b7454-117">**Kehittyneet uhkien torjunta (ATP) turvalliset linkit**</span><span class="sxs-lookup"><span data-stu-id="b7454-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="b7454-118">**ATP turvalliset liitteet**</span><span class="sxs-lookup"><span data-stu-id="b7454-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="b7454-119">**ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="b7454-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="b7454-120">**Exchange Online Archiving**</span><span class="sxs-lookup"><span data-stu-id="b7454-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="b7454-121">**Tietojen menetyksen estäminen (DLP)**</span><span class="sxs-lookup"><span data-stu-id="b7454-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="b7454-122">**Azure-tietojen suojaus (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="b7454-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="b7454-123">Jos haluat aloittaa, Katso, [Määritä suoja uksen lisä käytännöt](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="b7454-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="b7454-124">Katso myös [Top 10-tapoja suojata Microsoft 365-liike toiminnan](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) etenemis suunnitelma parhaista tieto turva käytännöistä.</span><span class="sxs-lookup"><span data-stu-id="b7454-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="b7454-125">Vaihe 3: Windows 10-laitteiden määrittäminen ja hallinta</span><span class="sxs-lookup"><span data-stu-id="b7454-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="b7454-126">Kun liityt Windows 10-laitteeseen Azure ADIIN, [vaiheessa 2](#step-2-set-up-security-policies-and-configure-devices) käyttöön asettamat käytännöt kohdistetaan siihen.</span><span class="sxs-lookup"><span data-stu-id="b7454-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="b7454-127">Windows 10 Pro on Microsoft 365 [Businessin edellytys](pre-requisites-for-data-protection.md) , mutta jos sinulla on Windows 7 Pro, Windows 8 Pro tai Windows 8,1 Pro, tilauksesi oikeuttaa sinut [päivittämään Windows 10 Pro-versioon](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="b7454-127">Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="b7454-128">Määritä Windows 10-laitteiden käytännöt [ohjatun asennus toiminnon](set-up.md#protect-data-and-devices) avulla.</span><span class="sxs-lookup"><span data-stu-id="b7454-128">Use the [Setup wizard](set-up.md#protect-data-and-devices) to configure policies for Windows 10 devices.</span></span>

## <a name="stes-4-install-office-365-business"></a><span data-ttu-id="b7454-129">STES 4: Asenna Office 365 Business</span><span class="sxs-lookup"><span data-stu-id="b7454-129">Stes 4: Install Office 365 Business</span></span>
- <span data-ttu-id="b7454-130">Voit asentaa Officen automaattisesti Windows-laitteisiin [ohjatun asennus toiminnon](set-up.md#deploy-office-365-client-apps)avulla.</span><span class="sxs-lookup"><span data-stu-id="b7454-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="b7454-131">[Asenna Office](auto-install-or-uninstall-office.md) automaattisesti hallinta keskuksesta.</span><span class="sxs-lookup"><span data-stu-id="b7454-131">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
- <span data-ttu-id="b7454-132">Anna käyttäjien [asentaa Office-sovelluksia](https://docs.microsoft.com/office365/admin/setup/install-applications) Windowsille ja laitteille.</span><span class="sxs-lookup"><span data-stu-id="b7454-132">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="b7454-133">Kehittynyt</span><span class="sxs-lookup"><span data-stu-id="b7454-133">Advanced</span></span>
- <span data-ttu-id="b7454-134">**Uusien laitteiden määrittäminen automaatti ohjauksen avulla**</span><span class="sxs-lookup"><span data-stu-id="b7454-134">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="b7454-135">[Windows auto pilotin](add-autopilot-devices-and-profile.md) avulla voit määrittää käyttäjälle automaattisesti **uusia** Windows 10-laitteita, mutta [kumppanin](https://www.microsoft.com/solution-providers/search) , joka voi tehdä tämän puolestasi, on ehkä helpompi hankkia se.</span><span class="sxs-lookup"><span data-stu-id="b7454-135">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="b7454-136">Voit myös siirtyä [Microsoft Storeen](https://go.microsoft.com/fwlink/?linkid=874598) ja pyytää pilvi teknologian asiantuntijaa hankkimaan sinulle uusia laitteita.</span><span class="sxs-lookup"><span data-stu-id="b7454-136">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

- <span data-ttu-id="b7454-137">**Paikallisten resurssien käyttö**</span><span class="sxs-lookup"><span data-stu-id="b7454-137">**Access on-premises resources**</span></span>

     - <span data-ttu-id="b7454-138">Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Businessin suojaamaan Windows 10-laitteitasi samalla, kun ylläpidämme paikallisen todennuksen edellyttävien paikallisten resurssien käyttö oikeuksia.</span><span class="sxs-lookup"><span data-stu-id="b7454-138">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="b7454-139">Määritä Microsoft 365 Business, jotta voit määrittää tämän noudattamalla [toimi alueeseen liittyneiden Windows 10-laitteiden käyttöönotto](manage-windows-devices.md) ohjeita.</span><span class="sxs-lookup"><span data-stu-id="b7454-139">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="b7454-140">Tämä on ensisijainen menetelmä ja laitteet tässä tilassa kutsutaan hybridi Azure AD liitetyt laitteet.</span><span class="sxs-lookup"><span data-stu-id="b7454-140">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="b7454-141">Jos yrityksessasi on paikallinen Active Directory, joka sisältää joitakin paikallisia resursseja (kuten tiedosto resursseja ja tulostimia), voit antaa Azure AD-liitettyjen laitteiden käyttää näitä resursseja noudattamalla seuraavia ohjeita: [paikallisten resurssien käyttö Azure AD-liitetty laite Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="b7454-141">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  