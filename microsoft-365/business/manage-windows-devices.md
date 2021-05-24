---
title: Toimialueeseen liitettyjen Windows 10 laitteiden hallinnoiminen Microsoft 365 yrityksille
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
description: Opi, miten voit Microsoft 365 active-directory-laitteisiin Windows 10-laitteissasi muutamassa vaiheessa.
ms.openlocfilehash: f16962dd3c33c3c228da507bc5c4a902d76a8a08
ms.sourcegitcommit: b0d3abbccf4dd37e32d69664d3ebc9ab8dea760d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/21/2021
ms.locfileid: "52593889"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="5f146-103">Toimialueen liitettyjen laitteiden Windows 10 hallitaan Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="5f146-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="5f146-104">Jos organisaatiosi käyttää Windows Server Active Directorya paikallisesti, voit määrittää Microsoft 365 Business Premium:n suojaamaan Windows 10-laitteitasi säilyttäen edelleen paikallisen todentamisen edellyttävän paikallisen todentamisen resurssien käyttöoikeuden.</span><span class="sxs-lookup"><span data-stu-id="5f146-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="5f146-105">Voit määrittää tämän suojauksen laitteella, jossa Azure **AD-yhdistelmäympäristö on liitetty.**</span><span class="sxs-lookup"><span data-stu-id="5f146-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="5f146-106">Nämä laitteet liitetään sekä paikalliseen Active Directoryyn että Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5f146-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="5f146-107">Tässä videossa kuvataan ohjeet sen käyttöön yleisimpään tilanteeseen, joka on myös kuvattu seuraavissa vaiheissa.</span><span class="sxs-lookup"><span data-stu-id="5f146-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="5f146-108">Varmista ennen aloittamista, että olet suorittanut seuraavat vaiheet:</span><span class="sxs-lookup"><span data-stu-id="5f146-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="5f146-109">Synkronoi käyttäjät Azure AD:n kanssa Azure AD Näyttöyhteys.</span><span class="sxs-lookup"><span data-stu-id="5f146-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="5f146-110">Viimeistele Azure AD Näyttöyhteys organisaatioyksikön (OU) synkronointi.</span><span class="sxs-lookup"><span data-stu-id="5f146-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="5f146-111">Varmista, että kaikilla synkronoiduilla toimialuekäyttäjillä on käyttöoikeudet Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="5f146-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="5f146-112">Katso [ohjeet toimialuekäyttäjien synkronoiminen Microsoftiin.](manage-domain-users.md)</span><span class="sxs-lookup"><span data-stu-id="5f146-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="5f146-113">1. MDM-myöntäjän tarkistaminen Intunessa</span><span class="sxs-lookup"><span data-stu-id="5f146-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="5f146-114">Siirry [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) ja valitse Microsoft Intune -sivulla Laitteen rekisteröinti **ja** varmista sitten  Yleiskatsaus-sivulla, että **MDM-myöntäjä** on **Intune**.</span><span class="sxs-lookup"><span data-stu-id="5f146-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="5f146-115">Jos **MDM-myöntäjä** **on Ei** mitään , määritä **MDM-myöntäjäksi** **Intune.**</span><span class="sxs-lookup"><span data-stu-id="5f146-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="5f146-116">Jos **MDM-myöntäjä** on **Microsoft Office 365,** valitse Laitteet Ilmoittavat laitteet ja lisää Intune MDM -myöntäjä oikealla olevan Lisää MDM -myöntäjä -valintaikkunan avulla  >   (Lisää  **MDM-myöntäjä** -valintaikkuna on käytettävissä vain, jos **MDM-myöntäjäksi** on määritetty Microsoft Office 365). </span><span class="sxs-lookup"><span data-stu-id="5f146-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="5f146-117">2. Varmista, että Azure AD on otettu käyttöön tietokoneisiin liittymistä varten</span><span class="sxs-lookup"><span data-stu-id="5f146-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="5f146-118">Siirry hallintakeskukseen kohdassa ja valitse hallintakeskuksen Azure Active Directory (valitse Hallintakeskukset Azure Active Directory näytä kaikki, jos ne eivät <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **ole**  näkyvissä).</span><span class="sxs-lookup"><span data-stu-id="5f146-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="5f146-119">Siirry **Azure Active Directory hallintakeskuksessa** kohtaan Azure Active Directory **,** **valitse Laitteet** ja sitten **Laiteasetukset**.</span><span class="sxs-lookup"><span data-stu-id="5f146-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="5f146-120">Varmista,**että käyttäjät voivat liittyä laitteisiin Azure AD:ssä** on otettu käyttöön</span><span class="sxs-lookup"><span data-stu-id="5f146-120">Verify **Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="5f146-121">Ota kaikki käyttäjät käyttöön asettamalla arvoksi **Kaikki**.</span><span class="sxs-lookup"><span data-stu-id="5f146-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="5f146-122">Jos haluat ottaa tietyt käyttäjät käyttöön, valitse **Valittu,** jotta tietty käyttäjäryhmä otetaan käyttöön.</span><span class="sxs-lookup"><span data-stu-id="5f146-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="5f146-123">Lisää haluamasi Azure AD:ssä synkronoidut toimialuekäyttäjät [käyttöoikeusryhmään.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="5f146-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="5f146-124">Ota **MDM-käyttäjäalue** käyttöön tässä käyttöoikeusryhmässä valitsemalla Valitse ryhmät.</span><span class="sxs-lookup"><span data-stu-id="5f146-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="5f146-125">3. Varmista, että Azure AD on otettu käyttöön MDM:ssä</span><span class="sxs-lookup"><span data-stu-id="5f146-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="5f146-126">Siirry hallintakeskukseen at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ja valitse **Endpoint Managemen** t (valitse **Näytä kaikki,** **jos Endpoint Manager** ei ole näkyvissä)</span><span class="sxs-lookup"><span data-stu-id="5f146-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen** t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="5f146-127">Valitse **Microsoft Endpoint Manager hallintakeskuksessa** Laitteet, jotka   >  **Windows**  >  **Windows automaattisen**  >  **rekisteröinnin**.</span><span class="sxs-lookup"><span data-stu-id="5f146-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="5f146-128">Tarkista, että MDM-käyttäjäalue on käytössä.</span><span class="sxs-lookup"><span data-stu-id="5f146-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="5f146-129">Jos haluat rekisteröidä kaikki  tietokoneet, määritä Kaikki-asentoon, jos haluat rekisteröidä automaattisesti kaikki käyttäjät, jotka on liitetty Azure AD:han ja uusiin tietokoneisiin, kun käyttäjät lisäävät työtilin Windows.</span><span class="sxs-lookup"><span data-stu-id="5f146-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="5f146-130">Valitse **Jotkin,** jos haluat rekisteröidä tietyn käyttäjäryhmän tietokoneet.</span><span class="sxs-lookup"><span data-stu-id="5f146-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="5f146-131">Lisää haluamasi Azure AD:ssä synkronoidut toimialuekäyttäjät [käyttöoikeusryhmään.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="5f146-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="5f146-132">Ota **MDM-käyttäjäalue** käyttöön tässä käyttöoikeusryhmässä valitsemalla Valitse ryhmät.</span><span class="sxs-lookup"><span data-stu-id="5f146-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="5f146-133">4. Tarvittavien resurssien luominen</span><span class="sxs-lookup"><span data-stu-id="5f146-133">4. Create the required resources</span></span> 

<span data-ttu-id="5f146-134">[Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) -yhdistelmäliitoksen määrittämiseen tarvittavien tehtävien suorittamista on helpottettu [Käyttämällä Initialize-SecMgmtHybirdDeviceEnrollment-cmdlet-komentoa,](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) joka löytyy [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell -moduulista.</span><span class="sxs-lookup"><span data-stu-id="5f146-134">Performing the required tasks to [configure hybrid Azure AD join](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="5f146-135">Kun käynnistät tämän cmdlet-komentoa, se luo ja määrittää vaaditun palveluyhteyspisteen ja ryhmäkäytännön.</span><span class="sxs-lookup"><span data-stu-id="5f146-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="5f146-136">Voit asentaa tämän moduulin käyttämällä PowerShellin esiintymää seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="5f146-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="5f146-137">On suositeltavaa asentaa tämä moduuli Azure AD Windows-Näyttöyhteys.</span><span class="sxs-lookup"><span data-stu-id="5f146-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="5f146-138">Jos haluat luoda vaaditun palveluyhteyspisteen ja ryhmäkäytännön, käynnistä [Initialize-SecMgmtHybirdDeviceEnrollment-cmdlet-komento.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="5f146-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="5f146-139">Tämän tehtävän suorittamiseen tarvitaan Microsoft 365 Business Premium järjestelmänvalvojan tunnistetiedot.</span><span class="sxs-lookup"><span data-stu-id="5f146-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="5f146-140">Kun olet valmis luomaan resurssit, avaa seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="5f146-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="5f146-141">Ensimmäinen komento muodostaa yhteyden Microsoftin pilvipalveluun, ja kun sinua kehotetaan, määritä yleisen Microsoft 365 Business Premium tunnistetiedot.</span><span class="sxs-lookup"><span data-stu-id="5f146-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="5f146-142">5. Linkitä ryhmäkäytäntö</span><span class="sxs-lookup"><span data-stu-id="5f146-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="5f146-143">Napsauta ryhmäkäytäntöjen hallintakonsolissa hiiren kakkospainikkeella sijaintia, johon haluat linkittää käytännön, ja valitse pikavalikosta Linkitä aiemmin luotu *ryhmäkäytäntöobjekti....*</span><span class="sxs-lookup"><span data-stu-id="5f146-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="5f146-144">Valitse yllä olevassa vaiheessa luotu käytäntö ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="5f146-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="5f146-145">Hanki uusimmat hallintamallit</span><span class="sxs-lookup"><span data-stu-id="5f146-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="5f146-146">Jos et näe käytäntöä Enable **automatic MDM enrollment using default Azure AD credentials**(Ota automaattinen MDM-rekisteröinti käyttöön Azure AD:n oletustunnuksilla), ADMX ei ehkä ole asennettuna Windows 10:lle, versiolle 1803 tai uudempaan.</span><span class="sxs-lookup"><span data-stu-id="5f146-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, or later.</span></span> <span data-ttu-id="5f146-147">Voit korjata ongelman seuraavasti (Huomautus: uusin MDM.admx on yhteensopiva aiempien versioiden kanssa):</span><span class="sxs-lookup"><span data-stu-id="5f146-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="5f146-148">Lataa: [Hallintamallit (.admx) Windows 10 lokakuun 2020 päivityksen (20H2) mukaan.](https://www.microsoft.com/download/102157)</span><span class="sxs-lookup"><span data-stu-id="5f146-148">Download: [Administrative Templates (.admx) for Windows 10 October 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span></span>
2.  <span data-ttu-id="5f146-149">Asenna paketti toimialueen ohjauskoneeseen.</span><span class="sxs-lookup"><span data-stu-id="5f146-149">Install the package on a Domain Controller.</span></span>
3.  <span data-ttu-id="5f146-150">Siirry kansioon hallintamalliversion mukaan: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2).**</span><span class="sxs-lookup"><span data-stu-id="5f146-150">Navigate, depending on the Administrative Templates version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span></span>
4.  <span data-ttu-id="5f146-151">Nimeä yllä **olevassa** polussa oleva Käytäntömääritykset-kansio uudelleen **policydefinitions-kansioon.**</span><span class="sxs-lookup"><span data-stu-id="5f146-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="5f146-152">Kopioi **PolicyDefinitions-kansio** SYSVOL-jakamaan, oletusarvoisesti sijaintiin **C:\Windows\SYSVOL\domain\Policies.**</span><span class="sxs-lookup"><span data-stu-id="5f146-152">Copy the **PolicyDefinitions** folder to your SYSVOL share, by default located at **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="5f146-153">Jos aiot käyttää keskitettyä käytäntösäilöä koko toimialueellesi, lisää Siellä PolicyDefinitions -sisältö.</span><span class="sxs-lookup"><span data-stu-id="5f146-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="5f146-154">Jos sinulla on useita toimialueen ohjauskomia, odota, että SYSVOL replikoi käytännöt.</span><span class="sxs-lookup"><span data-stu-id="5f146-154">In case you have several Domain Controllers, wait for SYSVOL to replicate for the policies to be available.</span></span> <span data-ttu-id="5f146-155">Tämä toimenpide toimii myös kaikissa tulevissa hallintamallien versioissa.</span><span class="sxs-lookup"><span data-stu-id="5f146-155">This procedure will work for any future version of the Administrative Templates as well.</span></span>

<span data-ttu-id="5f146-156">Tässä vaiheessa sinun pitäisi nähdä käytäntö Enable automatic MDM enrollment using default Azure AD credentials available (Ota käyttöön automaattinen **MDM-rekisteröinti käyttäen oletusarvoista Azure AD -tunnistetietoja).**</span><span class="sxs-lookup"><span data-stu-id="5f146-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

## <a name="related-content"></a><span data-ttu-id="5f146-157">Aiheeseen liittyvä sisältö</span><span class="sxs-lookup"><span data-stu-id="5f146-157">Related content</span></span>

<span data-ttu-id="5f146-158">[Toimialuekäyttäjien synkronoiminen Microsoft 365](manage-domain-users.md) (artikkeli)</span><span class="sxs-lookup"><span data-stu-id="5f146-158">[Synchronize domain users to Microsoft 365](manage-domain-users.md) (article)</span></span>

<span data-ttu-id="5f146-159">[Ryhmän luominen hallintakeskuksessa](../admin/create-groups/create-groups.md) (artikkeli)</span><span class="sxs-lookup"><span data-stu-id="5f146-159">[Create a group in the admin center](../admin/create-groups/create-groups.md) (article)</span></span>

<span data-ttu-id="5f146-160">[Opetusohjelma: Yhdistelmäympäristön Azure Active Directory määrittäminen hallittuja toimialueita varten](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (artikkeli)</span><span class="sxs-lookup"><span data-stu-id="5f146-160">[Tutorial: Configure hybrid Azure Active Directory join for managed domains](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (article)</span></span>