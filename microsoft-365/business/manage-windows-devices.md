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
ms.openlocfilehash: 2eaf5aa76cae1680b93af008af615ae872e4fb20
ms.sourcegitcommit: fab425ea4580d1924fb421e6db233d135f5b7d19
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/31/2020
ms.locfileid: "46533781"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="fdb81-103">Toimialueen käyttöön liitettyjen Windows 10 -laitteiden hallinta Microsoft 365 Business Premiumilla</span><span class="sxs-lookup"><span data-stu-id="fdb81-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="fdb81-104">Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Business Premiumin suojaamaan Windows 10 -laitteita säilyttäen samalla paikallisen todennuksen edellyttävien paikallisten resurssien käytön.</span><span class="sxs-lookup"><span data-stu-id="fdb81-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="fdb81-105">Voit määrittää tämän suojauksen mukautuksella **Hybrid Azure AD -liitettyjä laitteita**.</span><span class="sxs-lookup"><span data-stu-id="fdb81-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="fdb81-106">Nämä laitteet on liitetty sekä paikalliseen Active Directoryyn että Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="fdb81-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="fdb81-107">Tässä videossa kuvataan, miten tämä määritetään yleisin skenaario, joka on myös kuvattu vaiheet, joita seurataan.</span><span class="sxs-lookup"><span data-stu-id="fdb81-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="fdb81-108">Ennen kuin aloitat, varmista, että olet suorittanut seuraavat toimet:</span><span class="sxs-lookup"><span data-stu-id="fdb81-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="fdb81-109">Synkronoi käyttäjät Azure AD:hen Azure AD Connectin avulla.</span><span class="sxs-lookup"><span data-stu-id="fdb81-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="fdb81-110">Suorita Azure AD Connect Organizational Unit (OU) -synkronointi loppuun.</span><span class="sxs-lookup"><span data-stu-id="fdb81-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="fdb81-111">Varmista, että kaikilla synkronoiduilla toimialueen käyttäjillä on käyttöoikeudet Microsoft 365 Business Premiumiin.</span><span class="sxs-lookup"><span data-stu-id="fdb81-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="fdb81-112">Vaiheet ovat [ohjeaiheessa Toimialueen käyttäjien synkronoiminen Microsoftiin.](manage-domain-users.md)</span><span class="sxs-lookup"><span data-stu-id="fdb81-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="fdb81-113">1. Tarkista MDM-viranomainen Intuessa</span><span class="sxs-lookup"><span data-stu-id="fdb81-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="fdb81-114">Siirry portal.azure.com ja sivun yläreunassa etsi Intune.</span><span class="sxs-lookup"><span data-stu-id="fdb81-114">Go to portal.azure.com and on the top of the page search for Intune.</span></span>
<span data-ttu-id="fdb81-115">Valitse Microsoft Intune -sivulla **Laiterekisteröinti** ja varmista **Yleiskatsaus-sivulla,** että **MDM-myöntäjä** on **Intune**.</span><span class="sxs-lookup"><span data-stu-id="fdb81-115">On the Microsoft Intune page, select **Device enrollment** and on the **Overview** page make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="fdb81-116">Jos **MDM-viranomainen** **ei ole Ei mitään**, määritä **MDM-myöntäjäksi** **Intune**.</span><span class="sxs-lookup"><span data-stu-id="fdb81-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="fdb81-117">Jos **MDM-myöntäjä** on **Microsoft Office 365**, siirry **Devices**  >  **Laitteet-rekisteröintilaitteisiin** ja lisää **Intune MDM** -myöntäjä lisää **MDM-myöntäjän lisääminen** -valintaikkunassa **(Lisää MDM-myöntäjä** -valintaikkuna on käytettävissä vain, jos **MDM-myöntäjäksi** on määritetty Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="fdb81-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="fdb81-118">2. Varmista, että Azure AD on otettu käyttöön tietokoneiden liittämistä varten</span><span class="sxs-lookup"><span data-stu-id="fdb81-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="fdb81-119">Siirry hallintakeskukseen kohdassa <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ja valitse **Hallintakeskukset-luettelosta Azure Active Directory** (valitse Näytä kaikki, jos Azure Active Directory ei ole näkyvissä). **Admin centers**</span><span class="sxs-lookup"><span data-stu-id="fdb81-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="fdb81-120">Siirry **Azure Active Directory -hallintakeskuksessa** **Azure Active Directoryyn** , valitse **Laitteet** ja sitten **Laiteasetukset**.</span><span class="sxs-lookup"><span data-stu-id="fdb81-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="fdb81-121">Tarkista, että**käyttäjät voivat liittyä laitteisiin Azure AD:ssä** on käytössä</span><span class="sxs-lookup"><span data-stu-id="fdb81-121">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="fdb81-122">Jos haluat ottaa kaikki käyttäjät käyttöön, määritä **Kaikki**.</span><span class="sxs-lookup"><span data-stu-id="fdb81-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="fdb81-123">Jos haluat ottaa tietyt käyttäjät käyttöön, ota tietty käyttäjäryhmä käyttöön määrittämällä **Valittu.**</span><span class="sxs-lookup"><span data-stu-id="fdb81-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="fdb81-124">Lisää Azure AD:ssä synkronoidut toimialueen käyttäjät [suojausryhmään](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="fdb81-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="fdb81-125">Ota MDM-käyttäjäalue käyttöön kyseisessä suojausryhmässä valitsemalla **Valitse ryhmät.**</span><span class="sxs-lookup"><span data-stu-id="fdb81-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="fdb81-126">3. Varmista, että Azure AD on otettu käyttöön MDM:ssä</span><span class="sxs-lookup"><span data-stu-id="fdb81-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="fdb81-127">Siirry hallintakeskukseen ja <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> valitse **päätepisteen hallinta**t (valitse Näytä **kaikki,** jos **Päätepisteen hallinta** ei ole näkyvissä)</span><span class="sxs-lookup"><span data-stu-id="fdb81-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="fdb81-128">Siirry **Microsoft Endpoint Manager -hallintakeskuksessa** **kohtaan Laitteet**  >  **Windows**  >  **Windowsin rekisteröityminen**  >  **automaattisesti**.</span><span class="sxs-lookup"><span data-stu-id="fdb81-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="fdb81-129">Varmista, että MDM-käyttäjän vaikutusalue on käytössä.</span><span class="sxs-lookup"><span data-stu-id="fdb81-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="fdb81-130">Jos haluat rekisteröidä kaikki tietokoneet, määritä **Kaikki** rekisteröimään automaattisesti kaikki käyttäjätietokoneet, jotka on liitetty Azure AD:hen ja uusiin tietokoneisiin, kun käyttäjät lisäävät työtilin Windowsiin.</span><span class="sxs-lookup"><span data-stu-id="fdb81-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="fdb81-131">Määritä **Joidenkin-asetukseksi,** jos haluat rekisteröidä tietyn käyttäjäryhmän tietokoneet.</span><span class="sxs-lookup"><span data-stu-id="fdb81-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="fdb81-132">Lisää Azure AD:ssä synkronoidut toimialueen käyttäjät [suojausryhmään](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="fdb81-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="fdb81-133">Ota MDM-käyttäjäalue käyttöön kyseisessä suojausryhmässä valitsemalla **Valitse ryhmät.**</span><span class="sxs-lookup"><span data-stu-id="fdb81-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="fdb81-134">4. Tarvittavien resurssien luominen</span><span class="sxs-lookup"><span data-stu-id="fdb81-134">4. Create the required resources</span></span> 

