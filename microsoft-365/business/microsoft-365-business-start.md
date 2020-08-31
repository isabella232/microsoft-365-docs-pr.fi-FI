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
description: Tietoja Microsoft 365 for Businessista, sen määrittämisestä ja käyttäjien laitteiden ja tieto koneiden valmistelemisesta sen varmistamiseksi, että ne ovat suojattuja Microsoft 365 for Businessissa.
ms.openlocfilehash: ec50036f589cfd8497b0e7e9af6519b30d25dcd3
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306485"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Microsoft 365 for Businessin käytön aloittaminen

## <a name="what-is-microsoft-365-for-business"></a>Mikä on Microsoft 365 for Business

Microsoft 365 for Business on kattava joukko yrityksen tuottavuutta ja yhteiskäyttötyökaluja, kuten Outlook, Word, Excel ja muut Office-tuotteet, jotka ovat aina ajan tasalla. Voit suojata työtiedostosi kaikissa iOS-, Android-ja Windows 10-laitteissa, joissa on helppo hallita yritys tason suojausta.

Katsomalla tämän videon saat nopeasti yleiskatsauksen Microsoft 365 for Businessista.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 for Business on tarkoitettu enintään 300-käyttö oikeuksien käyttöön. Jos tarvitset enemmän käyttöoikeuksia, saat lisätietoja [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) -ohjeista. 
  
## <a name="get-microsoft-365-for-business"></a>Microsoft 365 for Businessin hankkiminen

- Jos sinulla on partneri, he saavat Microsoft 365 for Businessin: [saat microsoft 365 for Businessin Microsoft-yhteistyökeskuksen](get-microsoft-365-business.md)kautta.
    
