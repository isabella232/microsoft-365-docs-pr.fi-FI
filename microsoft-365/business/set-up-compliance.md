---
title: Lisää Microsoft 365 Business Premiumin uhkasuojausta
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
description: Määritä yhteensopivuusominaisuudet, jotka estävät tietojen häviämisen ja auttavat pitämään asiakkaiden ja asiakkaidesi arkaluonteiset tiedot turvassa.
ms.openlocfilehash: 9b900367c22ec5bb5c2719af63049045ecd5e466
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/27/2020
ms.locfileid: "44402690"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="5c04c-103">Yhteensopivuusominaisuuksien määrittäminen</span><span class="sxs-lookup"><span data-stu-id="5c04c-103">Set up compliance features</span></span>

<span data-ttu-id="5c04c-104">Microsoft 365 Business Premiumsisältää ominaisuuksia, jotka suojaavat tietojasi ja laitteitasi ja auttavat pitämään asiakkaiden ja asiakkaidesi arkaluonteiset tiedot turvassa.</span><span class="sxs-lookup"><span data-stu-id="5c04c-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="5c04c-105">DLP-ominaisuuksien määrittäminen</span><span class="sxs-lookup"><span data-stu-id="5c04c-105">Set up DLP features</span></span>

<span data-ttu-id="5c04c-106">Lisätietoja [dlp-käytännön luomisesta mallista](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) on kohdassa, miten voit määrittää käytännön, joka suojaa henkilökohtaisilta tunnisteilta (PII).</span><span class="sxs-lookup"><span data-stu-id="5c04c-106">See [Create a DLP policy from a template](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="5c04c-107">DLP sisältää monia käyttövalmiita käytäntömalleja monille eri kielille.</span><span class="sxs-lookup"><span data-stu-id="5c04c-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="5c04c-108">Esimerkiksi Australia Financial Data, Canada Personal Information Act, Yhdysvaltain taloudelliset tiedot ja niin edelleen.</span><span class="sxs-lookup"><span data-stu-id="5c04c-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="5c04c-109">Täydellinen luettelo on [kohdassa, mitä DLP-käytäntömallit sisältävät.](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include)</span><span class="sxs-lookup"><span data-stu-id="5c04c-109">See [What the DLP policy templates include](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) for a full list.</span></span> <span data-ttu-id="5c04c-110">Kaikki nämä mallit voidaan ottaa käyttöön samalla tavalla kuin pii-malliesimerkki.</span><span class="sxs-lookup"><span data-stu-id="5c04c-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="5c04c-111">Sähköpostin säilyttämisen määrittäminen Exchange Online -arkistoinnin avulla</span><span class="sxs-lookup"><span data-stu-id="5c04c-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="5c04c-112">**Exchange OnlineArchiving -käyttöoikeusominaisuudet** auttavat ylläpitämään vaatimustenmukaisuus- ja sääntelystandardeja säilyttämällä eDiscovery-sähköpostin sisällön.</span><span class="sxs-lookup"><span data-stu-id="5c04c-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="5c04c-113">Se auttaa myös vähentämään riskiä, jos on oikeusjuttu, ja tarjoaa tavan palauttaa tietoja tietoturvaloukkauksen jälkeen tai kun sinun täytyy palauttaa poistetut kohteet.</span><span class="sxs-lookup"><span data-stu-id="5c04c-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="5c04c-114">Oikeustoimiin liittyvän pidon avulla voit säilyttää käyttäjän koko sisällön tai mukauttaa säilytettävääsi sisältöä säilytyskäytäntöjen avulla.</span><span class="sxs-lookup"><span data-stu-id="5c04c-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="5c04c-115">**Oikeustoimiin liittyvä pito:** Voit säilyttää kaiken postilaatikon sisällön, poistetut kohteet mukaan lukien, asettamalla käyttäjän koko postilaatikon oikeustoimiin liittyvään pitoon.</span><span class="sxs-lookup"><span data-stu-id="5c04c-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="5c04c-116">Postilaatikon sijoitaminen oikeustoimiin liittyvään pitoon hallintakeskuksessa:</span><span class="sxs-lookup"><span data-stu-id="5c04c-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="5c04c-117">Valitse vasemmasta siirtymisruudusta **Käyttäjät** \> **aktiiviset käyttäjät**.</span><span class="sxs-lookup"><span data-stu-id="5c04c-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="5c04c-118">Valitse käyttäjä, jonka postilaatikon haluat sijoittaa oikeustoimiin liittyvään pitoon.</span><span class="sxs-lookup"><span data-stu-id="5c04c-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="5c04c-119">Laajenna käyttäjäruudussa **Mailin asetukset**ja valitse **Lisää asetuksia**-kohdan vierestä **Muokkaa Exchange-ominaisuuksia**.</span><span class="sxs-lookup"><span data-stu-id="5c04c-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="5c04c-120">Valitse käyttäjän postilaatikkosivulla \*\* postilaatikon ominaisuudet \*\* vasemmasta siirtymisruudusta ja valitse sitten **Ottaminen-linkki** **Oikeustoimiin liittyväpito**-kohdasta.</span><span class="sxs-lookup"><span data-stu-id="5c04c-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="5c04c-121">**Oikeustoimiin liittyvän pidon** valintaikkunassa voit määrittää oikeustoimiin liittyvän pidon keston **Oikeustoimiin liittyvän pidon kesto** -kentässä.</span><span class="sxs-lookup"><span data-stu-id="5c04c-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="5c04c-122">Jätä kenttä tyhjäksi, jos haluat sijoittaa äärettömän pidon.</span><span class="sxs-lookup"><span data-stu-id="5c04c-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="5c04c-123">Voit myös lisätä muistiinpanoja ja ohjata postilaatikon omistajan sivustoon, jota saatat joutua selittämään lisätietoja oikeustoimiin liittyvästä pidon pidon.</span><span class="sxs-lookup"><span data-stu-id="5c04c-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="5c04c-124">\>**Tallenna.**</span><span class="sxs-lookup"><span data-stu-id="5c04c-124">\> **Save**.</span></span>
    
<span data-ttu-id="5c04c-125">**Säilyttäminen:** Voit ottaa käyttöön mukautetut säilytyskäytännöt, esimerkiksi säilyttää tietyn ajan tai poistaa sisältöä pysyvästi säilytysajan lopussa.</span><span class="sxs-lookup"><span data-stu-id="5c04c-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="5c04c-126">Lisätietoja on [ohjeaiheessa Säilytyskäytäntöjen yleiskatsaus](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span><span class="sxs-lookup"><span data-stu-id="5c04c-126">To learn more, see [Overview of retention policies](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="5c04c-127">Herkkyysotsikoiden määrittäminen</span><span class="sxs-lookup"><span data-stu-id="5c04c-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="5c04c-128">Herkkyysotsikoissa on Azure Information Protection (AIP) Plan 1, ja ne auttavat sinua luokittelemaan ja halutessasi suojaamaan asiakirjoja ja sähköposteja käyttämällä tarroja.</span><span class="sxs-lookup"><span data-stu-id="5c04c-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="5c04c-129">Sääntöjä voivat käyttää automaattisesti järjestelmänvalvojat, jotka määrittävät säännöt ja ehdot manuaalisesti käyttäjien toimesta, tai käyttämällä yhdistelmää, jossa käyttäjille annetaan suosituksia.</span><span class="sxs-lookup"><span data-stu-id="5c04c-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="5c04c-130">Voit määrittää herkkyysotsikot tarkastelemaan [luojaa ja hallitsemaan herkkyystarroja- videota.](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)</span><span class="sxs-lookup"><span data-stu-id="5c04c-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="5c04c-131">Azure Information Protection -asiakkaan asentaminen manuaalisesti</span><span class="sxs-lookup"><span data-stu-id="5c04c-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="5c04c-132">AIP-asiakkaan asentaminen manuaalisesti:</span><span class="sxs-lookup"><span data-stu-id="5c04c-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="5c04c-133">Download **AzinfoProtection_UL.exe** polveutua [Mikroskooppi download keskittyä](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="5c04c-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="5c04c-134">Voit varmistaa, että asennus toimi tarkastelemalla Word-asiakirjaa ja varmistamalla, että **Herkkyys-vaihtoehto** on käytettävissä **Aloitus-välilehdessä.**</span><span class="sxs-lookup"><span data-stu-id="5c04c-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="5c04c-135">![Word-asiakirjan Suojaus-välilehden avattava.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="5c04c-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="5c04c-136">Lisätietoja on [ohjeaiheessa Asiakkaan asentaminen](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="5c04c-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
