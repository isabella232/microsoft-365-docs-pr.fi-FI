---
title: Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa
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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Lue tietoja Microsoft 365 Business -sovellusten suojausasetusten tarkistamisesta Windows 10 -laitteissa.
ms.openlocfilehash: 577921f7f33eafbbe652dcf825a145d89f1ff556
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2020
ms.locfileid: "42057213"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="928e9-103">Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa</span><span class="sxs-lookup"><span data-stu-id="928e9-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="928e9-104">Sen tarkistaminen, että käyttäjät eivät voi kopioida yritystietoja yrityksen laitteiden henkilökohtaisiin tiedostoihin</span><span class="sxs-lookup"><span data-stu-id="928e9-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="928e9-105">Kun olet [määrittänyt sovellusten suojauskäytännöt](protection-settings-for-windows-10-devices.md), saattaa kestää muutama tunti, ennen kuin käytäntöä sovelletaan käyttäjien laitteissa.</span><span class="sxs-lookup"><span data-stu-id="928e9-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="928e9-106">Jos olet ottanut **Käyttöön** **Estä käyttäjiä kopioimasta yrityksen tietoja henkilökohtaisiin tiedostoihin ja pakottanut heidät tallentamaan työtiedostot Yrityksen** omistamien laitteiden OneDrive for Business -asetukseen, voit tarkistaa tämän käyttäjän laitteesta sen jälkeen, kun he ovat muodostaneet yhteyden Azure AD:hen ja kirjautunut sisään.</span><span class="sxs-lookup"><span data-stu-id="928e9-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="928e9-107">**Yhteysasetusten tarkistaminen**</span><span class="sxs-lookup"><span data-stu-id="928e9-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="928e9-p102">Kun olet kirjautunut sisään Microsoft 365 Business -tunnistetiedoilla ja muodostanut yhteyden Azure AD:hen [Windows-laitteiden määrittäminen Microsoft 365 Business -käyttäjille](set-up-windows-devices.md) -kohdassa kuvatun mukaisesti, siirry kohtaan **Windowsin asetukset** \> **Tilit** \> **Käytä työpaikan tai oppilaitoksen tiliä**. Valitse **Yhteys muodostettu \<vuokraajan nimi\> Azure AD:hen** ja valitse sitten **Tiedot**.</span><span class="sxs-lookup"><span data-stu-id="928e9-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="928e9-111">**Hallitut** \<vuokraajan\> nimi -sivulla on **Yhteystiedot,** jotka sisältävät **hallintapalvelimen osoitteen,** kuten seuraavassa kuvassa.</span><span class="sxs-lookup"><span data-stu-id="928e9-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="928e9-113">**Yrityksen tietojen liittämisen ei-hallittuun sovellukseen ei onnistu**</span><span class="sxs-lookup"><span data-stu-id="928e9-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="928e9-114">Avaa Outlook 2016, jonka on asentanut Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="928e9-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="928e9-115">Avaa sähköpostiviesti ja kopioi siitä jotakin sisältöä.</span><span class="sxs-lookup"><span data-stu-id="928e9-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="928e9-116">Avaa Muistio ja yritä sitten liittää sisältö siihen.</span><span class="sxs-lookup"><span data-stu-id="928e9-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="928e9-117">Saat virheen, jonka mukaan sovellus ei voi käyttää sisältöä.</span><span class="sxs-lookup"><span data-stu-id="928e9-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="928e9-119">Voit kuitenkin liittää saman sisällön Word 2016:een.</span><span class="sxs-lookup"><span data-stu-id="928e9-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="928e9-120">Sen tarkistaminen, että käyttäjät eivät voi kopioida yritystietoja henkilökohtaisten laitteiden henkilökohtaisiin tiedostoihin</span><span class="sxs-lookup"><span data-stu-id="928e9-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="928e9-121">**Yhteysasetusten tarkistaminen**</span><span class="sxs-lookup"><span data-stu-id="928e9-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="928e9-122">Siirry Windows 10:n henkilökohtaiseen laitteeseen, johon olet kirjautunut paikallisena käyttäjänä, **Windowsin asetukset**ja valitse **Tilit** \> **Accessin työ tai koulu**.</span><span class="sxs-lookup"><span data-stu-id="928e9-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="928e9-123">Valitse **Käytä työpaikan tai oppilaitoksen tiliä** -kohdasta **Yhdistä**.</span><span class="sxs-lookup"><span data-stu-id="928e9-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="928e9-124">Kirjoita Microsoft 365 Business -tunnistetietosi **Määritä työpaikan tai oppilaitoksen tili -valintaikkunaan** \> **Kirjaudu sisään**.</span><span class="sxs-lookup"><span data-stu-id="928e9-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="928e9-125">Valitse **Käytä työpaikan tai oppilaitoksen tiliä** -sivulla **Työpaikan tai oppilaitoksen tili** ja valitse sitten **Tiedot**.</span><span class="sxs-lookup"><span data-stu-id="928e9-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Napsauta tai napauta Tietoja Työ- tai koulutili -valintaikkunassa.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="928e9-127">**Accessin työ- tai koulusivulla** on **yhteystiedot,** jotka sisältävät **hallintapalvelimen osoitteen,** kuten seuraavassa \*\* kuvassa näkyvä \*\* ns.</span><span class="sxs-lookup"><span data-stu-id="928e9-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="928e9-129">**Yrityksen tietojen liittämisen ei-hallittuun sovellukseen ei onnistu**</span><span class="sxs-lookup"><span data-stu-id="928e9-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="928e9-130">Avaa Outlook 2016 ja lisää tarvittaessa Microsoft 365 Business -tilisi ja kirjaudu sisään Microsoft 365 Business -tunnistetiedoillasi.</span><span class="sxs-lookup"><span data-stu-id="928e9-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="928e9-131">Avaa sähköpostiviesti ja kopioi siitä jotakin sisältöä.</span><span class="sxs-lookup"><span data-stu-id="928e9-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="928e9-132">Avaa Muistio ja yritä sitten liittää sisältö siihen.</span><span class="sxs-lookup"><span data-stu-id="928e9-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="928e9-133">Saat virheen, jonka mukaan sovellus ei voi käyttää sisältöä.</span><span class="sxs-lookup"><span data-stu-id="928e9-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="928e9-135">Voit kuitenkin liittää saman sisällön Word 2016:een.</span><span class="sxs-lookup"><span data-stu-id="928e9-135">You can, however, paste the same content into Word 2016.</span></span>
    

