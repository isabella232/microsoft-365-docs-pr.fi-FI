---
title: Toimialueen liitettyjen Windows 10 -laitteiden ottaminen käyttöön Microsoft 365 for Businessin hallinnassa
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
description: Opi, miten voit ottaa Microsoft 365:n käyttöön paikallisten Active Directoryyn liitettyjen Windows 10 -laitteiden suojaamisessa muutamalla vaiheella.
ms.openlocfilehash: 0b597110447272be128bfe1866234ac25a8e67e6
ms.sourcegitcommit: 070724118be25cd83418d2a56863da95582dae65
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/03/2021
ms.locfileid: "50407074"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="b1bfe-103">Toimialueen liitettyjen Windows 10 -laitteiden ottaminen käyttöön Microsoft 365 Business Premiumin hallinnassa</span><span class="sxs-lookup"><span data-stu-id="b1bfe-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="b1bfe-104">Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Business Premiumin suojaamaan Windows 10 -laitteitasi säilyttäen silti paikallisen todentamisen edellyttävän paikallisen todentamisen resurssien käyttöoikeuden.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="b1bfe-105">Voit määrittää tämän suojauksen laitteella, joka on liitetty **Azure AD-yhdistelmäympäristön laitteisiin.**</span><span class="sxs-lookup"><span data-stu-id="b1bfe-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="b1bfe-106">Nämä laitteet liitetään sekä paikalliseen Active Directoryyn että Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="b1bfe-107">Tässä videossa kerrotaan, miten voit määrittää tämän yleisimpään tilanteeseen, joka on myös kuvattu seuraavissa vaiheissa.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="b1bfe-108">Varmista ennen aloittamista, että olet suorittanut seuraavat vaiheet:</span><span class="sxs-lookup"><span data-stu-id="b1bfe-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="b1bfe-109">Synkronoi käyttäjät Azure AD:n kanssa Azure AD Connectin avulla.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="b1bfe-110">Viimeistele Azure AD Connectin organisaatioyksikön (OU) synkronointi.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="b1bfe-111">Varmista, että kaikilla synkronoiduilla toimialuekäyttäjillä on Microsoft 365 Business Premiumin käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="b1bfe-112">Katso [ohjeet toimialuekäyttäjien synkronoinnin ohjeesta Microsoftin](manage-domain-users.md) kanssa.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="b1bfe-113">1. MDM-myöntäjän tarkistaminen Intunessa</span><span class="sxs-lookup"><span data-stu-id="b1bfe-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="b1bfe-114">Siirry [Endpoint Manageriin](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) ja valitse Microsoft Intune -sivulla Laitteen  rekisteröinti ja varmista Sitten Yleiskatsaus-sivulla, että **MDM-myöntäjä** on **Intune.**</span><span class="sxs-lookup"><span data-stu-id="b1bfe-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="b1bfe-115">Jos **MDM-myöntäjä** **on** Ei mitään, määritä sen arvoksi Intune napsauttamalla MDM-myöntäjää.  </span><span class="sxs-lookup"><span data-stu-id="b1bfe-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="b1bfe-116">Jos **MDM-myöntäjä** on Microsoft Office  **365,** siirry Laitteet-rekisteröintilaitteisiin ja lisää Intune MDM -myöntäjä oikealla olevan Lisää MDM -myöntäjä -valintaikkunan avulla (Lisää MDM-myöntäjä -valintaikkuna on käytettävissä vain, jos  >     **MDM-myöntäjäksi** on määritetty Microsoft Office 365). </span><span class="sxs-lookup"><span data-stu-id="b1bfe-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="b1bfe-117">2. Tarkista, että Azure AD on otettu käyttöön tietokoneisiin liittymistä varten</span><span class="sxs-lookup"><span data-stu-id="b1bfe-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="b1bfe-118">Siirry hallintakeskukseen ja valitse Hallintakeskukset-luettelosta Näytä kaikki, jos Azure Active Directory ei ole <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> näkyvissä.  </span><span class="sxs-lookup"><span data-stu-id="b1bfe-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="b1bfe-119">Siirry **Azure Active Directory -hallintakeskuksessa** **Azure Active Directoryyn,** valitse **Laitteet** ja sitten **Laiteasetukset.**</span><span class="sxs-lookup"><span data-stu-id="b1bfe-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="b1bfe-120">Tarkista,**että käyttäjät voivat liittyä laitteisiin Azure AD:ssä** on otettu käyttöön</span><span class="sxs-lookup"><span data-stu-id="b1bfe-120">Verify **Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="b1bfe-121">Jos haluat ottaa kaikki käyttäjät käyttöön, määritä arvoksi **Kaikki.**</span><span class="sxs-lookup"><span data-stu-id="b1bfe-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="b1bfe-122">Jos haluat ottaa tietyt käyttäjät käyttöön, **määritä** se valituiksi, jotta tietty käyttäjäryhmä otetaan käyttöön.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="b1bfe-123">Lisää haluamasi Azure AD:ssä synkronoidut toimialuekäyttäjät [käyttöoikeusryhmään.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="b1bfe-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="b1bfe-124">Ota **MDM-käyttäjäalue** käyttöön tässä käyttöoikeusryhmässä valitsemalla Valitse ryhmät.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="b1bfe-125">3. Tarkista, että Azure AD on otettu käyttöön MDM:ssä</span><span class="sxs-lookup"><span data-stu-id="b1bfe-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="b1bfe-126">Siirry hallintakeskukseen ja valitse <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Endpoint Managemen** t (Valitse **Näytä** kaikki, jos **Endpoint Manager** ei ole näkyvissä)</span><span class="sxs-lookup"><span data-stu-id="b1bfe-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen** t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="b1bfe-127">Valitse **Microsoft Endpoint Manager -hallintakeskuksessa** **Laitteet,**  >  **joissa Windows**  >  **Windows-rekisteröinti on automaattinen**  >  **rekisteröinti.**</span><span class="sxs-lookup"><span data-stu-id="b1bfe-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="b1bfe-128">Tarkista, että MDM-käyttäjän laajuus on otettu käyttöön.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="b1bfe-129">Jos haluat rekisteröidä kaikki  tietokoneet, määritä Kaikki rekisteröimaan automaattisesti kaikki käyttäjät, jotka on liitetty Azure AD:han ja uusiin tietokoneisiin, kun käyttäjät lisäävät työtilin Windowsiin.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="b1bfe-130">Määritä **Jotkin-asentoon** tietyn käyttäjäryhmän tietokoneiden rekisteröinti.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="b1bfe-131">Lisää haluamasi Azure AD:ssä synkronoidut toimialuekäyttäjät [käyttöoikeusryhmään.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="b1bfe-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="b1bfe-132">Ota **MDM-käyttäjäalue** käyttöön tässä käyttöoikeusryhmässä valitsemalla Valitse ryhmät.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="b1bfe-133">4. Tarvittavien resurssien luominen</span><span class="sxs-lookup"><span data-stu-id="b1bfe-133">4. Create the required resources</span></span> 

