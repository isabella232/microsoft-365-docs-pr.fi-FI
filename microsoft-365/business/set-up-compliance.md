---
title: Microsoft 365 Business Premiumin uhkien uhkien suojauksen nostaminen
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
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Määritä yhteensopivuusominaisuudet, jotka estävät tietojen menettämisen ja auttavat pitämään asiakkaidesi ja asiakkaidesi luottamukselliset tiedot turvassa.
ms.openlocfilehash: c0accc37d3dcda9ba75813f01a98a3233c5a8369
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579950"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="08c40-103">Yhteensopivuusominaisuuksien määritäminen</span><span class="sxs-lookup"><span data-stu-id="08c40-103">Set up compliance features</span></span>

<span data-ttu-id="08c40-104">Microsoft 365 Business Premium sisältää ominaisuuksia, jotka suojaavat tietojasi ja laitteitasi ja auttavat sinua pitämään asiakkaidesi ja asiakkaidesi luottamukselliset tiedot turvassa.</span><span class="sxs-lookup"><span data-stu-id="08c40-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="08c40-105">DLP-ominaisuuksien asetusten täytäminen</span><span class="sxs-lookup"><span data-stu-id="08c40-105">Set up DLP features</span></span>

<span data-ttu-id="08c40-106">Katso [mallista DLP-käytännön](../compliance/create-a-dlp-policy-from-a-template.md) luominen esimerkiksi siitä, miten voit määrittää käytännön, joka suojaa henkilökohtaisten tietojen menetykseltä.</span><span class="sxs-lookup"><span data-stu-id="08c40-106">See [Create a DLP policy from a template](../compliance/create-a-dlp-policy-from-a-template.md) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="08c40-107">DLP sisältää useita käyttövalmiita käytäntömalleja useille eri kielille.</span><span class="sxs-lookup"><span data-stu-id="08c40-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="08c40-108">Esimerkiksi Australia Financial Data, Canada Personal Information Act, U.S. Financial Data ja niin edelleen.</span><span class="sxs-lookup"><span data-stu-id="08c40-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="08c40-109">Katso, [mitkä DLP-käytäntömallit](../compliance/what-the-dlp-policy-templates-include.md) sisältävät täydellisen luettelon.</span><span class="sxs-lookup"><span data-stu-id="08c40-109">See [What the DLP policy templates include](../compliance/what-the-dlp-policy-templates-include.md) for a full list.</span></span> <span data-ttu-id="08c40-110">Kaikki nämä mallit voidaan ottaa käyttöön samalla tavalla kuin PII-malliesimerkki.</span><span class="sxs-lookup"><span data-stu-id="08c40-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="08c40-111">Sähköpostin säilytyksen määrittäminen Exchange Online Archivingin avulla</span><span class="sxs-lookup"><span data-stu-id="08c40-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="08c40-112">**Exchange Online Archiving** -käyttöoikeusominaisuudet auttavat säilyttämään vaatimustenmukaisuus- ja säädöstenmukaisuusstandardit säilyttämällä eDiscoveryn sähköpostisisällön.</span><span class="sxs-lookup"><span data-stu-id="08c40-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="08c40-113">Se myös vähentää riskiäsi, jos oikeusjutun on olemassa, ja tarjoaa keinon tietojen palauttamiseen tietoturvarikkomuksen jälkeen tai silloin, kun haluat palauttaa poistetut kohteet.</span><span class="sxs-lookup"><span data-stu-id="08c40-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="08c40-114">Voit säilyttää kaiken käyttäjän sisällön oikeus oikeushallintapitoa käyttämällä tai mukauttaa säilytyskäytäntöjen avulla sitä, mitä haluat säilyttää.</span><span class="sxs-lookup"><span data-stu-id="08c40-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="08c40-115">**Oikeusistuntoon pito:** Voit säilyttää postilaatikon kaiken sisällön poistetut kohteet mukaan lukien asettamalla käyttäjän koko postilaatikon oikeusistuntoon.</span><span class="sxs-lookup"><span data-stu-id="08c40-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="08c40-116">Voit sijoittaa postilaatikon oikeusportaalin pitoon hallintakeskuksessa:</span><span class="sxs-lookup"><span data-stu-id="08c40-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="08c40-117">Valitse vasemmassa siirtymispalkin yläkulmassa **Käyttäjät,** \> **jotka ovat aktiivisia.**</span><span class="sxs-lookup"><span data-stu-id="08c40-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="08c40-118">Valitse käyttäjä, jonka postilaatikon haluat sijoittaa oikeusistuntoon.</span><span class="sxs-lookup"><span data-stu-id="08c40-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="08c40-119">Laajenna käyttäjäruudussa **Sähköpostiasetukset ja valitse** Lisää asetuksia **-kohdassa** Muokkaa **Exchange-ominaisuuksia.**</span><span class="sxs-lookup"><span data-stu-id="08c40-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="08c40-120">Valitse käyttäjän postilaatikkosivulla \*\* postilaatikon ominaisuudet \*\* vasemmasta siirtymispalkin kohdasta ja valitse sitten Ota käyttöön -linkki **Oikeusmääräys-pito-kohdassa.** </span><span class="sxs-lookup"><span data-stu-id="08c40-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="08c40-121">Voit määrittää **oikeus riitautuksen** pitovalintaikkunassa oikeusistuinten pitoajan keston oikeus oikeusistuinten **kestokentässä.**</span><span class="sxs-lookup"><span data-stu-id="08c40-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="08c40-122">Jätä kenttä tyhjäksi, jos haluat sijoittaa äärettömän pitoon.</span><span class="sxs-lookup"><span data-stu-id="08c40-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="08c40-123">Voit myös lisätä muistiinpanoja ja ohjata postilaatikon omistajan verkkosivustoon, jossa sinun on ehkä selitettävä lisää oikeus oikeusistuntoon liittyen.</span><span class="sxs-lookup"><span data-stu-id="08c40-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="08c40-124">\>**Tallenna.**</span><span class="sxs-lookup"><span data-stu-id="08c40-124">\> **Save**.</span></span>
    
