---
title: Microsoft 365 Businessin käytön aloittaminen
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Opettele Microsoft 365 Businessin perustamista.
ms.openlocfilehash: 32bb30208083c4f62dd449290a7c9f5d8c725631
ms.sourcegitcommit: c5ca71d6feb0f033b50ccd4de816fd59b0925007
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/04/2019
ms.locfileid: "39831409"
---
# <a name="get-started-with-microsoft-365-business"></a>Microsoft 365 Businessin käytön aloittaminen

## <a name="what-is-microsoft-365-business"></a>Mikä Microsoft 365 Business on?

Microsoft 365 Business on kattava joukko yritysten tuottavuus-ja yhteistyötyökaluja, kuten Outlook, Word, Excel ja muut Office-tuotteet, jotka ovat aina ajan tasalla. Voit suojata työtiedostojasi kaikissa iOS-, Android-ja Windows 10-laitteissa yritys tason suoja uksen avulla, jota on helppo hallita.

Katso tästä videosta nopea yleiskatsaus Microsoft 365-liike toiminnan.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 Business on tarkoitettu jopa 300 lisensseihin. Jos tarvitset lisää käyttö oikeuksia, Katso lisä tietoja [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) -dokumentaatiosta. 
  
## <a name="get-microsoft-365-business"></a>Microsoft 365 Businessin hankkiminen

- Jos sinulla on kumppani, he saavat Microsoft 365 Business: [Hanki microsoft 365 Business Microsoft Partner Centeristä](get-microsoft-365-business.md).
    
