---
title: Toimialueen käyttöön liitettyjen Windows 10 -laitteiden hallinta Microsoft 365 for Businessissa
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Lue, miten voit ottaa Microsoft 365:n käyttöön paikallisten Active Directoryyn liitettyjen Windows 10 -laitteiden suojaamisessa muutamassa vaiheessa.
ms.openlocfilehash: 6275c6c4be9cd9631ab095f8b0e1b39683022bb2
ms.sourcegitcommit: d988faa292c2661ffea43c7161aef92b2b4b99bc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/04/2020
ms.locfileid: "46560839"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="6082b-103">Toimialueen käyttöön liitettyjen Windows 10 -laitteiden hallinta Microsoft 365 Business Premiumilla</span><span class="sxs-lookup"><span data-stu-id="6082b-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="6082b-104">Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Business Premiumin suojaamaan Windows 10 -laitteita säilyttäen samalla paikallisen todennuksen edellyttävien paikallisten resurssien käytön.</span><span class="sxs-lookup"><span data-stu-id="6082b-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="6082b-105">Voit määrittää tämän suojauksen mukautuksella **Hybrid Azure AD -liitettyjä laitteita**.</span><span class="sxs-lookup"><span data-stu-id="6082b-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="6082b-106">Nämä laitteet on liitetty sekä paikalliseen Active Directoryyn että Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="6082b-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="6082b-107">Tässä videossa kuvataan, miten tämä määritetään yleisin skenaario, joka on myös kuvattu vaiheet, joita seurataan.</span><span class="sxs-lookup"><span data-stu-id="6082b-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="6082b-108">Ennen kuin aloitat, varmista, että olet suorittanut seuraavat toimet:</span><span class="sxs-lookup"><span data-stu-id="6082b-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="6082b-109">Synkronoi käyttäjät Azure AD:hen Azure AD Connectin avulla.</span><span class="sxs-lookup"><span data-stu-id="6082b-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="6082b-110">Suorita Azure AD Connect Organizational Unit (OU) -synkronointi loppuun.</span><span class="sxs-lookup"><span data-stu-id="6082b-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="6082b-111">Varmista, että kaikilla synkronoiduilla toimialueen käyttäjillä on käyttöoikeudet Microsoft 365 Business Premiumiin.</span><span class="sxs-lookup"><span data-stu-id="6082b-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="6082b-112">Vaiheet ovat [ohjeaiheessa Toimialueen käyttäjien synkronoiminen Microsoftiin.](manage-domain-users.md)</span><span class="sxs-lookup"><span data-stu-id="6082b-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="6082b-113">1. Tarkista MDM-viranomainen Intuessa</span><span class="sxs-lookup"><span data-stu-id="6082b-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="6082b-114">Siirry [Endpoint Manageriin](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) ja valitse Microsoft Intune -sivulla **Laiterekisteröinti**ja varmista **sitten Yleiskatsaus-sivulla,** että **MDM-viranomainen** on **Intune**.</span><span class="sxs-lookup"><span data-stu-id="6082b-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="6082b-115">Jos **MDM-viranomainen** **ei ole Ei mitään**, määritä **MDM-myöntäjäksi** **Intune**.</span><span class="sxs-lookup"><span data-stu-id="6082b-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="6082b-116">Jos **MDM-myöntäjä** on **Microsoft Office 365**, siirry **Devices**  >  **Laitteet-rekisteröintilaitteisiin** ja lisää **Intune MDM** -myöntäjä lisää **MDM-myöntäjän lisääminen** -valintaikkunassa **(Lisää MDM-myöntäjä** -valintaikkuna on käytettävissä vain, jos **MDM-myöntäjäksi** on määritetty Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="6082b-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="6082b-117">2. Varmista, että Azure AD on otettu käyttöön tietokoneiden liittämistä varten</span><span class="sxs-lookup"><span data-stu-id="6082b-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="6082b-118">Siirry hallintakeskukseen kohdassa <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ja valitse **Hallintakeskukset-luettelosta Azure Active Directory** (valitse Näytä kaikki, jos Azure Active Directory ei ole näkyvissä). **Admin centers**</span><span class="sxs-lookup"><span data-stu-id="6082b-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="6082b-119">Siirry **Azure Active Directory -hallintakeskuksessa** **Azure Active Directoryyn** , valitse **Laitteet** ja sitten **Laiteasetukset**.</span><span class="sxs-lookup"><span data-stu-id="6082b-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="6082b-120">Tarkista, että**käyttäjät voivat liittyä laitteisiin Azure AD:ssä** on käytössä</span><span class="sxs-lookup"><span data-stu-id="6082b-120">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="6082b-121">Jos haluat ottaa kaikki käyttäjät käyttöön, määritä **Kaikki**.</span><span class="sxs-lookup"><span data-stu-id="6082b-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="6082b-122">Jos haluat ottaa tietyt käyttäjät käyttöön, ota tietty käyttäjäryhmä käyttöön määrittämällä **Valittu.**</span><span class="sxs-lookup"><span data-stu-id="6082b-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="6082b-123">Lisää Azure AD:ssä synkronoidut toimialueen käyttäjät [suojausryhmään](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="6082b-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="6082b-124">Ota MDM-käyttäjäalue käyttöön kyseisessä suojausryhmässä valitsemalla **Valitse ryhmät.**</span><span class="sxs-lookup"><span data-stu-id="6082b-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="6082b-125">3. Varmista, että Azure AD on otettu käyttöön MDM:ssä</span><span class="sxs-lookup"><span data-stu-id="6082b-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="6082b-126">Siirry hallintakeskukseen ja <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> valitse **päätepisteen hallinta**t (valitse Näytä **kaikki,** jos **Päätepisteen hallinta** ei ole näkyvissä)</span><span class="sxs-lookup"><span data-stu-id="6082b-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="6082b-127">Siirry **Microsoft Endpoint Manager -hallintakeskuksessa** **kohtaan Laitteet**  >  **Windows**  >  **Windowsin rekisteröityminen**  >  **automaattisesti**.</span><span class="sxs-lookup"><span data-stu-id="6082b-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="6082b-128">Varmista, että MDM-käyttäjän vaikutusalue on käytössä.</span><span class="sxs-lookup"><span data-stu-id="6082b-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="6082b-129">Jos haluat rekisteröidä kaikki tietokoneet, määritä **Kaikki** rekisteröimään automaattisesti kaikki käyttäjätietokoneet, jotka on liitetty Azure AD:hen ja uusiin tietokoneisiin, kun käyttäjät lisäävät työtilin Windowsiin.</span><span class="sxs-lookup"><span data-stu-id="6082b-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="6082b-130">Määritä **Joidenkin-asetukseksi,** jos haluat rekisteröidä tietyn käyttäjäryhmän tietokoneet.</span><span class="sxs-lookup"><span data-stu-id="6082b-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="6082b-131">Lisää Azure AD:ssä synkronoidut toimialueen käyttäjät [suojausryhmään](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="6082b-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="6082b-132">Ota MDM-käyttäjäalue käyttöön kyseisessä suojausryhmässä valitsemalla **Valitse ryhmät.**</span><span class="sxs-lookup"><span data-stu-id="6082b-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="6082b-133">4. Tarvittavien resurssien luominen</span><span class="sxs-lookup"><span data-stu-id="6082b-133">4. Create the required resources</span></span> 

