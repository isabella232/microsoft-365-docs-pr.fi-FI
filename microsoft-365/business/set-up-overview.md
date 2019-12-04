---
title: Yleiskatsaus asennuksesta
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Yleiskatsaus Microsoft 365 Businessin asennus vaiheista.
ms.openlocfilehash: 425c465262c266ca764ae8c7a52130903fa635a5
ms.sourcegitcommit: 8fda7852b2a5baa92b8a365865b014ea6d100bbc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/03/2019
ms.locfileid: "39812774"
---
# <a name="overview-of-setup"></a><span data-ttu-id="daeb3-103">Yleiskatsaus asennuksesta</span><span class="sxs-lookup"><span data-stu-id="daeb3-103">Overview of setup</span></span>

<span data-ttu-id="daeb3-104">Suurin osa asennus vaiheista voidaan tehdä ohjatussa asennus toiminnossa, mutta muut vaihto ehdot luetellaan myös.</span><span class="sxs-lookup"><span data-stu-id="daeb3-104">Most of the setup steps can be done in the setup wizard, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="daeb3-105">Vaihe 1: Lisää verkko tunnuksesi ja käyttäjät</span><span class="sxs-lookup"><span data-stu-id="daeb3-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="daeb3-106">**[Lisää verkko tunnuksesi](set-up.md#add-your-domain-to-personalize-sign-in)** (jos ostit verkko tunnuksesi [rekisteröitymistä](sign-up.md)varten, tämä vaihe on jo tehty.)</span><span class="sxs-lookup"><span data-stu-id="daeb3-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="daeb3-107">**Lisää käyttäjiä**.</span><span class="sxs-lookup"><span data-stu-id="daeb3-107">**Add users**.</span></span> <span data-ttu-id="daeb3-108">Voit lisätä käyttäjiä seuraavilla kolmella tavalla:</span><span class="sxs-lookup"><span data-stu-id="daeb3-108">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="daeb3-109">[Ohjatussa toiminnossa](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="daeb3-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="daeb3-110">Käytä hakemiston synkronointia [lisätäksesi käyttäjiä Azure AD Connectin avulla](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) , jos sinulla on paikallinen Active Directory.</span><span class="sxs-lookup"><span data-stu-id="daeb3-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="daeb3-111">Voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallinta keskukseen.</span><span class="sxs-lookup"><span data-stu-id="daeb3-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="daeb3-112">Vaihe 2: suojaus käytäntöjen määrittäminen ja laitteiden määrittäminen</span><span class="sxs-lookup"><span data-stu-id="daeb3-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="daeb3-113">Määritä laite käytännöt [ohjatun asennus toiminnon](set-up.md#protect-your-organization) avulla.</span><span class="sxs-lookup"><span data-stu-id="daeb3-113">Use the [Setup wizard](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="daeb3-114">Voit myös lisätä tai muokata niitä myöhemmin [hallinta keskuksessa](view-policies-and-devices.md) ja [Intune-portaalissa](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="daeb3-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="daeb3-115">Ohjattu asennus toiminto määrittää myös perusuhkien torjunnan ja tietojen menetyksen eston asetukset.</span><span class="sxs-lookup"><span data-stu-id="daeb3-115">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="daeb3-116">Ohjatun asennus toiminnon suojaus asetusten lisäksi voit lisätä suojausta lisäämällä seuraavat asetukset:</span><span class="sxs-lookup"><span data-stu-id="daeb3-116">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="daeb3-117">**Sähkö postin haitta ohjelmien torjunta**</span><span class="sxs-lookup"><span data-stu-id="daeb3-117">**Email malware protection**</span></span>
      - <span data-ttu-id="daeb3-118">**ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="daeb3-118">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="daeb3-119">**Exchange Online Archiving**</span><span class="sxs-lookup"><span data-stu-id="daeb3-119">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="daeb3-120">**Azure-tietojen suojaus (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="daeb3-120">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="daeb3-121">Jos haluat aloittaa, Katso, [Määritä suoja uksen lisä käytännöt](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="daeb3-121">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="daeb3-122">Katso myös [Top 10-tapoja suojata Microsoft 365-liike toiminnan](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) etenemis suunnitelma parhaista tieto turva käytännöistä.</span><span class="sxs-lookup"><span data-stu-id="daeb3-122">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="daeb3-123">Vaihe 3: Windows 10-laitteiden määrittäminen ja hallinta</span><span class="sxs-lookup"><span data-stu-id="daeb3-123">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="daeb3-124">Kun olet suorittanut ohjatun asennus toiminnon, sinun on suoritettava kaikki organisaatiosi Windwos 10-tieto koneet.</span><span class="sxs-lookup"><span data-stu-id="daeb3-124">After you run the set up wizard, you will want to proctect all the Windwos 10 computers in your organization.</span></span>
  
- <span data-ttu-id="daeb3-125">Windows 10 Pro on [edellytys](pre-requisites-for-data-protection.md) Microsoft 365 Business, mutta jos sinulla on Windows 7 Pro, Windows 8 Pro, tai Windows 8,1 Pro, tilauksesi oikeuttaa [päivityksen Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="daeb3-125">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
- <span data-ttu-id="daeb3-126">Määritä Windows 10-laitteiden käytännöt noudattamalla [suojattujen Windows 10-tieto koneiden](secure-win-10-pcs.md) ohjeita.</span><span class="sxs-lookup"><span data-stu-id="daeb3-126">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="daeb3-127">Kun liityt Windows 10-laitteeseen Azure ADIIN, Windows 10-tieto koneille asetetut käytännöt kohdistetaan siihen.</span><span class="sxs-lookup"><span data-stu-id="daeb3-127">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="daeb3-128">Lisä tietoja on kohdassa [Windows-laitteiden määrittäminen Microsoft 365-yritys käyttäjille](set-up-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="daeb3-128">For more information, see [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-office-365-business"></a><span data-ttu-id="daeb3-129">Vaihe 4: Asenna Office 365 Business</span><span class="sxs-lookup"><span data-stu-id="daeb3-129">Step 4: Install Office 365 Business</span></span>
- <span data-ttu-id="daeb3-130">Voit asentaa Officen automaattisesti Windows-laitteisiin [ohjatun asennus toiminnon](set-up.md#deploy-office-365-client-apps)avulla.</span><span class="sxs-lookup"><span data-stu-id="daeb3-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="daeb3-131">Anna käyttäjien [asentaa Office-sovelluksia](https://docs.microsoft.com/office365/admin/setup/install-applications) Windowsille ja laitteille.</span><span class="sxs-lookup"><span data-stu-id="daeb3-131">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="daeb3-132">Kehittynyt</span><span class="sxs-lookup"><span data-stu-id="daeb3-132">Advanced</span></span>
- <span data-ttu-id="daeb3-133">**Uusien laitteiden määrittäminen automaatti ohjauksen avulla**</span><span class="sxs-lookup"><span data-stu-id="daeb3-133">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="daeb3-134">[Windows auto pilotin](add-autopilot-devices-and-profile.md) avulla voit määrittää käyttäjälle automaattisesti **uusia** Windows 10-laitteita, mutta [kumppanin](https://www.microsoft.com/solution-providers/search) , joka voi tehdä tämän puolestasi, on ehkä helpompi hankkia se.</span><span class="sxs-lookup"><span data-stu-id="daeb3-134">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="daeb3-135">Voit myös siirtyä [Microsoft Storeen](https://go.microsoft.com/fwlink/?linkid=874598)ja pyytää pilvi tekniikan asiantuntijaa ostamaan uusia laitteita.</span><span class="sxs-lookup"><span data-stu-id="daeb3-135">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="daeb3-136">**Paikallisten resurssien käyttö**</span><span class="sxs-lookup"><span data-stu-id="daeb3-136">**Access on-premises resources**</span></span>

     - <span data-ttu-id="daeb3-137">Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Businessin suojaamaan Windows 10-laitteitasi samalla, kun ylläpidämme paikallisen todennuksen edellyttävien paikallisten resurssien käyttö oikeuksia.</span><span class="sxs-lookup"><span data-stu-id="daeb3-137">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="daeb3-138">Määritä Microsoft 365 Business, jotta voit määrittää tämän noudattamalla [toimi alueeseen liittyneiden Windows 10-laitteiden käyttöönotto](manage-windows-devices.md) ohjeita.</span><span class="sxs-lookup"><span data-stu-id="daeb3-138">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="daeb3-139">Tämä on ensisijainen menetelmä, ja laitteet tässä tilassa kutsutaan hybridi Azure AD liitetyt laitteet.</span><span class="sxs-lookup"><span data-stu-id="daeb3-139">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="daeb3-140">Jos yrityksellasi on paikallinen Active Directory, joka sisältää joitakin paikallisia resursseja (kuten tiedosto resursseja ja tulostimia), voit antaa Azure AD-liitetyille laitteille näiden resurssien käyttö oikeudet noudattamalla seuraavia ohjeita: [paikallisten resurssien käyttö Azure AD-liitetystä laitteesta Microsoft 365-liike toiminnassa](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="daeb3-140">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="daeb3-141">Katso myös</span><span class="sxs-lookup"><span data-stu-id="daeb3-141">See also</span></span>

[<span data-ttu-id="daeb3-142">Microsoft 365-liike toiminnan koulutus videot</span><span class="sxs-lookup"><span data-stu-id="daeb3-142">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
