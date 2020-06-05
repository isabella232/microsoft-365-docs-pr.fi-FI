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
ms.openlocfilehash: 857651081fb10856d28dd419333ebef655388407
ms.sourcegitcommit: e6e704cbd9a50fc7db1e6a0cf5d3f8c6cbb94363
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/04/2020
ms.locfileid: "44564933"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="a6ca4-103">Toimialueen käyttöön liitettyjen Windows 10 -laitteiden hallinta Microsoft 365 Business Premiumilla</span><span class="sxs-lookup"><span data-stu-id="a6ca4-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="a6ca4-104">Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Business Premiumin suojaamaan Windows 10 -laitteita säilyttäen samalla paikallisen todennuksen edellyttävien paikallisten resurssien käytön.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="a6ca4-105">Voit määrittää tämän suojauksen mukautuksella **Hybrid Azure AD -liitettyjä laitteita**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="a6ca4-106">Nämä laitteet on liitetty sekä paikalliseen Active Directoryyn että Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="a6ca4-107">Tässä videossa kuvataan, miten tämä määritetään yleisin skenaario, joka on myös kuvattu vaiheet, joita seurataan.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="a6ca4-108">Ennen kuin aloitat, varmista, että olet suorittanut seuraavat toimet:</span><span class="sxs-lookup"><span data-stu-id="a6ca4-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="a6ca4-109">Synkronoi käyttäjät Azure AD:hen Azure AD Connectin avulla.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="a6ca4-110">Suorita Azure AD Connect Organizational Unit (OU) -synkronointi loppuun.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="a6ca4-111">Varmista, että kaikilla synkronoiduilla toimialueen käyttäjillä on käyttöoikeudet Microsoft 365 Business Premiumiin.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="a6ca4-112">Vaiheet ovat [ohjeaiheessa Toimialueen käyttäjien synkronoiminen Microsoftiin.](manage-domain-users.md)</span><span class="sxs-lookup"><span data-stu-id="a6ca4-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="a6ca4-113">1. Tarkista MDM-viranomainen Intuessa</span><span class="sxs-lookup"><span data-stu-id="a6ca4-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="a6ca4-114">Siirry portal.azure.com ja sivun yläreunassa etsi Intune.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-114">Go to portal.azure.com and on the top of the page search for Intune.</span></span>
<span data-ttu-id="a6ca4-115">Valitse Microsoft Intune -sivulla **Laiterekisteröinti** ja varmista **Yleiskatsaus-sivulla,** että **MDM-myöntäjä** on **Intune**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-115">On the Microsoft Intune page, select **Device enrollment** and on the **Overview** page make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="a6ca4-116">Jos **MDM-viranomainen** **ei ole Ei mitään**, määritä **MDM-myöntäjäksi** **Intune**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="a6ca4-117">Jos **MDM-myöntäjä** on **Microsoft Office 365**, siirry **Devices**  >  **Laitteet-rekisteröintilaitteisiin** ja lisää **Intune MDM** -myöntäjä lisää **MDM-myöntäjän lisääminen** -valintaikkunassa **(Lisää MDM-myöntäjä** -valintaikkuna on käytettävissä vain, jos **MDM-myöntäjäksi** on määritetty Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="a6ca4-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="a6ca4-118">2. Varmista, että Azure AD on otettu käyttöön tietokoneiden liittämistä varten</span><span class="sxs-lookup"><span data-stu-id="a6ca4-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="a6ca4-119">Siirry hallintakeskukseen kohdassa <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ja valitse **Hallintakeskukset-luettelosta Azure Active Directory** (valitse Näytä kaikki, jos Azure Active Directory ei ole näkyvissä). **Admin centers**</span><span class="sxs-lookup"><span data-stu-id="a6ca4-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="a6ca4-120">Siirry **Azure Active Directory -hallintakeskuksessa** **Azure Active Directoryyn** , valitse **Laitteet** ja sitten **Laiteasetukset**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="a6ca4-121">Tarkista, että**käyttäjät voivat liittyä laitteisiin Azure AD:ssä** on käytössä</span><span class="sxs-lookup"><span data-stu-id="a6ca4-121">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="a6ca4-122">Jos haluat ottaa kaikki käyttäjät käyttöön, määritä **Kaikki**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="a6ca4-123">Jos haluat ottaa tietyt käyttäjät käyttöön, ota tietty käyttäjäryhmä käyttöön määrittämällä **Valittu.**</span><span class="sxs-lookup"><span data-stu-id="a6ca4-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="a6ca4-124">Lisää Azure AD:ssä synkronoidut toimialueen käyttäjät [suojausryhmään](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="a6ca4-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="a6ca4-125">Ota MDM-käyttäjäalue käyttöön kyseisessä suojausryhmässä valitsemalla **Valitse ryhmät.**</span><span class="sxs-lookup"><span data-stu-id="a6ca4-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="a6ca4-126">3. Varmista, että Azure AD on otettu käyttöön MDM:ssä</span><span class="sxs-lookup"><span data-stu-id="a6ca4-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="a6ca4-127">Siirry hallintakeskukseen ja <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> valitse **päätepisteen hallinta**t (valitse Näytä **kaikki,** jos **Päätepisteen hallinta** ei ole näkyvissä)</span><span class="sxs-lookup"><span data-stu-id="a6ca4-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="a6ca4-128">Siirry **Microsoft Endpoint Manager -hallintakeskuksessa** **kohtaan Laitteet**  >  **Windows**  >  **Windowsin rekisteröityminen**  >  **automaattisesti**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="a6ca4-129">Varmista, että MDM-käyttäjän vaikutusalue on käytössä.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="a6ca4-130">Jos haluat rekisteröidä kaikki tietokoneet, määritä **Kaikki** rekisteröimään automaattisesti kaikki käyttäjätietokoneet, jotka on liitetty Azure AD:hen ja uusiin tietokoneisiin, kun käyttäjät lisäävät työtilin Windowsiin.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="a6ca4-131">Määritä **Joidenkin-asetukseksi,** jos haluat rekisteröidä tietyn käyttäjäryhmän tietokoneet.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="a6ca4-132">Lisää Azure AD:ssä synkronoidut toimialueen käyttäjät [suojausryhmään](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="a6ca4-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="a6ca4-133">Ota MDM-käyttäjäalue käyttöön kyseisessä suojausryhmässä valitsemalla **Valitse ryhmät.**</span><span class="sxs-lookup"><span data-stu-id="a6ca4-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-set-up-service-connection-point-scp"></a><span data-ttu-id="a6ca4-134">4. Palveluyhteyspisteen (SCP) määrittäminen</span><span class="sxs-lookup"><span data-stu-id="a6ca4-134">4. Set up Service connection point (SCP)</span></span>

