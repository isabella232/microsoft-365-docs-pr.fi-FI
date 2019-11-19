---
title: Lisää uhkien suojausta Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
description: Määritä yhteensopivuus ominaisuuksia tietojen menettämisen estämiseksi ja arkaluonteisten tietojen otsikoiksi.
ms.openlocfilehash: 6fae95e8c5e6d133e3163dbdfd3c09cfede11382
ms.sourcegitcommit: 5d11f516e78ea4a74145e19ba2300f0792c8bac1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/19/2019
ms.locfileid: "38715118"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="95e5b-103">Yhteensopivuus ominaisuuksien määrittäminen</span><span class="sxs-lookup"><span data-stu-id="95e5b-103">Set up compliance features</span></span>

<span data-ttu-id="95e5b-104">Microsoft 365-yritys sisältää ominaisuuksia, jotka suojaavat tietojasi ja laitteitasi sekä auttavat pitämään omasi ja asiakkaidesi arkaluonteiset tiedot turvassa.</span><span class="sxs-lookup"><span data-stu-id="95e5b-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="95e5b-105">DLP-ominaisuuksien määrittäminen</span><span class="sxs-lookup"><span data-stu-id="95e5b-105">Set up DLP features</span></span>

<span data-ttu-id="95e5b-106">Katso [Luo DLP-käytäntö mallista](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) esimerkkinä siitä, miten voit määrittää käytännön suojaamaan henkilökohtaisia tunniste tietoja (pii) vastaan.</span><span class="sxs-lookup"><span data-stu-id="95e5b-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="95e5b-107">DLP sisältää monia valmiita käytäntö malleja monille eri kieli alueilla.</span><span class="sxs-lookup"><span data-stu-id="95e5b-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="95e5b-108">Esimerkiksi Australian taloudelliset tiedot, Kanadan henkilö tieto laki, Yhdysvaltain taloudelliset tiedot ja niin vielä.</span><span class="sxs-lookup"><span data-stu-id="95e5b-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="95e5b-109">Katso, [mitä DLP-käytäntö mallit sisältävät](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) täydellisestä luettelosta.</span><span class="sxs-lookup"><span data-stu-id="95e5b-109">See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="95e5b-110">Kaikki nämä mallit voidaan ottaa käyttöön samanlaisiksi kuin PII-malli esimerkki.</span><span class="sxs-lookup"><span data-stu-id="95e5b-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="95e5b-111">Sähkö postin säilyttämisen määrittäminen Exchange Online-arkistoinnin avulla</span><span class="sxs-lookup"><span data-stu-id="95e5b-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="95e5b-112">**Exchange Online-arkistointi** lisenssi ominaisuudet auttavat ylläpitämään yhteensopivuus-ja sääntely standardeja säilyttämällä Sähkö posti sisällön eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="95e5b-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="95e5b-113">Se myös auttaa vähentämään riskiä, jos on oikeus juttu, ja tarjoaa tapa palauttaa tietoja, kun tieto turva loukkaus tai kun haluat palauttaa poistetut kohteet.</span><span class="sxs-lookup"><span data-stu-id="95e5b-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="95e5b-114">Voit säilyttää kaikki käyttäjän sisällöt tai käyttää säilytys käytäntöjä, kun haluat muokata säilytetä.</span><span class="sxs-lookup"><span data-stu-id="95e5b-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="95e5b-115">**Oikeuden käyntien pito:** Voit säilyttää kaiken posti laatikon sisällön, mukaan lukien poistetut kohteet, asettamalla käyttäjän koko posti laatikon oikeus riita-asioihin.</span><span class="sxs-lookup"><span data-stu-id="95e5b-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="95e5b-116">Voit sijoittaa posti laatikon oikeuden käyntiin pitämällä hallinta keskuksessa:</span><span class="sxs-lookup"><span data-stu-id="95e5b-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="95e5b-117">Siirry vasemmassa siirtymis osassa **käyttäjät** \> **aktiiviset käyttäjät**-kohtaan.</span><span class="sxs-lookup"><span data-stu-id="95e5b-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="95e5b-118">Valitse käyttäjä, jonka posti laatikon haluat sijoittaa riita-asioihin.</span><span class="sxs-lookup"><span data-stu-id="95e5b-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="95e5b-119">Laajenna käyttäjä ruudussa **mailin asetukset**ja valitse **Lisää asetuksia**-kohdasta **Muokkaa Exchangen ominaisuuksia**.</span><span class="sxs-lookup"><span data-stu-id="95e5b-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="95e5b-120">Valitse käyttäjän posti laatikko-sivulla \* \* posti laatikon ominaisuudet \* \* vasemmassa NAV-ohjelmassa ja valitse sitten **Ota käyttöön** -linkki kohdassa **oikeuden käynti pito**.</span><span class="sxs-lookup"><span data-stu-id="95e5b-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="95e5b-121">Voit määrittää **oikeuden käynnin pito-valinta ikkunassa** oikeuden käyntien keston **oikeuden käynnin** keston kentässä.</span><span class="sxs-lookup"><span data-stu-id="95e5b-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="95e5b-122">Jätä kenttä tyhjäksi, jos haluat sijoittaa äärettömän pito-arvon.</span><span class="sxs-lookup"><span data-stu-id="95e5b-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="95e5b-123">Voit myös lisätä muistiinpanoja ja ohjata posti laatikon omistajaa verkkosivustolle, jota saatat joutua selittämään lisää riita-asioiden pito paikasta.</span><span class="sxs-lookup"><span data-stu-id="95e5b-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="95e5b-124">\>**Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="95e5b-124">\> **Save**.</span></span>
    