<span data-ttu-id="08c40-125">**Säilytys:** Voit ottaa käyttöön mukautettuja säilytyskäytäntöjä, jos esimerkiksi haluat säilyttää tietyn ajan tai poistaa sisältöä pysyvästi säilytysajan lopussa.</span><span class="sxs-lookup"><span data-stu-id="08c40-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="08c40-126">Lisätietoja on ohjeaiheessa [Säilytyskäytäntöjen yleiskatsaus.](../compliance/retention.md)</span><span class="sxs-lookup"><span data-stu-id="08c40-126">To learn more, see [Overview of retention policies](../compliance/retention.md).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="08c40-127">Luottamuksellisuusotsikoiden valitseminen</span><span class="sxs-lookup"><span data-stu-id="08c40-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="08c40-128">Luottamuksellisuustunnisteet tulevat Azure Information Protection (AIP) -palvelupaketti 1:n mukana, ja ne auttavat luokittelemaan ja suojaamaan asiakirjojasi ja sähköpostejasi käyttämällä tarroja.</span><span class="sxs-lookup"><span data-stu-id="08c40-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="08c40-129">Järjestelmänvalvojat, jotka määrittävät sääntöjä ja ehtoja, voivat ottaa selitteet käyttöön automaattisesti, käyttäjien manuaalisesti tai käyttämällä yhdistelmää, jossa käyttäjille annetaan suosituksia.</span><span class="sxs-lookup"><span data-stu-id="08c40-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="08c40-130">Jos haluat määrittää luottamuksellisuusotsikot, tarkastele [luottamuksellisuusotsikoiden luontia ja hallintaa](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) videossa.</span><span class="sxs-lookup"><span data-stu-id="08c40-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="08c40-131">Azure Information Protection -asiakasohjelman asentaminen manuaalisesti</span><span class="sxs-lookup"><span data-stu-id="08c40-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="08c40-132">AIP-asiakasohjelman asentaminen manuaalisesti:</span><span class="sxs-lookup"><span data-stu-id="08c40-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="08c40-133">Lataa **AzinfoProtection_UL.exe** Microsoft [Download Centeristä.](https://www.microsoft.com/download/details.aspx?id=53018)</span><span class="sxs-lookup"><span data-stu-id="08c40-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="08c40-134">Voit tarkistaa, että asennus on toiminut tarkastelemalla Word-asiakirjaa ja varmistamalla, että Luottamuksellisuus-vaihtoehto  on käytettävissä **Aloitus-välilehdessä.**</span><span class="sxs-lookup"><span data-stu-id="08c40-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="08c40-135">![Word-asiakirjan avattava Suojaus-välilehti.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="08c40-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="08c40-136">Lisätietoja on kohdassa [Asiakkaan asentaminen.](/azure/information-protection/infoprotect-tutorial-step3)</span><span class="sxs-lookup"><span data-stu-id="08c40-136">For more information, see [Install the client](/azure/information-protection/infoprotect-tutorial-step3).</span></span>