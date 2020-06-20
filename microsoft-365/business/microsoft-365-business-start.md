---
title: Microsoft 365 for Businessin käytön aloittaminen
f1.keywords:
- NOCSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Lue tietoja Microsoft 365 for Businessista, sen määrittämisestä ja käyttäjien laitteiden ja tietokoneiden valmistelemisesta, jotta Microsoft 365 for Business suojaa niitä.
ms.openlocfilehash: 48a103333e101d545d562e7f2e9dd7329686f107
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/18/2020
ms.locfileid: "44786150"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Microsoft 365 for Businessin käytön aloittaminen

## <a name="what-is-microsoft-365-for-business"></a>Mikä on Microsoft 365 for Business

Microsoft 365 for Business on kattava joukko liiketoiminnan tuottavuus- ja yhteistyötyökaluja, kuten Outlook, Word, Excel ja muut Office-tuotteet, jotka ovat aina ajan tasalla. Voit suojata työtiedostot kaikilla iOS-, Android- ja Windows 10 -laitteillasi yritystason suojauksella, jota on helppo hallita.

Tämä video on nopea yleiskatsaus Microsoft 365 for Business -versiosta.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 for Business on tarkoitettu jopa 300 käyttöoikeuteen. Jos tarvitset enemmän käyttöoikeuksia, saat lisätietoja [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) -ohjeista. 
  
## <a name="get-microsoft-365-for-business"></a>Hanki Microsoft 365 for Business

- Jos sinulla on kumppani, he saavat Microsoft 365 for Businessin: [Hanki Microsoft 365 for Business Microsoft-kumppanikeskuksesta](get-microsoft-365-business.md).
    
