---
title: Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Vahvista Microsoft 365 Business Premium -sovelluksen suojausasetukset Windows 10 -laitteissa ja varmista, että käyttäjät eivät voi kopioida yritystietoja henkilökohtaisiin tiedostoihin tai ei-hallittuihin sovelluksiin.
ms.openlocfilehash: e319ffa5149f055b5de45078facc8899acffc223
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579858"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="f97c2-103">Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa</span><span class="sxs-lookup"><span data-stu-id="f97c2-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="f97c2-104">Sen tarkistaminen, että käyttäjät eivät voi kopioida yritystietoja yrityksen laitteiden henkilökohtaisiin tiedostoihin</span><span class="sxs-lookup"><span data-stu-id="f97c2-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="f97c2-105">Kun olet [määrittänyt sovellusten suojauskäytännöt](protection-settings-for-windows-10-devices.md), saattaa kestää muutama tunti, ennen kuin käytäntöä sovelletaan käyttäjien laitteissa.</span><span class="sxs-lookup"><span data-stu-id="f97c2-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="f97c2-106">Jos olet **ottanut Estä** käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin ja pakotit heidät tallentamaan työtiedostot Yrityksen omistamien laitteiden **OneDrive for Business** -asetukseen, voit tarkistaa tämän käyttäjän laitteessa, kun käyttäjä on muodostanut yhteyden Azure AD:hen ja kirjautunut sisään.</span><span class="sxs-lookup"><span data-stu-id="f97c2-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="f97c2-107">**Yhteysasetusten tarkistaminen**</span><span class="sxs-lookup"><span data-stu-id="f97c2-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="f97c2-108">Kun olet kirjautunut Sisään Microsoft 365 Business Premium -tunnistetiedoilla ja muodostanut yhteyden Azure AD:seen [artikkelissa Windows-laitteiden määrittäminen Microsoft 365 Business Premium](set-up-windows-devices.md)-käyttäjille kuvatulla tavalla, siirry **Windows-asetusten** tileihin, jotka ovat käytössä töissä \>  \> **tai oppilaitoksessa.**</span><span class="sxs-lookup"><span data-stu-id="f97c2-108">After you sign in with Microsoft 365 Business Premium credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**.</span></span> <span data-ttu-id="f97c2-109">Valitse **Yhdistetty \<tenant name\> Azure AD:en** ja valitse **sitten Tiedot.**</span><span class="sxs-lookup"><span data-stu-id="f97c2-109">Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="f97c2-111">**Hallittu-sivulla** näet hallintapalvelimen osoitteen sisältävät yhteystiedot seuraavassa kuvassa \<tenant name\>  esitetyllä tavalla. </span><span class="sxs-lookup"><span data-stu-id="f97c2-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="f97c2-113">**Varmista, että yritystietoja ei voi liittää ei-hallittavaan sovellukseen**</span><span class="sxs-lookup"><span data-stu-id="f97c2-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="f97c2-114">Avaa Microsoft 365 Business Premiumin asentama Outlook 2016.</span><span class="sxs-lookup"><span data-stu-id="f97c2-114">Open Outlook 2016 that was installed by Microsoft 365 Business Premium.</span></span>
    
2. <span data-ttu-id="f97c2-115">Avaa sähköpostiviesti ja kopioi siitä jotakin sisältöä.</span><span class="sxs-lookup"><span data-stu-id="f97c2-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="f97c2-116">Avaa Muistio ja yritä sitten liittää sisältö siihen.</span><span class="sxs-lookup"><span data-stu-id="f97c2-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="f97c2-117">Näyttöön tulee virheilmoitus, jossa todetaan, että sovellus ei voi käyttää sisältöä.</span><span class="sxs-lookup"><span data-stu-id="f97c2-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="f97c2-119">Voit kuitenkin liittää saman sisällön Word 2016:een.</span><span class="sxs-lookup"><span data-stu-id="f97c2-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="f97c2-120">Sen tarkistaminen, että käyttäjät eivät voi kopioida yritystietoja henkilökohtaisten laitteiden henkilökohtaisiin tiedostoihin</span><span class="sxs-lookup"><span data-stu-id="f97c2-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="f97c2-121">**Yhteysasetusten tarkistaminen**</span><span class="sxs-lookup"><span data-stu-id="f97c2-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="f97c2-122">Siirry henkilökohtaisessa Windows 10 -laitteessasi, jossa olet kirjautunut sisään paikallisena käyttäjänä, **Windows-asetukset** ja valitse **sitten Tilien** käyttö töissä \> **tai oppilaitoksessa.**</span><span class="sxs-lookup"><span data-stu-id="f97c2-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="f97c2-123">Valitse **Käytä työpaikan tai oppilaitoksen tiliä** -kohdasta **Yhdistä**.</span><span class="sxs-lookup"><span data-stu-id="f97c2-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="f97c2-124">Anna Microsoft 365 Business Premium -tunnistetietosi Määritä työ- tai koulutili **-valintaikkunaan** \> **Kirjaudu sisään.**</span><span class="sxs-lookup"><span data-stu-id="f97c2-124">Enter your Microsoft 365 Business Premium credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="f97c2-125">Valitse **Käytä työpaikan tai oppilaitoksen tiliä** -sivulla **Työpaikan tai oppilaitoksen tili** ja valitse sitten **Tiedot**.</span><span class="sxs-lookup"><span data-stu-id="f97c2-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Napsauta tai napauta Tiedot Työ- tai koulutili -valintaikkunassa.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="f97c2-127">Accessin **työ-** tai koulusivulla  näet yhteystiedot, jotka sisältävät **hallintapalvelimen** osoitteen, kuten seuraavassa kuvassa, ja sisältää sanat *wip* and *mam* within.</span><span class="sxs-lookup"><span data-stu-id="f97c2-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="f97c2-129">**Varmista, että yritystietoja ei voi liittää ei-hallittavaan sovellukseen**</span><span class="sxs-lookup"><span data-stu-id="f97c2-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="f97c2-130">Avaa Outlook 2016, lisää Tarvittaessa Microsoft 365 Business Premium -tili ja kirjaudu sisään Microsoft 365 Business Premium -tunnistetiedoillasi.</span><span class="sxs-lookup"><span data-stu-id="f97c2-130">Open Outlook 2016 and add your Microsoft 365 Business Premium account if necessary and sign in with your Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="f97c2-131">Avaa sähköpostiviesti ja kopioi siitä jotakin sisältöä.</span><span class="sxs-lookup"><span data-stu-id="f97c2-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="f97c2-132">Avaa Muistio ja yritä sitten liittää sisältö siihen.</span><span class="sxs-lookup"><span data-stu-id="f97c2-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="f97c2-133">Näyttöön tulee virhesanoma, jonka mukaan Sovellus ei voi käyttää sisältöä.</span><span class="sxs-lookup"><span data-stu-id="f97c2-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="f97c2-135">Voit kuitenkin liittää saman sisällön Word 2016:een.</span><span class="sxs-lookup"><span data-stu-id="f97c2-135">You can, however, paste the same content into Word 2016.</span></span>
    

