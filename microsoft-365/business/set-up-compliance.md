---
title: Nosta uhkien Microsoft 365 Business Premium
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
description: Vaatimustenmukaisuusominaisuuksien avulla voit estää tietojen menettämisen ja pitää asiakkaan ja asiakkaan luottamukselliset tiedot suojattuina.
ms.openlocfilehash: 945f8a283b90b89da2fbe67a073e0807b80d198f
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245080"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="bffec-103">Yhteensopivuusominaisuuksien täytäminen</span><span class="sxs-lookup"><span data-stu-id="bffec-103">Set up compliance features</span></span>

<span data-ttu-id="bffec-104">Oma Microsoft 365 Business Premium sisältää ominaisuuksia, joilla voit suojata tietojasi ja laitteitasi ja auttaa sinua pitämään sekä asiakkaidesi luottamukselliset tiedot suojattuina.</span><span class="sxs-lookup"><span data-stu-id="bffec-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="bffec-105">DLP-ominaisuuksien asetusten</span><span class="sxs-lookup"><span data-stu-id="bffec-105">Set up DLP features</span></span>

<span data-ttu-id="bffec-106">Katso [DLP-käytännön luominen mallista,](../compliance/create-a-dlp-policy-from-a-template.md) jos haluat esimerkiksi määrittää käytännön, joka suojaa henkilökohtaisten tietojen menetykseltä.</span><span class="sxs-lookup"><span data-stu-id="bffec-106">See [Create a DLP policy from a template](../compliance/create-a-dlp-policy-from-a-template.md) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="bffec-107">DLP sisältää useita käyttövalmiita käytäntömalleja monille eri kielille.</span><span class="sxs-lookup"><span data-stu-id="bffec-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="bffec-108">Esimerkki: Australia Financial Data, Canada Personal Information Act, Yhdysvaltain taloudelliset tiedot ja niin edelleen.</span><span class="sxs-lookup"><span data-stu-id="bffec-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="bffec-109">Täydellinen [luettelo on kohdassa Mitä DLP-käytäntömallit](../compliance/what-the-dlp-policy-templates-include.md) sisältävät.</span><span class="sxs-lookup"><span data-stu-id="bffec-109">See [What the DLP policy templates include](../compliance/what-the-dlp-policy-templates-include.md) for a full list.</span></span> <span data-ttu-id="bffec-110">Kaikki nämä mallit voidaan ottaa käyttöön samalla tavalla kuin PII-malliesimerkki.</span><span class="sxs-lookup"><span data-stu-id="bffec-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="bffec-111">Sähköpostin säilytysajan määrittäminen Exchange Online Archiving</span><span class="sxs-lookup"><span data-stu-id="bffec-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="bffec-112">**Exchange Online Archiving** käyttöoikeuksien ominaisuudet auttavat säilyttämään vaatimustenmukaisuus- ja sääntelystandardit säilyttämällä eDiscoveryn sähköpostisisällön.</span><span class="sxs-lookup"><span data-stu-id="bffec-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="bffec-113">Se myös vähentää riskiä, jos oikeusjutun on olemassa, ja tarjoaa keinon tietojen palauttamiseen suojausrikkomuksen jälkeen tai silloin, kun haluat palauttaa poistetut kohteet.</span><span class="sxs-lookup"><span data-stu-id="bffec-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="bffec-114">Oikeuskäytännön avulla voit säilyttää käyttäjän kaiken sisällön tai mukauttaa säilytettävät sisällöt säilytyskäytäntöjen avulla.</span><span class="sxs-lookup"><span data-stu-id="bffec-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="bffec-115">**Oikeus oikeusistuntoon pito:** Voit säilyttää postilaatikon kaiken sisällön poistetut kohteet mukaan lukien asettamalla käyttäjän koko postilaatikon oikeusistuntoon.</span><span class="sxs-lookup"><span data-stu-id="bffec-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="bffec-116">Voit sijoittaa postilaatikon oikeusistuntoon hallintakeskuksessa:</span><span class="sxs-lookup"><span data-stu-id="bffec-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="bffec-117">Valitse vasemmassa siirtymispalkin siirtymispalissa  \> **Käyttäjät, jotka ovat aktiivisia.**</span><span class="sxs-lookup"><span data-stu-id="bffec-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="bffec-118">Valitse käyttäjä, jonka postilaatikon haluat sijoittaa oikeus oikeusistuntoon.</span><span class="sxs-lookup"><span data-stu-id="bffec-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="bffec-119">Laajenna käyttäjäruudussa **Postiasetukset ja** valitse Lisää asetuksia **-kohdan vierestä** **Muokkaa Exchange ominaisuuksia**.</span><span class="sxs-lookup"><span data-stu-id="bffec-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="bffec-120">Valitse käyttäjän postilaatikkosivulla \*\* postilaatikon ominaisuudet \*\* vasemmassa siirtymispalkin siirtymispalissa ja valitse sitten Ota **käyttöön** -linkki oikeus **hallintapito -kohdassa.**</span><span class="sxs-lookup"><span data-stu-id="bffec-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="bffec-121">**Riitautuksen pitovalintaikkunassa** voit määrittää oikeusistuinten pitokentän **keston.**</span><span class="sxs-lookup"><span data-stu-id="bffec-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="bffec-122">Jätä kenttä tyhjäksi, jos haluat sijoittaa äärettömän pitoon.</span><span class="sxs-lookup"><span data-stu-id="bffec-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="bffec-123">Voit myös lisätä muistiinpanoja ja ohjata postilaatikon omistajan verkkosivustoon, jossa sinun on ehkä selitettävä enemmän oikeus oikeusistuntoon liittyen.</span><span class="sxs-lookup"><span data-stu-id="bffec-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="bffec-124">\>**Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="bffec-124">\> **Save**.</span></span>
    