<span data-ttu-id="b1bfe-134">[Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) -yhdistelmäliitoksen määrittämiseen tarvittavien tehtävien suorittamista on yksinkertaistettu [Käyttämällä SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell -moduulin [Initialize-SecMgmtHybirdDeviceEnrollment-cmdlet-komentoa.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="b1bfe-134">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="b1bfe-135">Kun käynnistät tämän cmdlet-komentoa, se luo ja määrittää vaaditun palveluyhteyspisteen ja ryhmäkäytännön.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="b1bfe-136">Voit asentaa tämän moduulin käyttämällä PowerShellin esiintymää seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="b1bfe-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="b1bfe-137">On suositeltavaa asentaa tämä moduuli Windows Serveriin, jossa on Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="b1bfe-138">Jos haluat luoda vaaditun palveluyhteyspisteen ja ryhmäkäytännön, [käynnistä Initialize-SecMgmtHybirdDeviceEnrollment-cmdlet-komento.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="b1bfe-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="b1bfe-139">Tämän tehtävän suorittamiseen tarvitaan yleisen Microsoft 365 Business Premium -järjestelmänvalvojan tunnistetiedot.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="b1bfe-140">Kun olet valmis luomaan resurssit, käynnistä seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="b1bfe-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="b1bfe-141">Ensimmäinen komento muodostaa yhteyden Microsoftin pilvipalveluun, ja kun sinua pyydetään, määritä Microsoft 365 Business Premiumin yleisen järjestelmänvalvojan tunnistetiedot.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="b1bfe-142">5. Linkitä ryhmäkäytäntö</span><span class="sxs-lookup"><span data-stu-id="b1bfe-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="b1bfe-143">Napsauta ryhmäkäytäntöjen hallintakonsolissa hiiren kakkospainikkeella sijaintia, johon haluat linkittää  käytännön, ja valitse pikavalikosta Linkitä aiemmin luotu ryhmäkäytäntöobjekti...</span><span class="sxs-lookup"><span data-stu-id="b1bfe-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="b1bfe-144">Valitse yllä olevassa vaiheessa luotu käytäntö ja valitse **sitten OK.**</span><span class="sxs-lookup"><span data-stu-id="b1bfe-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="b1bfe-145">Hanki uusimmat hallintamallit</span><span class="sxs-lookup"><span data-stu-id="b1bfe-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="b1bfe-146">Jos et näe käytäntöä Ota automaattinen **MDM-rekisteröinti** käyttöön Azure AD:n oletustunnuksilla, tämä voi olla mahdollista, koska ADMX:ää ei ole asennettu Windows 10:tä, versiota 1803 tai uudempaa versiota varten.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, or later.</span></span> <span data-ttu-id="b1bfe-147">Voit korjata ongelman seuraavasti (Huomautus: uusin MDM.admx on yhteensopiva aiempien versioiden kanssa):</span><span class="sxs-lookup"><span data-stu-id="b1bfe-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="b1bfe-148">Lataa: [Windows 10:n hallintamallit (.admx) lokakuun 2020 päivitys (20H2).](https://www.microsoft.com/download/102157)</span><span class="sxs-lookup"><span data-stu-id="b1bfe-148">Download: [Administrative Templates (.admx) for Windows 10 October 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span></span>
2.  <span data-ttu-id="b1bfe-149">Asenna paketti toimialueen ohjauskoneeseen.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-149">Install the package on a Domain Controller.</span></span>
3.  <span data-ttu-id="b1bfe-150">Siirry kansioon hallintamallien version mukaan: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2).**</span><span class="sxs-lookup"><span data-stu-id="b1bfe-150">Navigate, depending on the Administrative Templates version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span></span>
4.  <span data-ttu-id="b1bfe-151">Nimeä yllä **olevassa** polussa oleva Käytäntömääritelmät-kansio uudelleen **PolicyDefinitions-kansioon.**</span><span class="sxs-lookup"><span data-stu-id="b1bfe-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="b1bfe-152">Kopioi **PolicyDefinitions-kansio** SYSVOL-jakamaan, oletusarvoisesti kansiossa **C:\Windows\SYSVOL\domain\Policies.**</span><span class="sxs-lookup"><span data-stu-id="b1bfe-152">Copy the **PolicyDefinitions** folder to your SYSVOL share, by default located at **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="b1bfe-153">Jos aiot käyttää koko toimialueen keskitettyä käytäntösäilöä, lisää Siellä PolicyDefinitions-sisältö.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="b1bfe-154">Jos sinulla on useita toimialueen ohjauskoneeseeneja, odota, että SYSVOL replikoi käytännöt.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-154">In case you have several Domain Controllers, wait for SYSVOL to replicate for the policies to be available.</span></span> <span data-ttu-id="b1bfe-155">Tämä toimenpide toimii myös kaikissa hallintamallien tulevissa versioissa.</span><span class="sxs-lookup"><span data-stu-id="b1bfe-155">This procedure will work for any future version of the Administrative Templates as well.</span></span>

<span data-ttu-id="b1bfe-156">Tässä vaiheessa sinun pitäisi nähdä käytäntö Ota käyttöön automaattinen MDM-rekisteröinti käyttämällä **oletusarvoista Azure AD -tunnistetietoja.**</span><span class="sxs-lookup"><span data-stu-id="b1bfe-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>