- Jos sinulla ei ole kumppania ja haluat hankkia Microsoft 365 Business:n, [osta se täältä](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Microsoft 365 Businessin määrittäminen

 **Yleistä Microsoft 365 Business Suiten määrittämisestä**
  
Seuraavassa kaaviossa kerrotaan, miten järjestelmänvalvojat voivat määrittää Microsoft 365 Businessin. Siinä kuvataan myös Windows-tietokoneiden valmistelemisen vaiheet Microsoft 365 Business:ää varten. Voit myös lisätä uusia laitteita Microsoft 365 Business-hallinta keskukseen [Windowsin automaatti ohjauksen](add-autopilot-devices-and-profile.md)avulla. Voit määrittää ja esimäärittävät uusia laitteita automaatti ohjauksen avulla niin, että ne ovat valmiita tuottavaan käyttöön heti, kun käyttäjä kirjautuu sisään Microsoft 365-yrityksen tunniste tiedoilla.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Katso tästä videosta yleiskatsaus Microsoft 365-liike toiminnan asennukseen.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jos olet löytänyt tämän videon hyödyllisiksi, tutustu [koko koulutus sarjaan pien yrityksille ja niille, jotka ovat Microsoft 365-yrityksen uusia](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Määritä Microsoft 365 Business (järjestelmänvalvoja)

Kirjaudu sisään [microsoft 365 Business-hallinta keskukseen](https://portal.office.com/adminportal/home) , jossa on yleiset järjestelmänvalvojan tunniste tiedot, ja suorita seuraavat vaiheet, kun haluat määrittää Microsoft 365 Businessin. 
  
1. [Edellytykset tietojen suojaamiseksi laitteille, joissa on Microsoft 365 Business](pre-requisites-for-data-protection.md)
    
    Lue ensin edellytykset varmistaaksesi, että laitteesi ovat valmiita Microsoft 365-liike toimintaa varten.
    
2. [Microsoft 365 Businessin määrittäminen ohjatun asennus toiminnon avulla](set-up.md)
    
    Jos siirryt **pysyvästi paikallisesta Active Directorysta pilvi palveluun**, voit siirtyä Microsoft 365 Business-hallinta keskukseen ja lisätä käyttäjiä manuaalisesti ohjatun asennus toiminnon avulla tai voit SYNKRONOIDA Azure AD Connectin kanssa yhden kerran. Tämän voi tehdä kahdella eri tavalla: 
    
    - Jos sinulla on myös Exchange 2010-, Exchange 2013-tai Exchange 2016-palvelin, voit [nopeasti siirtää Exchange-posti laatikot Office 365-palvelimeen minimaalisen hybridi](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef)-sovelluksen avulla. Minimaaliset hybridi vaiheet sisältävät käyttäjien kerta synkronoinnin Azure ADIIN ja sähkö postin siirron paikallisesta pilvi palvelusta. Kun sähkö postin siirto on suoritettu, hakemiston synkronointi poistetaan automaattisesti käytöstä, kun käytät tätä menetelmää.
    
    - Synkronoi käyttäjät pilveen ohjatun Office 365 Directory Sync-toiminnon avulla. Suorita prosessi loppuun [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) -artikkelin ohjeiden mukaisesti. Kun olet synkronoitu käyttäjät pilvi palveluun, sinun on [sammutettu hakemiston synkronointi Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Sinun on myös annettava jokaiselle käyttäjälle, joka on lisätty tällä tavalla lisenssin Microsoft 365 Business. Voit tehdä tämän [ohjatussa asennuksessa](set-up.md) tai voit [määrittää käyttäjille käyttö oikeuksia Office 365 for Businessissa](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: mobiililaitteiden valmisteleminen

Noudata [microsoft 365-yritys käyttäjien mobiililaitteiden määrittäminen](set-up-mobile-devices.md) -ohjeita ja asenna Office-sovellukset laitteisiin ja varmista, että ne ovat Microsoft 365 Businessin suojaamassa. 
  
### <a name="3-prepare-pcs"></a>3: Valmistele tieto koneet

Järjestelmänvalvojat voivat valita uuden Windows 10-tieto koneen asetukset [Windowsin automaatti ohjauksen](add-autopilot-devices-and-profile.md)avulla. Käyttäjät voivat määrittää nykyiset tai uudet Windows 10-laitteet noudattamalla tämän ohje aiheen ohjeita: [Windows-tieto koneiden määrittäminen Microsoft 365-yritys käyttäjille](set-up-windows-devices.md). Aiemmin luotujen laitteiden käyttäjät voivat **vaihtoehtoisesti** [siirtää tiedostoja OneDrive for Businessille](move-files-to-onedrive.md). He voivat myös käyttää kolmannen osapuolen työkaluja siirtää tiedostoja, jotka liittyvät Windows-profiilin OneDrive.
  
Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Businessin suojaamaan Windows 10-laitteitasi samalla, kun ylläpidämme paikallisen todennuksen edellyttävien paikallisten resurssien käyttö oikeuksia. Määritä Microsoft 365 Business, jotta voit määrittää tämän noudattamalla [toimi alueeseen liittyneiden Windows 10-laitteiden käyttöönotto](manage-windows-devices.md) ohjeita. Tämä menetelmä on ensisijainen, ja laitteet tässä tilassa kutsutaan **hybridi Azure AD liitetyt laitteet**. 
  
Jos säilytät paikallisen Active Directoryn, joka sisältää joitakin paikallisia resursseja (kuten tiedosto resursseja ja tulostimia), voit antaa **Azure AD-liitettyjen laitteiden** käyttää näitä resursseja noudattamalla seuraavia vaiheita: paikallisten [resurssien käyttö Azure AD-liitetystä laitteesta Microsoft 365-liike toiminnassa](access-resources.md).
  
  
## <a name="contact-support"></a>Ota yhteyttä tukeen

 **Jos sinun täytyy ottaa yhteyttä tukeen:**
  
- Ota yhteyttä kumppaniin.
    
- Microsoft 365 Business Adminissa voit käyttää asiakas tuki tiimiä: ** [Ota yhteyttä yritys tuotteiden tukeen-järjestelmänvalvojan ohjeet](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="see-also"></a>Katso myös

[Microsoft 365 Businessin ohjeet ja resurssit](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Microsoft 365 Businessin hallinta](manage.md)[Microsoft 365 Businessin hallinta](migrate-to-microsoft-365-business.md)

[Microsoft 365-liike toiminnan koulutus videot](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