<span data-ttu-id="a6ca4-135">Näitä vaiheita yksinkertaistetaan [hybridi azure AD -liitoksen määrittämisestä.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="a6ca4-135">These steps are simplified from [configure hybrid azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="a6ca4-136">Voit suorittaa azure AD Connectin ja Microsoft 365 Business Premiumin yleisen järjestelmänvalvojan ja Active Directory -järjestelmänvalvojan salasanat.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-136">To complete the steps you need to use Azure AD Connect and your Microsoft 365 Business Premium global admin and Active Directory admin passwords.</span></span>

1.  <span data-ttu-id="a6ca4-137">Käynnistä Azure AD Connect ja valitse sitten **Määritä**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-137">Start Azure AD Connect, and then select **Configure**.</span></span>
2.  <span data-ttu-id="a6ca4-138">Valitse **Lisätehtävät-sivulla** **Määritä laiteasetukset**ja valitse sitten **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-138">On the **Additional tasks**  page, select **Configure device options**, and then select **Next**.</span></span>
3.  <span data-ttu-id="a6ca4-139">Valitse **Yleiskatsaus-sivulla** **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-139">On the **Overview** page, select **Next**.</span></span>
4.  <span data-ttu-id="a6ca4-140">Kirjoita **Yhdistä Azure AD:hen** -sivulla Microsoft 365 Business Premiumin yleisen järjestelmänvalvojan tunnistetiedot.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-140">On the **Connect to Azure AD** page, enter the credentials of a global administrator for Microsoft 365 Business Premium.</span></span>
5.  <span data-ttu-id="a6ca4-141">Valitse **Laiteasetukset-sivulla** **Määritä Azure AD -yhdistelmäliitos**ja valitse sitten **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-141">On the **Device options** page, select **Configure Hybrid Azure AD join**, and then select **Next**.</span></span>
6.  <span data-ttu-id="a6ca4-142">Tee seuraavat vaiheet **SCP-sivulla** jokaiselle puuryhmälle, johon haluat Azure AD Connectin määrittävän SCP:n, ja valitse sitten **Seuraava**:</span><span class="sxs-lookup"><span data-stu-id="a6ca4-142">On the **SCP** page, for each forest where you want Azure AD Connect to configure the SCP, complete the following steps, and then select **Next**:</span></span>
    - <span data-ttu-id="a6ca4-143">Valitse metsän nimen vieressä oleva valintaruutu.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-143">Check the box beside the forest name.</span></span> <span data-ttu-id="a6ca4-144">Puuryhmän pitäisi olla AD-toimialuenimesi.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-144">The forest should be your AD domain name.</span></span>
    - <span data-ttu-id="a6ca4-145">Avaa **Todennuspalvelu-sarakkeessa** avattava luettelo ja valitse vastaava toimialuenimi (vain yksi vaihtoehto pitäisi olla).</span><span class="sxs-lookup"><span data-stu-id="a6ca4-145">Under the **Authentication Service** column, open the dropdown and select matching domain name (there should only be one only option).</span></span>
    - <span data-ttu-id="a6ca4-146">Anna toimialueen järjestelmänvalvojan tunnistetiedot valitsemalla **Lisää.**</span><span class="sxs-lookup"><span data-stu-id="a6ca4-146">Select **Add** to enter the domain administrator credentials.</span></span>  
7.  <span data-ttu-id="a6ca4-147">Valitse **Laitteen käyttöjärjestelmät -sivulla** vain Windows 10 tai uudempi toimialueeseen liitetyt laitteet.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-147">On the **Device operating systems** page, select Windows 10 or later domain-joined devices only.</span></span>
8.  <span data-ttu-id="a6ca4-148">Valitse **Valmis konfiguroimaan** -sivulla **Määritä**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-148">On the **Ready to configure** page, select **Configure**.</span></span>
9.  <span data-ttu-id="a6ca4-149">Valitse **Kokoonpano valmis** -sivulla **Lopeta**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-149">On the **Configuration complete** page, select **Exit**.</span></span>


## <a name="5-create-a-gpo-for-intune-enrollment--admx-method"></a><span data-ttu-id="a6ca4-150">5. Luo GPO Intune Ilmoittautuminen - ADMX menetelmä</span><span class="sxs-lookup"><span data-stu-id="a6ca4-150">5. Create a GPO for Intune Enrollment – ADMX method</span></span>

<span data-ttu-id="a6ca4-151">Käyttää. ADMX-mallitiedosto.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-151">Use .ADMX template file.</span></span>

1.  <span data-ttu-id="a6ca4-152">Kirjaudu AD-palvelimeen, etsi ja avaa **Server Manager**  >  **Tools**  >  **-ryhmäkäytäntöjen hallinta**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-152">Log on to AD server, search and open **Server Manager** > **Tools** > **Group Policy Management**.</span></span>
2.  <span data-ttu-id="a6ca4-153">Valitse toimialuenimi **Toimialueet-kohdasta** ja valitse **Uusi**napsauttamalla hiiren kakkospainikkeella **Ryhmäkäytäntöobjektit** .</span><span class="sxs-lookup"><span data-stu-id="a6ca4-153">Select your domain name under **Domains** and right-click **Group Policy Objects** to select **New**.</span></span>
3.  <span data-ttu-id="a6ca4-154">Anna uudelle gpo:lle nimi, esimerkiksi "*Cloud_Enrollment*" ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-154">Give the new GPO an name, for example “*Cloud_Enrollment*” and then select **OK**.</span></span>
4.  <span data-ttu-id="a6ca4-155">Napsauta uutta ryhmäkäytäntöobjektia hiiren kakkospainikkeella **ryhmäkäytäntöobjektien** alla ja valitse **Muokkaa**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-155">Right-click the new GPO under **Group Policy Objects** and select **Edit**.</span></span>
5.  <span data-ttu-id="a6ca4-156">Siirry **ryhmäkäytäntöjen hallintaeditorissa** **kohtaan Tietokonemäärityskäytännöt**  >  **Policies**  >  **Hallintamallit**  >  **Windowsin osien**  >  **MDM**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-156">In the **Group Policy Management Editor**, go to **Computer Configuration** > **Policies** > **Administrative Templates** > **Windows Components** > **MDM**.</span></span>
6. <span data-ttu-id="a6ca4-157">Napsauta hiiren kakkospainikkeella **Ota automaattinen MDM-rekisteröinti käyttöön Azure AD -oletustunnistetietojen avulla** ja valitse sitten **Käytössä**  >  **OK**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-157">Right-click **Enable automatic MDM enrollment using default Azure AD credentials** and then select **Enabled** > **OK**.</span></span> <span data-ttu-id="a6ca4-158">Sulje editori-ikkuna.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-158">Close the editor window.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a6ca4-159">Jos **käytäntöä Ota automaattinen MDM-rekisteröinti käyttöön Azure AD -oletustunnistetietojen avulla**ei ole näkyvissä , katso [uusimmat hallintamallit](#get-the-latest-administrative-templates).</span><span class="sxs-lookup"><span data-stu-id="a6ca4-159">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, see [Get the latest Administrative Templates](#get-the-latest-administrative-templates).</span></span>

## <a name="6-deploy-the-group-policy"></a><span data-ttu-id="a6ca4-160">6. Ryhmäkäytännön käyttöönotto</span><span class="sxs-lookup"><span data-stu-id="a6ca4-160">6. Deploy the Group Policy</span></span>

1.  <span data-ttu-id="a6ca4-161">Valitse Palvelimen hallinnan **Toimialueet** > ryhmäkäytäntöobjektit -kohdassa ryhmäkäytäntöobjekti yllä olevasta vaiheesta 3, esimerkiksi "Cloud_Enrollment".</span><span class="sxs-lookup"><span data-stu-id="a6ca4-161">In the Server Manager, under **Domains** > Group Policy objects, select the GPO from Step 3 above, for example “Cloud_Enrollment”.</span></span>
2.  <span data-ttu-id="a6ca4-162">Valitse **gpo:n Laajuus-välilehti.**</span><span class="sxs-lookup"><span data-stu-id="a6ca4-162">Select the **Scope** tab for your GPO.</span></span>
3.  <span data-ttu-id="a6ca4-163">Napsauta GPO:n Vaikutusalue-välilehden **Linkit**-kohdan toimialueen linkkiä hiiren kakkospainikkeella.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-163">In the GPO’s Scope tab, right-click the link to the domain under **Links**.</span></span>
4.  <span data-ttu-id="a6ca4-164">Ota gpo käyttöön valitsemalla **Pakotettu** ja sitten **OK** vahvistusnäytössä.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-164">Select **Enforced** to deploy the GPO and then **OK** in the confirmation screen.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="a6ca4-165">Hanki uusimmat hallintamallit</span><span class="sxs-lookup"><span data-stu-id="a6ca4-165">Get the latest Administrative Templates</span></span>

<span data-ttu-id="a6ca4-166">Jos käytäntö **Ota automaattinen MDM-rekisteröinti käyttöön Azure AD -oletustunnistetietojen avulla**ei ole näkyvissä , syy siihen, että ADMX:ää ei ole asennettu Windows 10:lle, versiolle 1803, versiolle 1809 tai versiolle 1903.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-166">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="a6ca4-167">Voit korjata ongelman seuraavasti (Huomautus: uusin MDM.admx on taaksepäin yhteensopiva):</span><span class="sxs-lookup"><span data-stu-id="a6ca4-167">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="a6ca4-168">Download: [Windows 10:n toukokuun 2019 päivitys (1903) hallintamallit (.admx).](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all)</span><span class="sxs-lookup"><span data-stu-id="a6ca4-168">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="a6ca4-169">Asenna paketti ensisijaiseen toimialueen ohjauskoneeseen (PDC).</span><span class="sxs-lookup"><span data-stu-id="a6ca4-169">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="a6ca4-170">Siirry kansion version mukaan: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-170">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="a6ca4-171">Nimeä **käytäntömääritykset** -kansio uudelleen edellä mainitussa **PolicyDefinitions-polun polussa.**</span><span class="sxs-lookup"><span data-stu-id="a6ca4-171">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="a6ca4-172">Kopioi **PolicyDefinitions-kansio** **kansioon C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-172">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="a6ca4-173">Jos aiot käyttää koko toimialueen keskitettyä käytäntösäilöä, lisää siihen PolicyDefinitions-sisältö.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-173">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="a6ca4-174">Käynnistä ensisijainen toimialueen ohjauskone uudelleen, jotta käytäntö on käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-174">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="a6ca4-175">Tämä menettely toimii kaikissa tulevissa versioissa samoin.</span><span class="sxs-lookup"><span data-stu-id="a6ca4-175">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="a6ca4-176">Tässä vaiheessa sinun pitäisi pystyä näkemään käytäntö **Ota automaattinen MDM-rekisteröinti käyttöön käyttämällä Azure AD:n oletustunnistetietoja.**</span><span class="sxs-lookup"><span data-stu-id="a6ca4-176">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