- Jos sinulla ei ole kumppania ja haluat hankkia Microsoft 365 for Businessin, voit [ostaa sen täältä](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-for-business"></a>Microsoft 365 for Businessin määrittäminen

 **Yleistä Microsoft 365 for Business Suiten määrittämisestä**
  
Seuraavassa kaaviossa kerrotaan, miten järjestelmänvalvojat määrittävät Microsoft 365 for Businessin. Artikkelissa kuvataan myös Microsoft 365 for Businessin Windows-tieto koneiden valmistelu vaiheet. Voit myös lisätä uusia laitteita Microsoft 365-hallinta keskukseen [Windowsin AutoPilot](add-autopilot-devices-and-profile.md)-palveluiden avulla. Automaatti ohjauksen avulla voit määrittää ja määrittää uusia laitteita niin, että ne ovat valmiita käytettäväksi heti, kun käyttäjä kirjautuu sisään Microsoft 365 for Businessin tunniste tiedoilla.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Katsomalla tämän videon saat yleiskatsauksen Microsoft 365 for Businessin asennuksesta.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: Microsoft 365 for Businessin määrittäminen (järjestelmänvalvoja)

Kirjaudu sisään [microsoft 365-hallinta keskukseen](https://portal.office.com/adminportal/home) käyttämällä yleisiä järjestelmänvalvojan tunniste tietoja ja määritä Microsoft 365 for Businessin asetukset suorittamalla seuraavat vaiheet. 
  
1. [Laitteiden tietojen suojaamisen edellytykset Microsoft 365 for Businessin avulla](pre-requisites-for-data-protection.md)
    
    Lue ensin edellytykset varmistaaksesi, että laitteesi ovat valmiita Microsoft 365 for Businessiin.
    
2. [Microsoft 365 for Businessin määrittäminen ohjatun määritys toiminnon avulla](set-up.md)
    
    Jos siirryt **pysyvästi paikallisesta Active Directorysta pilvi palveluun**, voit siirtyä Microsoft 365-hallinta keskukseen ja lisätä käyttäjät manuaalisesti ohjatun määritys toiminnon avulla tai voit tehdä kerta synkronoinnin Azure AD Connectin avulla. Tämän voi tehdä kahdella eri tavalla: 
    
    - Jos sinulla on myös Exchange 2010-, Exchange 2013-tai Exchange 2016-palvelin, voit [nopeasti siirtää Exchange-posti laatikot Microsoft 365: een käyttämällä pientä yhdistelmä](https://docs.microsoft.com/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate)-vaihto kurssia. Minimaalinen yhdistelmä vaihe sisältää kertaluontoisen synkronoinnin käyttäjien Azure AD:hen ja sähkö postin siirron paikallisesta pilvi palveluun. Kun sähkö postin siirto on valmis, hakemisto synkronointi poistetaan automaattisesti käytöstä, kun käytät tätä tapaa.
    
    - Synkronoi käyttäjät pilvi palveluun ohjatun hakemisto synkronoinnin avulla. Suorita tämä prosessi noudattamalla artikkelissa [Microsoft 365-hakemisto synkronoinnin määrittäminen](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) annettuja ohjeita. Kun synkronoit käyttäjät pilvi palveluun, sinun on [poistettava Microsoft 365 hakemisto synkronointi käytöstä](https://docs.microsoft.com/microsoft-365/enterprise/turn-off-directory-synchronization).
    
    Sinun on myös annettava jokaiselle käyttäjälle, joka on lisätty tällä tavoin Microsoft 365 for Businessin käyttö oikeus. Voit tehdä tämän [ohjatussa määritys toiminnossa](set-up.md) tai voit [määrittää käyttäjille käyttö oikeuksia](../admin/manage/assign-licenses-to-users.md).
    
### <a name="2-prepare-mobile-devices"></a>2: mobiililaitteiden valmistelu

Asenna Office-sovellukset laitteisiin ja varmista, että ne on suojattu Microsoft 365 for Businessissa, noudattamalla artikkelissa [microsoft 365 for Business-käyttäjien mobiililaitteiden määrittäminen](set-up-mobile-devices.md) annettuja ohjeita. 
  
### <a name="3-prepare-pcs"></a>3: tieto koneen valmistelu

Järjestelmänvalvojat voivat esivalita uuden Windows 10-tieto koneen asetukset [Windowsin AutoPilot](add-autopilot-devices-and-profile.md)-toiminnolla. Käyttäjät voivat määrittää nykyiset tai uudet Windows 10-laitteet noudattamalla tämän ohje aiheen ohjeita: Windows- [tieto koneiden määrittäminen Microsoft 365 for Businessin käyttäjille](set-up-windows-devices.md). Olemassa olevissa laitteissa käyttäjät voivat **vaihtoehtoisesti** [siirtää tiedostoja OneDrive for Businessiin](move-files-to-onedrive.md). He voivat myös käyttää kolmansien osapuolten työkaluja Windows-profiiliin liittyvien tiedostojen siirtämiseen OneDriveen.
  
Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 for Businessin suojaamaan Windows 10-laitteitasi säilyttäen kuitenkin paikalliset resurssit, jotka vaativat paikallisen todennuksen. Määritä tämän asetukset noudattamalla kohdan [Ota käyttöön toimi alue-yhdistetyt Windows 10-laitteet, joita Microsoft 365 for Business hallitsee](manage-windows-devices.md) . Tämä menetelmä on suositeltava, ja tämän tilan laitteet ovat nimeltään **Hybrid Azure AD-yhdistetyt laitteet**. 
  
Jos säilytän paikallisen Active Directoryn, joka sisältää joitakin paikallisia resursseja (kuten jaetut tiedosto resurssit ja tulostimet), voit antaa Azure AD:hen **liittyneille laitteillesi** oikeuden käyttää näitä resursseja noudattamalla seuraavia ohjeita: paikallisten [resurssien käyttäminen Azure AD-liittyneestä laitteesta Microsoft 365 for Businessissa](access-resources.md).
  
  
## <a name="contact-support"></a>Ota yhteyttä tukeen

 **Jos sinun täytyy ottaa yhteyttä tukeen:**
  
- Ota yhteyttä kumppaniin.
    
- Microsoft 365 for Business-järjestelmänvalvojalla on oikeus käyttää asiakas tuki tiimiään: ** [Ota yhteyttä yritys tuotteiden tukeen – järjestelmänvalvojan ohje](https://docs.microsoft.com/microsoft-365/admin/contact-support-for-business-products)**
    
## <a name="see-also"></a>Tutustu myös seuraaviin ohjeartikkeleihin:

[Microsoft 365 for Businessin ohjeet ja resurssit](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Hallitse microsoft 365 for Businessin](manage.md)[siirtoa Microsoft 365 for Businessiin](migrate-to-microsoft-365-business.md)

[Microsoft 365 for Business-koulutus videot](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
