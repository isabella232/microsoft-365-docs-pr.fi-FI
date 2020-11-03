---
title: Paranna Microsoft 365 Business Premiumin uhkien suojausta
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
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Määritä yhteensopivuus ominaisuudet, jotka estävät tietojen menettämisen ja auttavat pitämään asiakkaiden luottamukselliset tiedot turvassa.
ms.openlocfilehash: 2c95ad3f36df28af2c68cd11192bcfe92dfe29e3
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841169"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="cb228-103">Yhteensopivuus ominaisuuksien määrittäminen</span><span class="sxs-lookup"><span data-stu-id="cb228-103">Set up compliance features</span></span>

<span data-ttu-id="cb228-104">Microsoft 365 Business Premiumin ominaisuuksiin kuuluu tietojen ja laitteiden suojaaminen, ja sen avulla voit pitää asiakkaidemme luottamukselliset tiedot turvassa.</span><span class="sxs-lookup"><span data-stu-id="cb228-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="cb228-105">DLP-ominaisuuksien määrittäminen</span><span class="sxs-lookup"><span data-stu-id="cb228-105">Set up DLP features</span></span>

<span data-ttu-id="cb228-106">Lisä tietoja on kohdassa [DLP-käytäntöjen luominen mallista](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) , jossa on esimerkki käytännöstä, jonka avulla voit suoja utua henkilökohtaisten tietojen menettämisen varalta.</span><span class="sxs-lookup"><span data-stu-id="cb228-106">See [Create a DLP policy from a template](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="cb228-107">DLP sisältää monia käyttövalmiita käytäntöjen malleja useille eri kieli alueille.</span><span class="sxs-lookup"><span data-stu-id="cb228-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="cb228-108">Esimerkiksi Australian taloudelliset tiedot, Kanadan henkilö tieto laki, USA:n taloudelliset tiedot ja niin edelleen.</span><span class="sxs-lookup"><span data-stu-id="cb228-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="cb228-109">Katso [, mitä DLP-käytännöt sisältävät](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) täydellisen luettelon.</span><span class="sxs-lookup"><span data-stu-id="cb228-109">See [What the DLP policy templates include](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) for a full list.</span></span> <span data-ttu-id="cb228-110">Kaikki nämä mallit voidaan ottaa käyttöön vastaavalla tavalla kuin PII-malli esimerkki.</span><span class="sxs-lookup"><span data-stu-id="cb228-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="cb228-111">Sähkö postin säilytyksen määrittäminen Exchange Online-arkistoinnin avulla</span><span class="sxs-lookup"><span data-stu-id="cb228-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="cb228-112">**Exchange Onlinen arkistoinnin** käyttö oikeus ominaisuuksien avulla voit ylläpitää yhteensopivuus-ja säännös standardeja säilyttämällä sähkö postin sisällön eDiscoveryyn.</span><span class="sxs-lookup"><span data-stu-id="cb228-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="cb228-113">Se myös vähentää riskiä, jos kyseessä on oikeus juttu, ja sen avulla voit palauttaa tietoja, kun tieto turva on rikottu tai kun sinun on palautettava poistetut kohteet.</span><span class="sxs-lookup"><span data-stu-id="cb228-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="cb228-114">Voit käyttää oikeus toimiin liittyvään pitoon, jos haluat säilyttää kaikki käyttäjän sisällöt, tai käyttää säilytys käytäntöjä, jotka mukauttavat säilytettävän sisällön.</span><span class="sxs-lookup"><span data-stu-id="cb228-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="cb228-115">**Oikeus toimiin liittyvään pitoon:** Voit säilyttää kaikki posti laatikon sisältö, mukaan lukien poistetut kohteet, asettamalla käyttäjän koko posti laatikon oikeus toimiin liittyvään pitoon.</span><span class="sxs-lookup"><span data-stu-id="cb228-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="cb228-116">Jos haluat sijoittaa posti laatikon oikeus toimiin liittyvään pitoon, valitse hallinta keskuksessa:</span><span class="sxs-lookup"><span data-stu-id="cb228-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="cb228-117">Valitse vasemmanpuoleisessa siirtymis ruudussa **käyttäjät** \> **aktiiviset käyttäjät**.</span><span class="sxs-lookup"><span data-stu-id="cb228-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="cb228-118">Valitse käyttäjä, jonka posti laatikon haluat sijoittaa oikeus toimiin liittyvään pitoon.</span><span class="sxs-lookup"><span data-stu-id="cb228-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="cb228-119">Laajenna käyttäjä ruudussa **Sähkö posti asetukset** ja valitse **lisä asetukset** -kohdan vierestä **Muokkaa Exchangen ominaisuuksia**.</span><span class="sxs-lookup"><span data-stu-id="cb228-119">In the user pane, expand **Mail settings** , and next to **More settings** , choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="cb228-120">Valitse käyttäjän posti laatikko-sivulla \* \* posti laatikon ominaisuudet \* \* vasemmassa siirtymis ruudussa ja valitse sitten **Ota käyttöön** -linkki **oikeus toimiin liittyvään pitoon**.</span><span class="sxs-lookup"><span data-stu-id="cb228-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="cb228-121">Oikeus toimiin liittyvän **pidon** valinta ikkunassa voit määrittää oikeus toimiin liittyvän pidon keston **oikeus toimiin liittyvän pidon kesto** -kentässä.</span><span class="sxs-lookup"><span data-stu-id="cb228-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="cb228-122">Jätä kenttä tyhjäksi, jos haluat sijoittaa äärettömään pitoon.</span><span class="sxs-lookup"><span data-stu-id="cb228-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="cb228-123">Voit myös lisätä muistiinpanoja ja ohjata posti laatikon omistajan sivustoon, josta sinun on ehkä selitettävä lisää oikeus toimiin liittyvästä pidosta.</span><span class="sxs-lookup"><span data-stu-id="cb228-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="cb228-124">\>**Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="cb228-124">\> **Save**.</span></span>
    
<span data-ttu-id="cb228-125">**Säilyttäminen:** Voit ottaa käyttöön mukautetut säilytys käytännöt, jotka esimerkiksi säilyttävät tietyn ajan tai poistavat sisältöä pysyvästi säilytys ajan päätyttyä.</span><span class="sxs-lookup"><span data-stu-id="cb228-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="cb228-126">Lisä tietoja on artikkelissa [säilytys käytäntöjen yleiskatsaus](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span><span class="sxs-lookup"><span data-stu-id="cb228-126">To learn more, see [Overview of retention policies](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="cb228-127">Luottamuksellisuusmerkkien määrittäminen</span><span class="sxs-lookup"><span data-stu-id="cb228-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="cb228-128">Herkkyys selitteissä on Azure Information Protectionin (AIP) sopimus 1, ja niiden avulla voit luokitella ja halutessasi suojata asia kirjoja ja sähkö posteja käyttämällä otsikoita.</span><span class="sxs-lookup"><span data-stu-id="cb228-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="cb228-129">Käyttäjät voivat ottaa nimiöt automaattisesti käyttöön, jotka määrittävät säännöt ja ehdot manuaalisesti käyttäjiltä tai käyttämällä yhdistelmää, jossa käyttäjille annetaan suosituksia.</span><span class="sxs-lookup"><span data-stu-id="cb228-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="cb228-130">Voit määrittää herkkyys otsikoita valitsemalla [Luo ja hallitse luottamuksellisuusotsikoita](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) -video.</span><span class="sxs-lookup"><span data-stu-id="cb228-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="cb228-131">Azure Information Protectionin asiakas ohjelman asentaminen manuaalisesti</span><span class="sxs-lookup"><span data-stu-id="cb228-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="cb228-132">Jos haluat asentaa AIP-asiakas ohjelman manuaalisesti, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="cb228-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="cb228-133">Lataa **AzinfoProtection_UL.exe** [Microsoft Download Centeristä](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="cb228-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="cb228-134">Voit varmistaa, että asennus onnistui tarkastelemalla Word-asia kirjaa ja varmistamalla, että **herkkyys** -vaihto ehto on käytettävissä **Aloitus** -väli lehdessä.</span><span class="sxs-lookup"><span data-stu-id="cb228-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="cb228-135">![Word-asia kirjan avattava suojaus-väli lehti.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="cb228-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="cb228-136">Lisä tietoja on Ohje aiheessa [asiakas ohjelman asentaminen](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="cb228-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
