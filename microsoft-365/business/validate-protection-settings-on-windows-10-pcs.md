---
title: Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Opettele tarkistaa Microsoft 365 Business app suojausasetukset Windows 10-laitteet.
ms.openlocfilehash: f00dd380103ad9498d77b0e8814bace3de168df4
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983293"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="6a448-103">Sovellusten suojausasetusten vahvistaminen Windows 10 -tietokoneissa</span><span class="sxs-lookup"><span data-stu-id="6a448-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="6a448-104">Sen tarkistaminen, että käyttäjät eivät voi kopioida yritystietoja yrityksen laitteiden henkilökohtaisiin tiedostoihin</span><span class="sxs-lookup"><span data-stu-id="6a448-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="6a448-p101">Kun olet [määrittänyt sovellusten suojauskäytännöt](protection-settings-for-windows-10-devices.md), saattaa kestää muutama tunti, ennen kuin käytäntöä sovelletaan käyttäjien laitteissa. Jos olet ottanut **käyttöön** **Estä käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin ja pakota heidät tallentamaan työtiedostot OneDrive for Businessiin** -asetuksen yrityksen omistamille laitteille, voit valita tämän käyttäjän laitteessa, kun käyttäjä on muodostanut yhteyden Azure AD:hen ja kirjautunut sisään.</span><span class="sxs-lookup"><span data-stu-id="6a448-p101">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices. If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they have connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="6a448-107">**Yhteysasetusten tarkistaminen**</span><span class="sxs-lookup"><span data-stu-id="6a448-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="6a448-p102">Kun olet kirjautunut sisään Microsoft 365 Business -tunnistetiedoilla ja muodostanut yhteyden Azure AD:hen [Windows-laitteiden määrittäminen Microsoft 365 Business -käyttäjille](set-up-windows-devices.md) -kohdassa kuvatun mukaisesti, siirry kohtaan **Windowsin asetukset** \> **Tilit** \> **Käytä työpaikan tai oppilaitoksen tiliä**. Valitse **Yhteys muodostettu \<vuokraajan nimi\> Azure AD:hen** ja valitse sitten **Tiedot**.</span><span class="sxs-lookup"><span data-stu-id="6a448-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="6a448-111">Voit nähdä **Hallinnoija** \<vuokraajan nimi\> -sivulla **yhteystiedot**, jotka sisältävät **hallintapalvelimen osoitteen** seuraavassa kuvassa näytetyn mukaisesti.</span><span class="sxs-lookup"><span data-stu-id="6a448-111">On the **Managed by** \<tenant name\> page you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="6a448-113">**Sen tarkistaminen, ettet voi liittää yritystietoja hallinnoimattomaan sovellukseen**</span><span class="sxs-lookup"><span data-stu-id="6a448-113">**Verify that you cannot paste company data to a non-managed app**</span></span>
  
1. <span data-ttu-id="6a448-114">Avaa Outlook 2016, jonka on asentanut Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="6a448-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="6a448-115">Avaa sähköpostiviesti ja kopioi siitä jotakin sisältöä.</span><span class="sxs-lookup"><span data-stu-id="6a448-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="6a448-116">Avaa Muistio ja yritä sitten liittää sisältö siihen.</span><span class="sxs-lookup"><span data-stu-id="6a448-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="6a448-117">Saat virheilmoituksen, jonka mukaan sovellus ei voi näyttää sisältöä.</span><span class="sxs-lookup"><span data-stu-id="6a448-117">You will receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="6a448-119">Voit kuitenkin liittää saman sisällön Word 2016:een.</span><span class="sxs-lookup"><span data-stu-id="6a448-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="6a448-120">Sen tarkistaminen, että käyttäjät eivät voi kopioida yritystietoja henkilökohtaisten laitteiden henkilökohtaisiin tiedostoihin</span><span class="sxs-lookup"><span data-stu-id="6a448-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="6a448-121">**Yhteysasetusten tarkistaminen**</span><span class="sxs-lookup"><span data-stu-id="6a448-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="6a448-122">Siirry henkilökohtaisessa Windows 10 -laitteessa, johon olet kirjautunut sisään paikallisena käyttäjänä, **Windowsin asetukset** -kohtaan, ja napsauta tai napauta **Tilit** \> **Käytä työpaikan tai oppilaitoksen tiliä**.</span><span class="sxs-lookup"><span data-stu-id="6a448-122">On your Windows 10 personal device where you are logged in as a local user, go to **Windows Settings** and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="6a448-123">Valitse **Käytä työpaikan tai oppilaitoksen tiliä** -kohdasta **Yhdistä**.</span><span class="sxs-lookup"><span data-stu-id="6a448-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="6a448-124">Kirjoita Microsoft 365 Business -tunnistetietosi **Määritä työpaikan tai oppilaitoksen tili -valintaikkunaan** \> **Kirjaudu sisään**.</span><span class="sxs-lookup"><span data-stu-id="6a448-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="6a448-125">Valitse **Käytä työpaikan tai oppilaitoksen tiliä** -sivulla **Työpaikan tai oppilaitoksen tili** ja valitse sitten **Tiedot**.</span><span class="sxs-lookup"><span data-stu-id="6a448-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Work or school account dalog.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="6a448-127">Voit nähdä **Käytä työpaikan tai oppilaitoksen tiliä** -sivulla **yhteystiedot**, jotka sisältävät **hallintapalvelimen osoitteen** seuraavassa kuvassa näytetyn mukaisesti sekä  *wip*  - ja  *mam*  -sanat.</span><span class="sxs-lookup"><span data-stu-id="6a448-127">On the **Access work or school** page you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="6a448-129">**Sen tarkistaminen, ettet voi liittää yritystietoja hallinnoimattomaan sovellukseen**</span><span class="sxs-lookup"><span data-stu-id="6a448-129">**Verify that you cannot paste company data to a non-managed app**</span></span>
  
1. <span data-ttu-id="6a448-130">Avaa Outlook 2016 ja lisää tarvittaessa Microsoft 365 Business -tilisi ja kirjaudu sisään Microsoft 365 Business -tunnistetiedoillasi.</span><span class="sxs-lookup"><span data-stu-id="6a448-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="6a448-131">Avaa sähköpostiviesti ja kopioi siitä jotakin sisältöä.</span><span class="sxs-lookup"><span data-stu-id="6a448-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="6a448-132">Avaa Muistio ja yritä sitten liittää sisältö siihen.</span><span class="sxs-lookup"><span data-stu-id="6a448-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="6a448-133">Saat virheilmoituksen, jonka mukaan sovellus ei voi näyttää sisältöä.</span><span class="sxs-lookup"><span data-stu-id="6a448-133">You will receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="6a448-135">Voit kuitenkin liittää saman sisällön Word 2016:een.</span><span class="sxs-lookup"><span data-stu-id="6a448-135">You can, however, paste the same content into Word 2016.</span></span>
    

