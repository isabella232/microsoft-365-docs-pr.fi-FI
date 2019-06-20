---
title: Suurenna Microsoft 365 Business suojaa uhka
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
search.appverid:
- BCS160
- MET150
description: 'Määrittäminen Office 365: n Advanced Threat Protection ja luottamuksellisten tietojen turvaamiseksi.'
ms.openlocfilehash: 53741a7726222bb32329a401953be72257df95cc
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086314"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="8076f-103">Määritä yhteensopivuuden ominaisuudet</span><span class="sxs-lookup"><span data-stu-id="8076f-103">Set up compliance features</span></span>

<span data-ttu-id="8076f-104">Microsoft 365 liiketoiminnan mukana ominaisuuksia suojaa tietoja ja laitteita ja auttaa pitämään teille ja asiakkaiden luottamukselliset tiedot turvassa.</span><span class="sxs-lookup"><span data-stu-id="8076f-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="8076f-105">DLP-ominaisuuksien määrittäminen</span><span class="sxs-lookup"><span data-stu-id="8076f-105">Set up DLP features</span></span>

<span data-ttu-id="8076f-106">Katso [luominen mallista DLP käytännön](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) esimerkki siitä, kuinka voit määrittää käytännön henkilökohtaisia tietoja (henkilökohtaisia tietoja) vastaan.</span><span class="sxs-lookup"><span data-stu-id="8076f-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="8076f-107">DLP mukana monta monta eri kieliversioiden valmis avulla käytännön malleja.</span><span class="sxs-lookup"><span data-stu-id="8076f-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="8076f-108">Taloudellisia tietoja Australian, Kanadan Personal Information Act, Yhdysvaltain taloudellisten tietojen, esimerkiksi jne. Saat täydellisen luettelon [mitä DLP-Käytäntömallit ovat](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) .</span><span class="sxs-lookup"><span data-stu-id="8076f-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="8076f-109">Kaikki mallit voidaan ottaa käyttöön henkilökohtaisia tietoja malli esimerkin.</span><span class="sxs-lookup"><span data-stu-id="8076f-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="8076f-110">Määritä Exchange Online arkistoida kanssa sähköpostin säilytys</span><span class="sxs-lookup"><span data-stu-id="8076f-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="8076f-111">Käyttöoikeuden ominaisuuksia **Exchange Online arkistoida** auttaa säilyttämään vaatimusten ja standardien säilytät sähköpostin sisällön eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="8076f-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="8076f-112">Se myös auttaa Jos Oletteko varotoimia ja avulla voit palauttaa tietoja turvallisuusongelmista jälkeen tai kun haluat palauttaa poistettuja kohteita.</span><span class="sxs-lookup"><span data-stu-id="8076f-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="8076f-113">Voit käyttää oikeudenkäyntiä pitoon säilyttää käyttäjän sisällön tai säilytyskäytännöt avulla voit mukauttaa haluat säilyttää.</span><span class="sxs-lookup"><span data-stu-id="8076f-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="8076f-114">**Pito oikeudenkäyntiä:** Voit säilyttää kaikki postilaatikon sisältö mukaan lukien poistetut sijoittamalla käyttäjän postilaatikon koko oikeudenkäyntiä, pidä.</span><span class="sxs-lookup"><span data-stu-id="8076f-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="8076f-115">Voit sijoittaa oikeudenkäyntiä postilaatikkoon hold Admin Centerissä:</span><span class="sxs-lookup"><span data-stu-id="8076f-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="8076f-116">Siirry vasemman nav- **käyttäjät** \> **aktiivisia käyttäjiä**.</span><span class="sxs-lookup"><span data-stu-id="8076f-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="8076f-117">Valitse käyttäjä, jonka postilaatikon haluat sijoittaa oikeudenkäyntiä pidä laajentaa käyttäjän ruudun **Sähköpostiasetukset** ja valita **Lisää asetuksia** -kohdan vieressä **Muokkaa Exchange-ominaisuudet**.</span><span class="sxs-lookup"><span data-stu-id="8076f-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="8076f-118">Valitse käyttäjän postilaatikko-sivulla \*\* postilaatikon ominaisuuksia \*\* vasemman nav-painiketta ja valitsemalla sitten **Ota käyttöön** -linkki **pidossa oikeudellisten toimien**mukaisesti.</span><span class="sxs-lookup"><span data-stu-id="8076f-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="8076f-119">Valintaikkunassa voit määrittää kanne **oikeusjutun pidä** pidä kesto **pidossa oikeudellisten toimien kesto** -kenttään, jätä kenttä tyhjäksi, jos haluat sijoittaa äärettömän pito.</span><span class="sxs-lookup"><span data-stu-id="8076f-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="8076f-120">Voit myös lisätä muistiinpanoja ja direct mail ruutuun omistaja Web-sivustoon saattaa olla lisätietoja kanne pitää selittää \> **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="8076f-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="8076f-121">**Säilyttäminen:** Voit ottaa käyttöön mukautetut säilytyskäytännöt, esimerkiksi säilyttää tietyn ajanjakson ajan tai poistaa sisällön pysyvästi säilytysajan päätyttyä.</span><span class="sxs-lookup"><span data-stu-id="8076f-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="8076f-122">Lisätietoja on kohdassa [Yleiskatsaus säilytyskäytäntöjä](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="8076f-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-azure-information-protection-features"></a><span data-ttu-id="8076f-123">Määritä Azure tietojen suojauksen ominaisuudet</span><span class="sxs-lookup"><span data-stu-id="8076f-123">Set up Azure Information Protection features</span></span>

<span data-ttu-id="8076f-124">Azure tietojen suojaus (järjestelmänvalvojan Asennuspiste) auttaa sinua luokitella ja myös suojata asiakirjoja tai sähköpostiviestejä, ja soveltamalla otsikot.</span><span class="sxs-lookup"><span data-stu-id="8076f-124">Azure Information Protection (AIP) helps you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="8076f-125">Otsikoita voi käyttää automaattisesti järjestelmänvalvojille, jotka määrittävät säännöt ja ehdot, manuaalisesti käyttäjät tai käyttämällä yhdistelmää, jossa käyttäjille annetaan suosituksia.</span><span class="sxs-lookup"><span data-stu-id="8076f-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="8076f-126">Outlookin web-voit käyttää sisäänrakennettu seuraavat otsikot ja rajoitukset että sähköpostit:</span><span class="sxs-lookup"><span data-stu-id="8076f-126">In Outlook on the web you can apply the following built-in labels and restrictions to your emails:</span></span>
  
- <span data-ttu-id="8076f-127">**Älä lähetä edelleen**: vastaanottajat voivat lukea viestin, mutta ne ei eteenpäin, tulostaa tai kopioida sen sisältöä</span><span class="sxs-lookup"><span data-stu-id="8076f-127">**Do Not Forward**: Recipients can read the message, but they can't forward, print, or copy content</span></span>
    
- <span data-ttu-id="8076f-128">**Salaa**: koko viesti on salattu.</span><span class="sxs-lookup"><span data-stu-id="8076f-128">**Encrypt**: The entire message is encrypted.</span></span> <span data-ttu-id="8076f-129">Vastaanottajien on henkilöllisyytensä ennen salatun sisällön käyttämistä ja salausta ei voi poistaa.</span><span class="sxs-lookup"><span data-stu-id="8076f-129">Recipients must confirm their identity before accessing encrypted content and can't remove encryption.</span></span>
    
- <span data-ttu-id="8076f-130">**Luottamuksellinen**: organisaation työntekijät antaa täydet oikeudet, sähköposti ja liitteet, mutta ei oman organisaation ulkopuolisille henkilöille.</span><span class="sxs-lookup"><span data-stu-id="8076f-130">**Confidential**: Gives the employees in your organization full permissions to the email content and attachments, but not to people outside your organization.</span></span> <span data-ttu-id="8076f-131">Tietojen omistajat voivat seurata ja sisältöä milloin tahansa peruuttaa.</span><span class="sxs-lookup"><span data-stu-id="8076f-131">Data owners can track and revoke content at any point.</span></span>
    
- <span data-ttu-id="8076f-132">**Erittäin luottamuksellisia**: Tämä rajoitus voidaan ottaa käyttöön erittäin luottamuksellisia tietoja, joiden avulla työntekijät voivat tarkastella, muokata, ja vastata, mutta ei välittää, tulostaa tai kopioida tiedot.</span><span class="sxs-lookup"><span data-stu-id="8076f-132">**Highly Confidential**: This restriction can be applied to highly confidential data, allowing employees to view, edit, and reply, but not forward, print, or copy the data.</span></span> <span data-ttu-id="8076f-133">Tietojen omistajat voivat seurata ja sisältöä milloin tahansa peruuttaa.</span><span class="sxs-lookup"><span data-stu-id="8076f-133">Data owners can track and revoke content at any point.</span></span>

### <a name="make-sure-azure-information-protection-is-activated"></a><span data-ttu-id="8076f-134">Varmista, että Azure tietojen suojaus on käytössä.</span><span class="sxs-lookup"><span data-stu-id="8076f-134">Make sure Azure Information Protection is activated</span></span>

<span data-ttu-id="8076f-135">Tarkista, että järjestelmänvalvojan Asennuspiste on käytössä:</span><span class="sxs-lookup"><span data-stu-id="8076f-135">To verify that AIP is activated :</span></span>

1. <span data-ttu-id="8076f-136">Kirjaudu [Azure](https://portal.azure.com/)portaaliin.</span><span class="sxs-lookup"><span data-stu-id="8076f-136">Sign into [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="8076f-137">Valitse **kaikki palvelut** ja kirjoita **Hakukenttään** *Azure tietojen suojaaminen* .</span><span class="sxs-lookup"><span data-stu-id="8076f-137">Select **All services** and type in *Azure Information Protection* in the **Search Box**.</span></span>

3. <span data-ttu-id="8076f-138">Kun näkyviin, napsauta Käynnistä-painiketta, seuraava **Azure tietojen suojaus** jotta suosikki ja helppo löytää myöhemmin.</span><span class="sxs-lookup"><span data-stu-id="8076f-138">Once the results display, click the start next to **Azure Information Protection** to make it a favorite and easy to find later.</span></span>

4. <span data-ttu-id="8076f-139">Valitse **Azure tietojen suojaus** \> **Suojaus aktivointi** ja tehdä Varmista, että otat voi aktivoitua.</span><span class="sxs-lookup"><span data-stu-id="8076f-139">Select **Azure Information Protection** \> **Protection activation** and make sure the status is set to activated.</span></span> 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a><span data-ttu-id="8076f-140">Näytä Azure tietojen suojaaminen ja käytännön oletusarvon otsikot</span><span class="sxs-lookup"><span data-stu-id="8076f-140">View the Azure Information Protection policy and default labels</span></span> 

<span data-ttu-id="8076f-141">Voit tarkastella ja muokata, olemassa olevat otsikot:</span><span class="sxs-lookup"><span data-stu-id="8076f-141">To view, and modify, the existing labels:</span></span>

1. <span data-ttu-id="8076f-142">Azure-tietojen suojaaminen kojelaudassa, valitse **luokitukset** \> **tarroja**.</span><span class="sxs-lookup"><span data-stu-id="8076f-142">On the Azure Information Protection dashboard, select **Classifications** \> **Labels**.</span></span> <br/><span data-ttu-id="8076f-143">![Azure-tietojen suojaaminen vakio-otsikoita.](media/AIPLabels.png)</span><span class="sxs-lookup"><span data-stu-id="8076f-143">![Standard labels for Azure Information Protection.](media/AIPLabels.png)</span></span>

2. <span data-ttu-id="8076f-144">Voit valita kaikki otsikon Näytä asetukset, voit muuttaa nimen, värit jne.</span><span class="sxs-lookup"><span data-stu-id="8076f-144">You can choose any label to view options, you can change the display name, colors, etc.</span></span>
 
3. <span data-ttu-id="8076f-145">Katso [Muokkaa ja luo uudet etiketit](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) Jos haluat luoda omia.</span><span class="sxs-lookup"><span data-stu-id="8076f-145">See  [Modify and create new labels](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) if you want to create your own.</span></span> 

### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="8076f-146">Tietojen suojaaminen Azure-asiakasohjelman asentaminen manuaalisesti</span><span class="sxs-lookup"><span data-stu-id="8076f-146">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="8076f-147">Manuaalisesti asentaminen järjestelmänvalvojan Asennuspiste-client:</span><span class="sxs-lookup"><span data-stu-id="8076f-147">To manually install the AIP client:</span></span>

1. <span data-ttu-id="8076f-148">**AzInfoProtection.exe** ladata [Microsoft download Centeristä](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="8076f-148">Download **AzInfoProtection.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="8076f-149">Voit varmistaa, että Word-asiakirjan tarkasteleminen ja varmistamalla, että **Suojaa** -vaihtoehto on käytettävissä **Aloitus** -välilehden työskennelleet asennus.</span><span class="sxs-lookup"><span data-stu-id="8076f-149">You can verify that the installation worked by viewing a Word document and making sure that the **Protect** option is available on the **Home** tab.</span></span> <br/><span data-ttu-id="8076f-150">![Suojaus-välilehden avattavan Word-asiakirjan.](media/Word_Protect.png)</span><span class="sxs-lookup"><span data-stu-id="8076f-150">![Protection tab drop-down in a Word document.](media/Word_Protect.png)</span></span>

<span data-ttu-id="8076f-151">Lisätietoja on ohjeaiheessa [Asenna asiakkaan](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="8076f-151">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
