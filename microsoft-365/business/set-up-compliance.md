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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Määritä Office 365 Advanced uhkien torjunta ja suojaa arkaluontoisia tietoja.
ms.openlocfilehash: 8144bcebe8a0cdf28a5e092f592362922ccbdd48
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288741"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="e4d73-103">Yhteensopivuus ominaisuuksien määrittäminen</span><span class="sxs-lookup"><span data-stu-id="e4d73-103">Set up compliance features</span></span>

<span data-ttu-id="e4d73-104">Microsoft 365-yritys sisältää ominaisuuksia, jotka suojaavat tietojasi ja laitteitasi sekä auttavat pitämään omasi ja asiakkaidesi arkaluonteiset tiedot turvassa.</span><span class="sxs-lookup"><span data-stu-id="e4d73-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="e4d73-105">DLP-ominaisuuksien määrittäminen</span><span class="sxs-lookup"><span data-stu-id="e4d73-105">Set up DLP features</span></span>

<span data-ttu-id="e4d73-106">Katso [Luo DLP-käytäntö mallista](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) esimerkkinä siitä, miten voit määrittää käytännön suojaamaan henkilökohtaisia tunniste tietoja (pii) vastaan.</span><span class="sxs-lookup"><span data-stu-id="e4d73-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="e4d73-107">DLP sisältää monia valmiita käytäntö malleja monille eri kieli alueilla.</span><span class="sxs-lookup"><span data-stu-id="e4d73-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="e4d73-108">Esimerkiksi Australian taloudelliset tiedot, Kanadan henkilö tieto laki, Yhdysvaltain taloudelliset tiedot jne. Katso, [mitä DLP-käytäntö mallit sisältävät](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) täydellisestä luettelosta.</span><span class="sxs-lookup"><span data-stu-id="e4d73-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="e4d73-109">Kaikki nämä mallit voidaan ottaa käyttöön samanlaisiksi kuin PII-malli esimerkki.</span><span class="sxs-lookup"><span data-stu-id="e4d73-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="e4d73-110">Sähkö postin säilyttämisen määrittäminen Exchange Online-arkistoinnin avulla</span><span class="sxs-lookup"><span data-stu-id="e4d73-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="e4d73-111">**Exchange Online-arkistointi** lisenssi ominaisuudet auttavat ylläpitämään yhteensopivuus-ja sääntely standardeja säilyttämällä Sähkö posti sisällön eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="e4d73-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="e4d73-112">Se auttaa myös vähentämään riskiä tapa uksessa oikeus juttu ja tarjoaa tapa palauttaa tietoja, kun tieto turva loukkaus, tai kun haluat palauttaa poistetut kohteet.</span><span class="sxs-lookup"><span data-stu-id="e4d73-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="e4d73-113">Voit säilyttää kaikki käyttäjän sisällöt tai käyttää säilytys käytäntöjä, kun haluat muokata säilytetä.</span><span class="sxs-lookup"><span data-stu-id="e4d73-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="e4d73-114">**Oikeuden käyntien pito:** Voit säilyttää kaiken posti laatikon sisällön, mukaan lukien poistetut kohteet, asettamalla käyttäjän koko posti laatikon oikeus riita-asioihin.</span><span class="sxs-lookup"><span data-stu-id="e4d73-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="e4d73-115">Voit sijoittaa posti laatikon oikeuden käyntiin pitämällä hallinta keskuksessa:</span><span class="sxs-lookup"><span data-stu-id="e4d73-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="e4d73-116">Siirry vasemmassa siirtymis osassa **käyttäjät** \> **aktiiviset käyttäjät**-kohtaan.</span><span class="sxs-lookup"><span data-stu-id="e4d73-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="e4d73-117">Valitse käyttäjä, jonka posti laatikon haluat sijoittaa oikeuden käyntien pito-ja käyttäjä ruudussa Laajenna Mail- **Asetukset** ja valitse **Lisää asetuksia** -kohdasta **Muokkaa Exchangen ominaisuuksia**.</span><span class="sxs-lookup"><span data-stu-id="e4d73-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="e4d73-118">Valitse käyttäjän posti laatikko-sivulla \* \* posti laatikon ominaisuudet \* \* vasemmassa NAV-ohjelmassa ja valitse sitten **Ota käyttöön** -linkki kohdassa **oikeuden käynti pito**.</span><span class="sxs-lookup"><span data-stu-id="e4d73-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="e4d73-119">Voit määrittää **riita-** asioiden pito-valinta ikkunassa oikeuden käynnin keston kesto-kentässä, jätä kenttä tyhjäksi, jos haluat sijoittaa äärettömän **pito ajan.**</span><span class="sxs-lookup"><span data-stu-id="e4d73-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="e4d73-120">Voit myös lisätä muistiinpanoja ja ohjata posti laatikon omistajan sivustoon, jossa saatat joutua selittämään lisää riita-asioiden pito \> - **säästä**.</span><span class="sxs-lookup"><span data-stu-id="e4d73-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="e4d73-121">**Säilyttäminen:** Voit ottaa käyttöön mukautetut säilytys käytännöt, esimerkiksi säilyttää tietyn ajan tai poistaa sisällön pysyvästi säilytys ajan päätyttyä.</span><span class="sxs-lookup"><span data-stu-id="e4d73-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="e4d73-122">Lisä tietoja [on kohdassa säilytys käytäntöjen yleiskatsaus](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="e4d73-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-azure-information-protection-features"></a><span data-ttu-id="e4d73-123">Azure-tietojen suojaus ominaisuuksien määrittäminen</span><span class="sxs-lookup"><span data-stu-id="e4d73-123">Set up Azure Information Protection features</span></span>

<span data-ttu-id="e4d73-124">Azure Information Protection (AIP) auttaa luokittelemaan ja valinnaisesti suojaamaan asia kirjoja ja sähkö posteja käyttämällä tunnisteita.</span><span class="sxs-lookup"><span data-stu-id="e4d73-124">Azure Information Protection (AIP) helps you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="e4d73-125">Järjestelmänvalvojat voivat käyttää otsikoita automaattisesti, jos käyttäjät määrittävät säännöt ja ehdot manuaalisesti, tai käyttämällä yhdistelmää, jossa käyttäjille annetaan suosituksia.</span><span class="sxs-lookup"><span data-stu-id="e4d73-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="e4d73-126">Outlookissa verkossa voit käyttää seuraavia sisäänrakennettuja tarroja ja rajoituksia sähkö posteihin:</span><span class="sxs-lookup"><span data-stu-id="e4d73-126">In Outlook on the web you can apply the following built-in labels and restrictions to your emails:</span></span>
  
- <span data-ttu-id="e4d73-127">**Älä välitä**: vastaanottajat voivat lukea viestin, mutta he eivät voi välittää, tulostaa tai kopioida sisältöä</span><span class="sxs-lookup"><span data-stu-id="e4d73-127">**Do Not Forward**: Recipients can read the message, but they can't forward, print, or copy content</span></span>
    
- <span data-ttu-id="e4d73-128">**Salaa**: koko viesti on salattu.</span><span class="sxs-lookup"><span data-stu-id="e4d73-128">**Encrypt**: The entire message is encrypted.</span></span> <span data-ttu-id="e4d73-129">Vastaanottajien on vahvistettava henkilöllisyytensä ennen salatun sisällön käyttämistä, eivätkä ne voi poistaa salausta.</span><span class="sxs-lookup"><span data-stu-id="e4d73-129">Recipients must confirm their identity before accessing encrypted content and can't remove encryption.</span></span>
    
- <span data-ttu-id="e4d73-130">**Luottamuksellinen**: antaa organisaation työn tekijöille täydet oikeudet sähkö postin sisältöön ja liitteisiin, mutta ei organisaatiosi ulkopuolisille henkilöille.</span><span class="sxs-lookup"><span data-stu-id="e4d73-130">**Confidential**: Gives the employees in your organization full permissions to the email content and attachments, but not to people outside your organization.</span></span> <span data-ttu-id="e4d73-131">Tietojen omistajat voivat seurata ja kumota sisältöä missä tahansa vaiheessa.</span><span class="sxs-lookup"><span data-stu-id="e4d73-131">Data owners can track and revoke content at any point.</span></span>
    
- <span data-ttu-id="e4d73-132">**Erittäin luottamuksellinen**: tätä rajoitusta voidaan soveltaa erittäin luottamuksellisiin tietoihin, jolloin työn tekijät voivat tarkastella, muokata ja vastata, mutta eivät välittää, tulostaa tai kopioida tietoja.</span><span class="sxs-lookup"><span data-stu-id="e4d73-132">**Highly Confidential**: This restriction can be applied to highly confidential data, allowing employees to view, edit, and reply, but not forward, print, or copy the data.</span></span> <span data-ttu-id="e4d73-133">Tietojen omistajat voivat seurata ja kumota sisältöä missä tahansa vaiheessa.</span><span class="sxs-lookup"><span data-stu-id="e4d73-133">Data owners can track and revoke content at any point.</span></span>

### <a name="make-sure-azure-information-protection-is-activated"></a><span data-ttu-id="e4d73-134">Varmista, että Azure-tietojen suojaus on aktivoitu</span><span class="sxs-lookup"><span data-stu-id="e4d73-134">Make sure Azure Information Protection is activated</span></span>

<span data-ttu-id="e4d73-135">Voit varmistaa, että AIP on aktivoitu:</span><span class="sxs-lookup"><span data-stu-id="e4d73-135">To verify that AIP is activated :</span></span>

1. <span data-ttu-id="e4d73-136">Kirjaudu sisään [Azure-portaaliin](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="e4d73-136">Sign into [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="e4d73-137">Valitse **Kaikki palvelut** ja kirjoita *Azure-tietojen suojaus* **haku ruutuun**.</span><span class="sxs-lookup"><span data-stu-id="e4d73-137">Select **All services** and type in *Azure Information Protection* in the **Search Box**.</span></span>

3. <span data-ttu-id="e4d73-138">Kun tulokset ovat näytössä, napsauta Aloita **Azure-tietojen suoja** uksen vieressä, jotta se on suosikki ja helppo löytää myöhemmin.</span><span class="sxs-lookup"><span data-stu-id="e4d73-138">Once the results display, click the start next to **Azure Information Protection** to make it a favorite and easy to find later.</span></span>

4. <span data-ttu-id="e4d73-139">Valitse **Azure-tieto suoja** \> **uksen Akti vointi** ja varmista, että tilaksi on määritetty aktivoitu.</span><span class="sxs-lookup"><span data-stu-id="e4d73-139">Select **Azure Information Protection** \> **Protection activation** and make sure the status is set to activated.</span></span> 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a><span data-ttu-id="e4d73-140">Näytä Azure-tietojen suojaus käytäntö ja oletus otsikot</span><span class="sxs-lookup"><span data-stu-id="e4d73-140">View the Azure Information Protection policy and default labels</span></span> 

<span data-ttu-id="e4d73-141">Voit tarkastella ja muokata olemassa olevia otsikoita:</span><span class="sxs-lookup"><span data-stu-id="e4d73-141">To view, and modify, the existing labels:</span></span>

1. <span data-ttu-id="e4d73-142">Valitse Azure-tieto suojan koonti näytössä **luokitusten** \> **otsikot**.</span><span class="sxs-lookup"><span data-stu-id="e4d73-142">On the Azure Information Protection dashboard, select **Classifications** \> **Labels**.</span></span> <br/><span data-ttu-id="e4d73-143">![Azure-tietojen suoja uksen vakio merkinnät.](media/AIPLabels.png)</span><span class="sxs-lookup"><span data-stu-id="e4d73-143">![Standard labels for Azure Information Protection.](media/AIPLabels.png)</span></span>

2. <span data-ttu-id="e4d73-144">Voit valita minkä tahansa otsikon nähdäksesi vaihto ehtoja, voit muuttaa näyttö nimeä, värejä jne.</span><span class="sxs-lookup"><span data-stu-id="e4d73-144">You can choose any label to view options, you can change the display name, colors, etc.</span></span>
 
3. <span data-ttu-id="e4d73-145">Jos haluat luoda omia tunnisteita, katso [Muokkaa ja luo uusia tarroja](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) .</span><span class="sxs-lookup"><span data-stu-id="e4d73-145">See  [Modify and create new labels](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) if you want to create your own.</span></span> 

### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="e4d73-146">Azure-tieto suoja asiakkaan asentaminen manuaalisesti</span><span class="sxs-lookup"><span data-stu-id="e4d73-146">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="e4d73-147">Voit asentaa AIP-asiakkaan manuaalisesti:</span><span class="sxs-lookup"><span data-stu-id="e4d73-147">To manually install the AIP client:</span></span>

1. <span data-ttu-id="e4d73-148">Lataa **Azinfoprotection. exe** [Microsoft Download Centeristä](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="e4d73-148">Download **AzInfoProtection.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="e4d73-149">Voit varmistaa, että asennus on toiminut tarkastelemalla Word-asia kirjaa ja varmistamalla, että **suojaa** -vaihto ehto on käytettävissä **Aloitus** -väli lehdellä.</span><span class="sxs-lookup"><span data-stu-id="e4d73-149">You can verify that the installation worked by viewing a Word document and making sure that the **Protect** option is available on the **Home** tab.</span></span> <br/><span data-ttu-id="e4d73-150">![Word-asia kirjan avattava suojaus-väli lehti.](media/Word_Protect.png)</span><span class="sxs-lookup"><span data-stu-id="e4d73-150">![Protection tab drop-down in a Word document.](media/Word_Protect.png)</span></span>

<span data-ttu-id="e4d73-151">Lisä tietoja [on kohdassa asiakkaan asentaminen](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="e4d73-151">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