<span data-ttu-id="6082b-134">Tarvittavien tehtävien suorittamista [Azure AD -yhdistelmän määrittämiseksi](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) on yksinkertaistettu [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) [PowerShell-moduulissa olevan Initialize-SecMgmtHybirdDeviceEnrollment-cmdlet-otoksen](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) avulla.</span><span class="sxs-lookup"><span data-stu-id="6082b-134">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="6082b-135">Kun käynnistät tämän cmdlet-liitännän, se luo ja määrittää tarvittavan palveluyhteyspisteen ja ryhmäkäytännön.</span><span class="sxs-lookup"><span data-stu-id="6082b-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="6082b-136">Voit asentaa tämän moduulin vetoamalla PowerShellin esiintymään seuraaviin nätin:</span><span class="sxs-lookup"><span data-stu-id="6082b-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="6082b-137">On suositeltavaa asentaa tämä moduuli Windows Serveriin, jossa on Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="6082b-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="6082b-138">Voit luoda tarvittavan palveluyhteyspisteen ja ryhmäkäytännön käynnistämalla [Initialize-SecMgmtHybirdDeviceEnrollment-cmdlet-liitännän.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="6082b-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="6082b-139">Tarvitset Microsoft 365 Business Premiumin yleiset järjestelmänvalvojan tunnistetiedot tätä tehtävää suoritettaessa.</span><span class="sxs-lookup"><span data-stu-id="6082b-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="6082b-140">Kun olet valmis luomaan resurssit, käynnistä seuraavat toimet:</span><span class="sxs-lookup"><span data-stu-id="6082b-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="6082b-141">Ensimmäinen komento muodostaa yhteyden Microsoftin pilveen, ja kun sinua kehotetaan, määritä Microsoft 365 Business Premiumin yleiset järjestelmänvalvojan tunnistetiedot.</span><span class="sxs-lookup"><span data-stu-id="6082b-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="6082b-142">5. Linkitä ryhmäkäytäntö</span><span class="sxs-lookup"><span data-stu-id="6082b-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="6082b-143">Napsauta ryhmäkäytäntöjen hallintakonsolissa (GPMC) hiiren kakkospainikkeella sijaintia, johon haluat linkittää käytännön, ja valitse pikavalikosta *Linkitä aiemmin luotu ryhmäkäytäntöobjekti...*</span><span class="sxs-lookup"><span data-stu-id="6082b-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="6082b-144">Valitse yllä olevassa vaiheessa luotu käytäntö ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="6082b-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="6082b-145">Hanki uusimmat hallintamallit</span><span class="sxs-lookup"><span data-stu-id="6082b-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="6082b-146">Jos käytäntö **Ota automaattinen MDM-rekisteröinti käyttöön Azure AD -oletustunnistetietojen avulla**ei ole näkyvissä , syy siihen, että ADMX:ää ei ole asennettu Windows 10:lle, versiolle 1803, versiolle 1809 tai versiolle 1903.</span><span class="sxs-lookup"><span data-stu-id="6082b-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="6082b-147">Voit korjata ongelman seuraavasti (Huomautus: uusin MDM.admx on taaksepäin yhteensopiva):</span><span class="sxs-lookup"><span data-stu-id="6082b-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="6082b-148">Download: [Windows 10:n toukokuun 2019 päivitys (1903) hallintamallit (.admx).](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all)</span><span class="sxs-lookup"><span data-stu-id="6082b-148">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="6082b-149">Asenna paketti ensisijaiseen toimialueen ohjauskoneeseen (PDC).</span><span class="sxs-lookup"><span data-stu-id="6082b-149">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="6082b-150">Siirry kansion version mukaan: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="6082b-150">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="6082b-151">Nimeä **käytäntömääritykset** -kansio uudelleen edellä mainitussa **PolicyDefinitions-polun polussa.**</span><span class="sxs-lookup"><span data-stu-id="6082b-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="6082b-152">Kopioi **PolicyDefinitions-kansio** **kansioon C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="6082b-152">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="6082b-153">Jos aiot käyttää koko toimialueen keskitettyä käytäntösäilöä, lisää siihen PolicyDefinitions-sisältö.</span><span class="sxs-lookup"><span data-stu-id="6082b-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="6082b-154">Käynnistä ensisijainen toimialueen ohjauskone uudelleen, jotta käytäntö on käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="6082b-154">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="6082b-155">Tämä menettely toimii kaikissa tulevissa versioissa samoin.</span><span class="sxs-lookup"><span data-stu-id="6082b-155">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="6082b-156">Tässä vaiheessa sinun pitäisi pystyä näkemään käytäntö **Ota automaattinen MDM-rekisteröinti käyttöön käyttämällä Azure AD:n oletustunnistetietoja.**</span><span class="sxs-lookup"><span data-stu-id="6082b-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>
