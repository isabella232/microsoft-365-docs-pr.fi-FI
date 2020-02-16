---
title: Microsoft 365 Business -versioon päivittäminen Office 365 Business Premiumista
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Vaiheet, jotka päivittät yrityksesi Office 365 Business Premiumista Microsoft 365 Business -versioon.
ms.openlocfilehash: e17ac2658c7276ba4a77de371847343866815c42
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065267"
---
# <a name="upgrade-to-microsoft-365-business-from-office-365-business-premium"></a><span data-ttu-id="5484a-103">Microsoft 365 Business -versioon päivittäminen Office 365 Business Premiumista</span><span class="sxs-lookup"><span data-stu-id="5484a-103">Upgrade to Microsoft 365 Business from Office 365 Business Premium</span></span>

<span data-ttu-id="5484a-104">Jos sinulla on [Office 365 for Business -tilaus,](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2)esimerkiksi Office 365 Business Premium, voit helposti päivittää Microsoft 365 Businessiin.</span><span class="sxs-lookup"><span data-stu-id="5484a-104">If you have an [Office 365 for business subscription](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), for example, Office 365 Business Premium, you can easily upgrade to Microsoft 365 Business.</span></span> <span data-ttu-id="5484a-105">Päivitä Microsoft 365 Businessiin, jos haluat lisätä:</span><span class="sxs-lookup"><span data-stu-id="5484a-105">Upgrade to Microsoft 365 Business if you want to add:</span></span> 
- <span data-ttu-id="5484a-106">Windows 10 Pro (Windows 8 tai uudempi) -tietokoneisiin</span><span class="sxs-lookup"><span data-stu-id="5484a-106">Windows 10 Pro (to PCs running Windows 8 or later)</span></span>
- <span data-ttu-id="5484a-107">Yksinkertaiset ohjausobjektit, jotka hallitsevat liiketoimintatietoja laitteissa</span><span class="sxs-lookup"><span data-stu-id="5484a-107">Simple controls that manage business data on devices</span></span>
- <span data-ttu-id="5484a-108">Kehittyneet suojausominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="5484a-108">Advanced security capabilities.</span></span>
<span data-ttu-id="5484a-109">Lue lisää Microsoft 365 Businessista [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span><span class="sxs-lookup"><span data-stu-id="5484a-109">Find out more about Microsoft 365 Business at [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span></span>

## <a name="whats-the-difference-between-office-365-business-premium-and-microsoft-365-business"></a><span data-ttu-id="5484a-110">Mitä eroa on Office 365 Business Premiumilla ja Microsoft 365 Businessilla?</span><span class="sxs-lookup"><span data-stu-id="5484a-110">What's the difference between Office 365 Business Premium and Microsoft 365 Business?</span></span>
<span data-ttu-id="5484a-111">Olemme lisänneet näiden kahden palvelupaketin sivuvertailun [Microsoft 365 Business Service Description -palveluun.](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description)</span><span class="sxs-lookup"><span data-stu-id="5484a-111">We've added a side-by-side comparison of these two plans to the [Microsoft 365 Business Service Description](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description).</span></span> 

## <a name="before-you-get-started"></a><span data-ttu-id="5484a-112">Ennen kuin aloitat</span><span class="sxs-lookup"><span data-stu-id="5484a-112">Before you get started</span></span>

- <span data-ttu-id="5484a-113">**Milloin minun pitäisi valita päivitys?**</span><span class="sxs-lookup"><span data-stu-id="5484a-113">**When should I choose to upgrade?**</span></span> <span data-ttu-id="5484a-114">Päivitys on oikea valinta, kun haluat päivittää **kaikki yksittäiseen** palvelupakettiin määritetyt käyttäjät.</span><span class="sxs-lookup"><span data-stu-id="5484a-114">Upgrade is the right choice when you want to upgrade **all users** assigned to a single plan.</span></span> <span data-ttu-id="5484a-115">Kun valitset päivityksen, kaikki palvelupaketin käyttäjät siirtyvät toiseen palvelupakettiin samanaikaisesti.</span><span class="sxs-lookup"><span data-stu-id="5484a-115">When you choose upgrade, all plan users get switched to another plan at the same time.</span></span> <span data-ttu-id="5484a-116">Jos et halua päivittää kaikkia yksittäiseen palvelupakettiin määritettyjä, osta uuden palvelupaketin käyttöoikeudet (tässä tapauksessa Microsoft 365 Business) ja [määritä kyseiset käyttöoikeudet erikseen](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) jokaiselle käyttäjälle, jonka haluat päivittää.</span><span class="sxs-lookup"><span data-stu-id="5484a-116">If you don't want to upgrade everyone assigned to a single plan, buy licenses for the new plan (in this case Microsoft 365 Business), and [assign those licenses individually](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) to each user that you want to upgrade.</span></span> 
- <span data-ttu-id="5484a-117">**Jotkin lisäosat saattavat estää päivityksen** Jos yrität käynnistää päivityksen ja sinulla on lisäosa, joka estää sinua jatkamasta, voit poistaa lisäosan ensin ja lisätä sen myöhemmin takaisin, jos tarvitset sitä edelleen.</span><span class="sxs-lookup"><span data-stu-id="5484a-117">**Some add-ons might prevent the upgrade** If you try to start an upgrade and you have an add-on that prevents you from continuing, you can remove the add-on first, and then add it back later if you still need it.</span></span> 
- <span data-ttu-id="5484a-118">**Jos olet maksanut tilauksesi valmiiksi** Valmiiksi maksetuille palvelupaketoille ei ole yksinkertaista päivityspolkua.</span><span class="sxs-lookup"><span data-stu-id="5484a-118">**If you prepaid your plan** There isn't a straightforward upgrade path for prepaid plans.</span></span> <span data-ttu-id="5484a-119">Tiedät, onko sinulla valmiiksi maksettu palvelupaketti, koska olet määrittänyt tilauksesi käyttämällä tuotetunnusta, jonka olet ehkä ostanut kaupasta.</span><span class="sxs-lookup"><span data-stu-id="5484a-119">You'll know if you have a prepaid plan because you set up your plan using a product ID that you might have purchased in a store.</span></span> <span data-ttu-id="5484a-120">Ota yhteyttä kumppaniin, siirry Microsoft Storeen tai odota, kunnes valmiiksi maksettu palvelupaketti vanhenee, jotta voit siirtyä uuteen palvelupakettiin.</span><span class="sxs-lookup"><span data-stu-id="5484a-120">Contact a partner, go to the Microsoft Store, or wait until your prepaid plan expires to switch to a new plan.</span></span>

## <a name="upgrade-to-microsoft-365-business"></a><span data-ttu-id="5484a-121">Päivitä Microsoft 365 Businessiin</span><span class="sxs-lookup"><span data-stu-id="5484a-121">Upgrade to Microsoft 365 Business</span></span>
<span data-ttu-id="5484a-122">Osta käyttöoikeudet seuraavasti [uudessa hallintakeskuksessa:](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="5484a-122">Buy your licenses by following these steps in the [new admin center](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview):</span></span>
1. <span data-ttu-id="5484a-123">Kirjaudu hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="5484a-123">Sign into the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>
2. <span data-ttu-id="5484a-124">Siirry siirtymisruutuun ja valitse **Laskutustuotteet** \> **& Palvelut**.</span><span class="sxs-lookup"><span data-stu-id="5484a-124">Go to the navigation pane and select **Billing** \> **Products & Services**.</span></span> <span data-ttu-id="5484a-125">Etsi Office 365 -tilauksesi ja valitse se, jos haluat tarkastella tietoja.</span><span class="sxs-lookup"><span data-stu-id="5484a-125">Find your Office 365 subscription and select it to view the details.</span></span> 

    ![Näyttökuva näyttää, miten voit etsiä ja valita tilauksesi hallintakeskuksessa.](../media/FindYourSubscription.png)

3. <span data-ttu-id="5484a-127">Valitse seuraavalla sivulla **Päivitä**.</span><span class="sxs-lookup"><span data-stu-id="5484a-127">On the next page, select **Upgrade**.</span></span> 

      ![Näyttökuva näyttää, missä valitse Päivitä hallintakeskuksessa.](../media/SelectUpgrade.png)

  > [!NOTE]
  > <span data-ttu-id="5484a-129">Jos näet viestin, jonka mukaan **Tilauksen päivittämistä ei tueta ryhmäpohjaisilla lisensointioikeuksilla Azure Active Directoryssa,** voit ohittaa tämän turvallisesti, ellei sinulla ole erittäin suurta organisaatiota.</span><span class="sxs-lookup"><span data-stu-id="5484a-129">If you see a message that says **Upgrading your subscription is not supported with group-based licensing in Azure Active Directory**, you can safely ignore this unless you have a very large organization.</span></span> <span data-ttu-id="5484a-130">Organisaatiot, jotka ovat valinneet tämän asetuksen, tietävät käyttävänsä ryhmäpohjaisia käyttöoikeuksia.</span><span class="sxs-lookup"><span data-stu-id="5484a-130">Organizations who have selected this option will be aware that they're using group-based licensing.</span></span>

4. <span data-ttu-id="5484a-131">Seuraavaksi voit tarkastella luetteloa Office-palvelupaketeista, joihin voit päivittää.</span><span class="sxs-lookup"><span data-stu-id="5484a-131">Next, you can view a list of Office plans that you can upgrade to.</span></span> <span data-ttu-id="5484a-132">Etsi tässä tapauksessa Microsoft 365 Business -palvelupaketti.</span><span class="sxs-lookup"><span data-stu-id="5484a-132">In this case, find the Microsoft 365 Business plan.</span></span> <span data-ttu-id="5484a-133">Voit vierittää alaspäin, jos haluat nähdä kaikki tähän palvelupakettiin sisältyvät Office-sovellukset ja -palvelut.</span><span class="sxs-lookup"><span data-stu-id="5484a-133">You can scroll down if you want to see all the Office apps and services that are included with this plan.</span></span> <span data-ttu-id="5484a-134">Lisää Microsoft 365 Business ostoskoriisi valitsemalla **Microsoft 365 Business**-kohdassa **Päivitä.**</span><span class="sxs-lookup"><span data-stu-id="5484a-134">Under **Microsoft 365 Business**, select **Upgrade** to add Microsoft 365 Business to your cart.</span></span>
5. <span data-ttu-id="5484a-135">Ostoskorissa:</span><span class="sxs-lookup"><span data-stu-id="5484a-135">In the cart:</span></span>
    1. <span data-ttu-id="5484a-136">Sisällytämme automaattisesti käyttöoikeudet kaikille nykyisille käyttäjillesi.</span><span class="sxs-lookup"><span data-stu-id="5484a-136">We'll automatically include licenses for all your current users.</span></span> <span data-ttu-id="5484a-137">Jos tarvitset enemmän tai vähemmän lisenssejä, sinun on [ostettava ja määritettävä kyseiset käyttöoikeudet erikseen](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="5484a-137">If you need more or fewer licenses, you need to [buy and assign those licenses individually](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users).</span></span>  
    2. <span data-ttu-id="5484a-138">Voit muuttaa maksutapaasi: kuukausittain tai vuosittain.</span><span class="sxs-lookup"><span data-stu-id="5484a-138">You can adjust how you'd like to pay: monthly or yearly.</span></span> <span data-ttu-id="5484a-139">Valitse haluamasi valikko avattavasta valikosta.</span><span class="sxs-lookup"><span data-stu-id="5484a-139">Select the drop-down menu to make your choice.</span></span>
6. <span data-ttu-id="5484a-140">Valitse **Siirry kassalle,** jossa näet yhteenvedon ostoksestasi, mukaan lukien tämän tilin maksutavan.</span><span class="sxs-lookup"><span data-stu-id="5484a-140">Select **Go to Checkout** where you'll see a summary of your purchase, including the payment method for this account.</span></span> <span data-ttu-id="5484a-141">Voit myös lisätä promo koodi täällä, jos sinulla on yksi.</span><span class="sxs-lookup"><span data-stu-id="5484a-141">You can also add a promo code here if you have one.</span></span>
7. <span data-ttu-id="5484a-142">Viimeistele ostos valitsemalla **Tee tilaus.**</span><span class="sxs-lookup"><span data-stu-id="5484a-142">Select **Place order** to complete your purchase.</span></span>
<span data-ttu-id="5484a-143">Uusien palvelupakettien määrittäminen kestää muutaman minuutin.</span><span class="sxs-lookup"><span data-stu-id="5484a-143">It takes Microsoft a few minutes to set up your new service plans.</span></span> <span data-ttu-id="5484a-144">Voit tarkistaa edistymisen valitsemalla **Tarkista päivityksen tila**.</span><span class="sxs-lookup"><span data-stu-id="5484a-144">To check on progress, select **Check upgrade status**.</span></span> 
1. <span data-ttu-id="5484a-145">Kun tilauksesi on valmis, sinun on ehkä suoritettava joitakin lisäasennusvaiheita hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="5484a-145">Once your plan is ready, you might need to complete some additional setup steps in the admin center.</span></span> <span data-ttu-id="5484a-146">Suorita muut asennusvaiheet valitsemalla siirtymisruudussa **Aloitus.**</span><span class="sxs-lookup"><span data-stu-id="5484a-146">In the navigation pane, select **Home** to complete any additional setup steps.</span></span>

> [!NOTE]
> <span data-ttu-id="5484a-147">Saat prorated-hyvityksen Office 365 -käyttöoikeuksista, joita et enää tarvitse.</span><span class="sxs-lookup"><span data-stu-id="5484a-147">You'll receive a prorated refund for the Office 365 licenses that you no longer need.</span></span> <span data-ttu-id="5484a-148">Pankkitililtäsi tai luottokortiltasi veloitetaan noin kaksi päivää uuden suunnitelman määrittämisen jälkeen.</span><span class="sxs-lookup"><span data-stu-id="5484a-148">Your bank account or credit card will be charged about two days after you set up the new plan.</span></span>
  
## <a name="protect-user-devices-and-files"></a><span data-ttu-id="5484a-149">Suojaa käyttäjän laitteet ja tiedostot</span><span class="sxs-lookup"><span data-stu-id="5484a-149">Protect user devices and files</span></span>

<span data-ttu-id="5484a-150">Nyt kun Microsoft 365 Business -käyttöoikeudet on määritetty, aloita laitteiden ja tiedostojen suojaaminen noudattamalla ohjeita.</span><span class="sxs-lookup"><span data-stu-id="5484a-150">Now that Microsoft 365 Business licenses have been assigned, complete steps to start protecting devices and files.</span></span> <span data-ttu-id="5484a-151">Voit käyttää joitakin hallintakeskuksen siirtymisruudun uusia asetuksia.</span><span class="sxs-lookup"><span data-stu-id="5484a-151">You'll use some new options included in the admin center navigation pane.</span></span>
  
1. <span data-ttu-id="5484a-152">Siirry hallintakeskuksen siirtymisruudussa **Kohtaan Laitekäytännöt** \> \*\*\*\*.</span><span class="sxs-lookup"><span data-stu-id="5484a-152">In the admin center, in the navigation pane, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="5484a-153">Valitse **Laitekäytännöt-sivulla** **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="5484a-153">On the **Device policies** page, select **Add**.</span></span>
    
3. <span data-ttu-id="5484a-154">Anna \*\*\*\* käytännölle nimi (esimerkiksi Suojaa työtiedostot) ja valitse sitten **käytäntötyyppi** avattavasta luettelosta.</span><span class="sxs-lookup"><span data-stu-id="5484a-154">In the **Add policy** pane give the policy a name (for example, Protect work files), and then choose a **Policy type** from the drop-down list.</span></span> 
    
    <span data-ttu-id="5484a-155">Voit määrittää sovelluskäytäntöjä tiedostojen suojaamiseksi Android- ja iPhone-laitteissa sekä Windows 10:ssä ja määrittää laitteen määrityskäytännöt yrityksen omistamille Windows 10 -laitteille.</span><span class="sxs-lookup"><span data-stu-id="5484a-155">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="5484a-156">Lisätietoja on seuraavissa linkeissä:</span><span class="sxs-lookup"><span data-stu-id="5484a-156">See the following links for details:</span></span>
    
  - [<span data-ttu-id="5484a-157">Sovellusten suojausasetusten määrittäminen Android- tai iOS-laitteita varten</span><span class="sxs-lookup"><span data-stu-id="5484a-157">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="5484a-158">Sovellusten suojausasetusten määrittäminen Windows 10 -laitteille</span><span class="sxs-lookup"><span data-stu-id="5484a-158">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="5484a-159">Laitesuojausasetusten määrittäminen Windows 10 -tietokoneille</span><span class="sxs-lookup"><span data-stu-id="5484a-159">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
    
  
4. <span data-ttu-id="5484a-160">Kun olet määrittänyt käytännöt, sinä ja työntekijäsi voitte määrittää laitteita:</span><span class="sxs-lookup"><span data-stu-id="5484a-160">After you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="5484a-161">Jos Windows-laitteesi eivät vielä käytä Windows Pro Creator -päivitystä, sinun on [päivitettävä ne Windows Pro Creators Updateksi](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="5484a-161">If your Windows devices aren't already using the Windows Pro Creator update, you'll need to [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
    
  - <span data-ttu-id="5484a-162">Lisätietoja Windows-laitteiden vaiheista [on ohjeaiheessa Windows-laitteiden määrittäminen Microsoft 365 Business -käyttäjille.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="5484a-162">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="5484a-163">Lisätietoja Android-puhelimista ja [iPhoneista on ohjeaiheessa Mobiililaitteiden määrittäminen Microsoft 365 Business -käyttäjille.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="5484a-163">See [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