<span data-ttu-id="fdb81-135">Tarvittavien tehtävien suorittamista [Azure AD -yhdistelmän määrittämiseksi](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) on yksinkertaistettu [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) [PowerShell-moduulissa olevan Initialize-SecMgmtHybirdDeviceEnrollment-cmdlet-otoksen](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) avulla.</span><span class="sxs-lookup"><span data-stu-id="fdb81-135">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="fdb81-136">Kun käynnistät tämän cmdlet-liitännän, se luo ja määrittää tarvittavan palveluyhteyspisteen ja ryhmäkäytännön.</span><span class="sxs-lookup"><span data-stu-id="fdb81-136">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="fdb81-137">Voit asentaa tämän moduulin vetoamalla PowerShellin esiintymään seuraaviin nätin:</span><span class="sxs-lookup"><span data-stu-id="fdb81-137">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="fdb81-138">On suositeltavaa asentaa tämä moduuli Windows Serveriin, jossa on Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="fdb81-138">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="fdb81-139">Voit luoda tarvittavan palveluyhteyspisteen ja ryhmäkäytännön käynnistämalla [Initialize-SecMgmtHybirdDeviceEnrollment-cmdlet-liitännän.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="fdb81-139">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="fdb81-140">Tarvitset Microsoft 365 Business Premiumin yleiset järjestelmänvalvojan tunnistetiedot tätä tehtävää suoritettaessa.</span><span class="sxs-lookup"><span data-stu-id="fdb81-140">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="fdb81-141">Kun olet valmis luomaan resurssit, käynnistä seuraavat toimet:</span><span class="sxs-lookup"><span data-stu-id="fdb81-141">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="fdb81-142">Ensimmäinen komento muodostaa yhteyden Microsoftin pilveen, ja kun sinua kehotetaan, määritä Microsoft 365 Business Premiumin yleiset järjestelmänvalvojan tunnistetiedot.</span><span class="sxs-lookup"><span data-stu-id="fdb81-142">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="fdb81-143">5. Linkitä ryhmäkäytäntö</span><span class="sxs-lookup"><span data-stu-id="fdb81-143">5. Link the Group Policy</span></span>

1. <span data-ttu-id="fdb81-144">Napsauta ryhmäkäytäntöjen hallintakonsolissa (GPMC) hiiren kakkospainikkeella sijaintia, johon haluat linkittää käytännön, ja valitse pikavalikosta *Linkitä aiemmin luotu ryhmäkäytäntöobjekti...*</span><span class="sxs-lookup"><span data-stu-id="fdb81-144">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="fdb81-145">Valitse yllä olevassa vaiheessa luotu käytäntö ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="fdb81-145">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="fdb81-146">Hanki uusimmat hallintamallit</span><span class="sxs-lookup"><span data-stu-id="fdb81-146">Get the latest Administrative Templates</span></span>

<span data-ttu-id="fdb81-147">Jos käytäntö **Ota automaattinen MDM-rekisteröinti käyttöön Azure AD -oletustunnistetietojen avulla**ei ole näkyvissä , syy siihen, että ADMX:ää ei ole asennettu Windows 10:lle, versiolle 1803, versiolle 1809 tai versiolle 1903.</span><span class="sxs-lookup"><span data-stu-id="fdb81-147">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="fdb81-148">Voit korjata ongelman seuraavasti (Huomautus: uusin MDM.admx on taaksepäin yhteensopiva):</span><span class="sxs-lookup"><span data-stu-id="fdb81-148">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="fdb81-149">Download: [Windows 10:n toukokuun 2019 päivitys (1903) hallintamallit (.admx).](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all)</span><span class="sxs-lookup"><span data-stu-id="fdb81-149">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="fdb81-150">Asenna paketti ensisijaiseen toimialueen ohjauskoneeseen (PDC).</span><span class="sxs-lookup"><span data-stu-id="fdb81-150">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="fdb81-151">Siirry kansion version mukaan: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="fdb81-151">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="fdb81-152">Nimeä **käytäntömääritykset** -kansio uudelleen edellä mainitussa **PolicyDefinitions-polun polussa.**</span><span class="sxs-lookup"><span data-stu-id="fdb81-152">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="fdb81-153">Kopioi **PolicyDefinitions-kansio** **kansioon C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="fdb81-153">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="fdb81-154">Jos aiot käyttää koko toimialueen keskitettyä käytäntösäilöä, lisää siihen PolicyDefinitions-sisältö.</span><span class="sxs-lookup"><span data-stu-id="fdb81-154">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="fdb81-155">Käynnistä ensisijainen toimialueen ohjauskone uudelleen, jotta käytäntö on käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="fdb81-155">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="fdb81-156">Tämä menettely toimii kaikissa tulevissa versioissa samoin.</span><span class="sxs-lookup"><span data-stu-id="fdb81-156">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="fdb81-157">Tässä vaiheessa sinun pitäisi pystyä näkemään käytäntö **Ota automaattinen MDM-rekisteröinti käyttöön käyttämällä Azure AD:n oletustunnistetietoja.**</span><span class="sxs-lookup"><span data-stu-id="fdb81-157">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>