<span data-ttu-id="95e5b-125">**Säilyttäminen:** Voit ottaa käyttöön mukautetut säilytys käytännöt, esimerkiksi säilyttää tietyn ajan tai poistaa sisällön pysyvästi säilytys ajan päätyttyä.</span><span class="sxs-lookup"><span data-stu-id="95e5b-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="95e5b-126">Lisä tietoja [on kohdassa säilytys käytäntöjen yleiskatsaus](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="95e5b-126">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="95e5b-127">Määritä herkkyys otsikot</span><span class="sxs-lookup"><span data-stu-id="95e5b-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="95e5b-128">Herkkyys tunnisteissa on Azure Information Protection (AIP)-suunnitelma 1, ja ne auttavat luokittelemaan ja valinnaisesti suojaamaan asia kirjasi ja sähkö postit käyttämällä tunnisteita.</span><span class="sxs-lookup"><span data-stu-id="95e5b-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="95e5b-129">Järjestelmänvalvojat voivat käyttää otsikoita automaattisesti, jos käyttäjät määrittävät säännöt ja ehdot manuaalisesti, tai käyttämällä yhdistelmää, jossa käyttäjille annetaan suosituksia.</span><span class="sxs-lookup"><span data-stu-id="95e5b-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="95e5b-130">Jos haluat määrittää herkkyys otsikot, katso [Luo ja hallitse herkkyys tarroja](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span><span class="sxs-lookup"><span data-stu-id="95e5b-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="95e5b-131">Azure-tieto suoja asiakkaan asentaminen manuaalisesti</span><span class="sxs-lookup"><span data-stu-id="95e5b-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="95e5b-132">Voit asentaa AIP-asiakkaan manuaalisesti:</span><span class="sxs-lookup"><span data-stu-id="95e5b-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="95e5b-133">Lataa **AzinfoProtection_UL. exe** [Microsoft Download Centeristä](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="95e5b-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="95e5b-134">Voit varmistaa, että asennus on toiminut tarkastelemalla Word-asia kirjaa ja varmistamalla, että **herkkyys** asetus on käytettävissä **Aloitus** -väli lehdellä.</span><span class="sxs-lookup"><span data-stu-id="95e5b-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="95e5b-135">![Word-asia kirjan avattava suojaus-väli lehti.](media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="95e5b-135">![Protection tab drop-down in a Word document.](media/word-sensitivity.png)</span></span>

<span data-ttu-id="95e5b-136">Lisä tietoja on kohdassa [Asenna asiakas](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="95e5b-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