- Jos sinulla ei ole kumppania ja haluat hankkia Microsoft 365 for Business, voit [ostaa sen täältä](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-for-business"></a>Microsoft 365 for Businessin määrittäminen

 **Microsoft 365 for business Suiten toiminnon yleiskatsaus**
  
Seuraavassa kaaviossa kuvataan, miten järjestelmänvalvojat määrittävät Microsoft 365 for Businessin. Artikkelissa kuvataan myös vaiheet Windows-tietokoneiden valmistelemiseksi Microsoft 365 for Business -käyttötarkoituksiin. Voit myös lisätä uusia laitteita Microsoft 365 -hallintakeskukseen [Windowsin automaattiohjauksella.](add-autopilot-devices-and-profile.md) Automaattisen pikatin avulla voit määrittää ja esimääritellä uusia laitteita niin, että ne ovat valmiita tuottavaan käyttöön heti, kun käyttäjä kirjautuu sisään Microsoft 365 for Business -tunnistetiedoillaan.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Tämä video on kohdassa Microsoft 365 for Businessin asennuksen yleiskatsaus.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: Microsoft 365 for Businessin määrittäminen (järjestelmänvalvoja)

Kirjaudu [Microsoft 365 -hallintakeskukseen](https://portal.office.com/adminportal/home) yleisillä järjestelmänvalvojan tunnistetiedoilla ja määritä Microsoft 365 for Business noudattamalla seuraavia ohjeita. 
  
1. [Microsoft 365 for Business -laitteiden tietojen suojaamisen edellytykset](pre-requisites-for-data-protection.md)
    
    Lue ensin edellytykset varmistaaksesi, että laitteesi ovat valmiita Microsoft 365 for Businessiin.
    
2. [Microsoft 365 for Businessin määrittäminen ohjatun asennustoiminnon avulla](set-up.md)
    
    Jos olet **pysyvästi siirtymässä paikallisesta Active Directorysta pilveen,** voit siirtyä Microsoft 365 -hallintakeskukseen ja lisätä käyttäjät manuaalisesti ohjatun asennustoiminnon avulla tai voit synkronoida käyttäjät kerran Azure AD Connectin kanssa. Tämän voi tehdä kahdella eri tavalla: 
    
    - Jos käytössäsi on myös Exchange 2010-, Exchange 2013- tai Exchange 2016 -palvelin, voit [siirtää Exchange-postilaatikot nopeasti Office 365:een Minimaalisen hybridin avulla.](https://docs.microsoft.com/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate) Minimaalisia hybridivaiheita ovat käyttäjien kertasynkronointi Azure AD:hen ja sähköpostin siirtäminen paikallisesta pilveen. Kun sähköpostin siirto on valmis, hakemistosynkronointi poistetaan automaattisesti käytöstä, kun käytät tätä menetelmää.
    
    - Synkronoi käyttäjät pilveen ohjatun hakemistosynkronoinnin avulla. Suorita tämä prosessi noudattamalla kohdan [Microsoft 365 hakemistosynkronoinnin määrittäminen](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) ohjeita. Kun olet synkronoinut käyttäjät pilveen, sinun on [kuittaattava office 365:n hakemistosynkronointi käytöstä.](https://docs.microsoft.com/office365/enterprise/turn-off-directory-synchronization)
    
    Sinun on myös annettava jokaiselle tällä tavalla lisätylle käyttäjälle käyttöoikeus Microsoft 365 for Businessiin. Voit tehdä tämän [ohjatussa asennustoiminnossa](set-up.md) tai [määrittää käyttöoikeuksia Microsoft 365 for Businessin käyttäjille.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)
    
### <a name="2-prepare-mobile-devices"></a>2: Mobiililaitteiden valmisteleminen

Noudata kohdan [Mobiililaitteiden määrittäminen Microsoft 365 for Business -käyttäjille](set-up-mobile-devices.md) ohjeita Office-sovellusten asentamiseksi laitteisiin ja niiden suojaamiseksi Microsoft 365 for Businessissa. 
  
### <a name="3-prepare-pcs"></a>3: Valmistele tietokoneet

Järjestelmänvalvojat voivat esivalita uusien Windows 10 -tietokoneiden asetukset [Windowsin automaattiohjauksen](add-autopilot-devices-and-profile.md)avulla. Käyttäjät voivat määrittää olemassa olevat tai uudet Windows 10 -laitteensa noudattamalla tämän ohjeaiheen ohjeita: [Windows-tietokoneiden määrittäminen Microsoft 365 yrityskäyttäjille](set-up-windows-devices.md). Nykyisissä laitteissa käyttäjät voivat **halutessaan** [siirtää tiedostoja OneDrive for Businessiin](move-files-to-onedrive.md). He voivat myös siirtää Windows-profiiliin liittyviä tiedostoja OneDriveen muiden valmistajien työkalujen avulla.
  
Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 for Businessin suojaamaan Windows 10 -laitteita säilyttäen samalla paikallisen todennuksen edellyttävien paikallisten resurssien käytön. Määritä tämä noudattamalla kohdan [Salli toimialueisiin liitettyjen Windows 10 -laitteiden hallintaa .](manage-windows-devices.md) Tätä menetelmää suositellaan, ja tämän tilan laitteita kutsutaan **Hybrid Azure AD -liitetyiksi laitteeksi**. 
  
Jos säilytät paikallisen Active Directoryn, joka sisältää joitakin paikallisia resursseja (kuten jaettuja tiedostoresursseja ja tulostimia), voit antaa **Azure AD-liitetyille laitteillesi** näiden resurssien käyttöoikeuden noudattamalla seuraavia ohjeita: [Azure AD-liitetyn laitteen paikallisten resurssien käyttäminen Microsoft 365 for Businessissa](access-resources.md).
  
  
## <a name="contact-support"></a>Ota yhteyttä tukeen

 **Jos sinun täytyy ottaa yhteyttä tukeen:**
  
- Ota yhteyttä kumppaniin.
    
- Microsoft 365 for business -järjestelmänvalvojana voit käyttää asiakastukitiimiämme: ** [Ota yhteyttä yritystuotteiden tukeen - Järjestelmänvalvojan ohjeet](https://docs.microsoft.com/microsoft-365/admin/contact-support-for-business-products)**
    
## <a name="see-also"></a>Tutustu myös seuraaviin ohjeaiheisiin

[Microsoft 365 yritysdokumentaatiolle ja resursseille](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Microsoft 365 for Businessin hallinta](manage.md)[Siirry Microsoft 365 for Businessiin](migrate-to-microsoft-365-business.md)

[Microsoft 365 yritysten koulutus videoita](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