<span data-ttu-id="bffec-125">**Säilytys:** Voit ottaa käyttöön mukautettuja säilytyskäytäntöjä, jos esimerkiksi haluat säilyttää tietyn ajan tai poistaa sisältöä pysyvästi säilytysajan lopussa.</span><span class="sxs-lookup"><span data-stu-id="bffec-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="bffec-126">Lisätietoja on kohdassa [Säilytyskäytäntöjen yleiskatsaus.](../compliance/retention.md)</span><span class="sxs-lookup"><span data-stu-id="bffec-126">To learn more, see [Overview of retention policies](../compliance/retention.md).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="bffec-127">Luottamuksellisuusotsikoiden valitseminen</span><span class="sxs-lookup"><span data-stu-id="bffec-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="bffec-128">Luottamuksellisuustunnisteet on varustettu Azure Information Protection (AIP) -palvelupaketti 1:llä, ja niiden avulla voit luokitella ja halutessasi suojata asiakirjoja ja sähköposteja käyttämällä tarroja.</span><span class="sxs-lookup"><span data-stu-id="bffec-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="bffec-129">Järjestelmänvalvojat, jotka määrittävät säännöt ja ehdot, voivat ottaa selitteet käyttöön automaattisesti, käyttäjien manuaalisesti tai yhdistelmällä, jossa käyttäjille annetaan suosituksia.</span><span class="sxs-lookup"><span data-stu-id="bffec-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="bffec-130">Jos haluat määrittää luottamuksellisuusotsikot, katso [luottamuksellisuusotsikoiden](../business-video/create-sensitivity-labels.md) luominen ja hallinta -video.</span><span class="sxs-lookup"><span data-stu-id="bffec-130">To set up Sensitivity labels, view [create and manage sensitivity labels](../business-video/create-sensitivity-labels.md) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="bffec-131">Azure Information Protection -asiakasohjelman asentaminen manuaalisesti</span><span class="sxs-lookup"><span data-stu-id="bffec-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="bffec-132">AIP-asiakasohjelman asentaminen manuaalisesti:</span><span class="sxs-lookup"><span data-stu-id="bffec-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="bffec-133">Lataa **AzinfoProtection_UL.exe** Microsoft [Download Centeristä.](https://www.microsoft.com/download/details.aspx?id=53018)</span><span class="sxs-lookup"><span data-stu-id="bffec-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="bffec-134">Voit tarkistaa asennuksen toimimisen tarkastelemalla Word-asiakirjaa  ja varmistamalla, että Luottamuksellisuus-vaihtoehto on käytettävissä **Aloitus-välilehdessä.**</span><span class="sxs-lookup"><span data-stu-id="bffec-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="bffec-135">![Word-asiakirjan avattava Suojaus-välilehti.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="bffec-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="bffec-136">Lisätietoja on kohdassa [Asiakkaan asentaminen.](/azure/information-protection/infoprotect-tutorial-step3)</span><span class="sxs-lookup"><span data-stu-id="bffec-136">For more information, see [Install the client](/azure/information-protection/infoprotect-tutorial-step3).</span></span>