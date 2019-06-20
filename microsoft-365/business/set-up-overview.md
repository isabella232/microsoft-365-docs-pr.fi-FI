---
title: Määritä yleiskatsaus
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Yleistä Microsoft 365 Business vaiheiden määrittäminen.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086312"
---
# <a name="overview-of-setup"></a><span data-ttu-id="09c0f-103">Asennuksen yleiskuvaus</span><span class="sxs-lookup"><span data-stu-id="09c0f-103">Overview of setup</span></span>

<span data-ttu-id="09c0f-104">Ohjattu asennus voidaan tehdä suurimman osan vaiheiden määrittäminen, mutta luetellaan myös muita vaihtoehtoja.</span><span class="sxs-lookup"><span data-stu-id="09c0f-104">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>


## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="09c0f-105">Vaihe 1: Lisää toimialue ja käyttäjät</span><span class="sxs-lookup"><span data-stu-id="09c0f-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="09c0f-106">**[Toimialueen lisääminen](set-up.md#add-your-domain-to-personalize-sign-in)** (Jos olet ostanut toimialueen aikana [rekisteröityä](sign-up.md), tässä vaiheessa on jo tehty.)</span><span class="sxs-lookup"><span data-stu-id="09c0f-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="09c0f-107">**Lisää käyttäjät**.</span><span class="sxs-lookup"><span data-stu-id="09c0f-107">**Add users**.</span></span> <span data-ttu-id="09c0f-108">Voit tehdä tämän jossakin seuraavista kolmesta tavasta:</span><span class="sxs-lookup"><span data-stu-id="09c0f-108">You can do this in any of the three ways:</span></span>
        - <span data-ttu-id="09c0f-109">[Ohjattu toiminto](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="09c0f-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="09c0f-110">Käyttää hakemiston synkronointi [Azure AD-yhteyden avulla käyttäjät](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) lisätään paikalliseen Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="09c0f-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="09c0f-111">Voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) admin Centerissä.</span><span class="sxs-lookup"><span data-stu-id="09c0f-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="09c0f-112">Vaihe 2: Määritä suojauskäytännöt ja määrittää laitteiden asetuksia</span><span class="sxs-lookup"><span data-stu-id="09c0f-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="09c0f-113">[Ohjatun asennuksen](set-up.md#set-up-security-policies-and-device-configurations) avulla voit määrittää laitteen ja suojauskäytännöt.</span><span class="sxs-lookup"><span data-stu-id="09c0f-113">Use the [Setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure device and security policies.</span></span> 
  - <span data-ttu-id="09c0f-114">Voit lisätä tai muokata niitä myöhemmin [hallintakeskukseen](view-policies-and-devices.md) ja [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="09c0f-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="09c0f-115">Lisäksi suojausasetukset ohjatun asennuksen voit suurentaa tietoturvan lisäämällä seuraavat asetukset:</span><span class="sxs-lookup"><span data-stu-id="09c0f-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="09c0f-116">**Sähköposti Suojaus haittaohjelmilta**</span><span class="sxs-lookup"><span data-stu-id="09c0f-116">**Email malware protection**</span></span>
      - <span data-ttu-id="09c0f-117">**Kokeneet Threat Protection (ATP) turvallinen linkit**</span><span class="sxs-lookup"><span data-stu-id="09c0f-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="09c0f-118">**ATP-Safe-liitteet**</span><span class="sxs-lookup"><span data-stu-id="09c0f-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="09c0f-119">**ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="09c0f-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="09c0f-120">**Exchange Online Archiving**</span><span class="sxs-lookup"><span data-stu-id="09c0f-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="09c0f-121">**Tietojen menetyksen estäminen (DLP)**</span><span class="sxs-lookup"><span data-stu-id="09c0f-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="09c0f-122">**Azure tietojen suojaus (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="09c0f-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="09c0f-123">Aloita ks- [käytäntöjen suojauksen lisäasetusten määrittäminen](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="09c0f-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="09c0f-124">Katso myös suojauksen parhaiden käytäntöjen opas [top 10 tapoja suojata yrityksen Microsoft 365](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) .</span><span class="sxs-lookup"><span data-stu-id="09c0f-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="09c0f-125">Vaihe 3: Määritä ja Hallitse Windows 10-laitteet</span><span class="sxs-lookup"><span data-stu-id="09c0f-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="09c0f-126">Kun liität laitteen Windows 10 Azure AD, [Vaihe 2](#step-2-set-up-security-policies-and-configure-devices) Määritä käytäntöjä saada käyttöön sitä.</span><span class="sxs-lookup"><span data-stu-id="09c0f-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="09c0f-127">Windows 10 Pro on [ennen sähköntoimitustarjoukset, joihin sisältyivät](pre-requisites-for-data-protection.md) Microsoft 365 Business, mutta jos sinulla on Windows 7 Pro, Windows 8 Pro tai Pro Windows 8.1, tilauksesi oikeuttaa asiakkaan [päivitettävä Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="09c0f-127">Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="09c0f-128">Käytännöt Windows 10-laitteiden [ohjatun asennustoiminnon](set-up.md#set-up-security-policies-and-device-configurations) avulla.</span><span class="sxs-lookup"><span data-stu-id="09c0f-128">Use the [setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure policies for Windows 10 devices.</span></span>

## <a name="stes-4-install-office-365-business"></a><span data-ttu-id="09c0f-129">Stes 4: Asenna Office 365: n liiketoiminnan</span><span class="sxs-lookup"><span data-stu-id="09c0f-129">Stes 4: Install Office 365 Business</span></span>
- <span data-ttu-id="09c0f-130">Voit asentaa Officen Windows-laitteet automaattisesti [ohjatun asennustoiminnon](set-up.md#deploy-office-365-client-apps)avulla.</span><span class="sxs-lookup"><span data-stu-id="09c0f-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="09c0f-131">Automaattisesti [asentaa Officen](auto-install-or-uninstall-office.md) hallintakeskukseen.</span><span class="sxs-lookup"><span data-stu-id="09c0f-131">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
- <span data-ttu-id="09c0f-132">Antaa käyttäjien [asentaa Office-sovellukset](https://docs.microsoft.com/office365/admin/setup/install-applications) ja laitteet.</span><span class="sxs-lookup"><span data-stu-id="09c0f-132">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="09c0f-133">Lisäasetukset</span><span class="sxs-lookup"><span data-stu-id="09c0f-133">Advanced</span></span>
- <span data-ttu-id="09c0f-134">**Automaattiohjauksen avulla voit määrittää uusia laitteita**</span><span class="sxs-lookup"><span data-stu-id="09c0f-134">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="09c0f-135">[Windows automaattiohjauksen](add-autopilot-devices-and-profile.md) avulla voit määrittää käyttäjän **Uusi** Windows 10-laitteet automaattisesti ennalta, mutta voi olla helpompi saada [kumppani](https://www.microsoft.com/solution-providers/search) , jolla voit tehdä tämän sinulle.</span><span class="sxs-lookup"><span data-stu-id="09c0f-135">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="09c0f-136">Voit myös siirtyä [Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) ja pyytää asiantuntija pilvi tekniikka määrittää, ostaa uusia laitteita.</span><span class="sxs-lookup"><span data-stu-id="09c0f-136">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

- <span data-ttu-id="09c0f-137">**Käyttää tiloissa resursseja**</span><span class="sxs-lookup"><span data-stu-id="09c0f-137">**Access on-premises resources**</span></span>

     - <span data-ttu-id="09c0f-138">Jos organisaatiossa käytetään Windows Server Active Directory tiloissa, voit määrittää Microsoft 365 liiketoiminnan suojaamaan Windows 10-laitteet, säilyttäen kuitenkin edellyttää paikallista todennusta tiloissa resurssien käytön.</span><span class="sxs-lookup"><span data-stu-id="09c0f-138">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="09c0f-139">Voit määrittää [toimialueeseen liittymistä Windows 10 laitteita voi hallita Microsoft 365 Business käyttöön](manage-windows-devices.md) noudattamalla.</span><span class="sxs-lookup"><span data-stu-id="09c0f-139">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="09c0f-140">Tämä on ensisijainen menetelmä, ja tässä tilassa laitteita kutsutaan hybridi Azure AD liitetyt laitteet.</span><span class="sxs-lookup"><span data-stu-id="09c0f-140">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="09c0f-141">Jos yrityksesi on paikallista Active Directory, joka sisältää joitakin tiloissa (kuten jaettujen tiedostoresurssien ja tulostinten), voit antaa Azure AD liittynyt laitteiden käyttöä noudattamalla tässä nämä resurssit: [käyttö paikalliset resurssit Microsoft 365 Business AD liitetty laite Azure](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="09c0f-141">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  