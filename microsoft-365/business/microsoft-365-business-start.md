---
title: Microsoft 365 käytön aloittaminen
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Lue Microsoft 365 yritysasiakkaista, sen määritämisistä ja käyttäjien laitteiden ja tietokoneiden valmisteleminen sen varmistamiseksi, että Microsoft 365 suojattu yritysasiakkaille.
ms.openlocfilehash: be5f0e74b71f412bf647e4ef0e496cd932fc306a
ms.sourcegitcommit: a05f61a291eb4595fa9313757a3815b7f217681d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/29/2021
ms.locfileid: "52706454"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Microsoft 365 käytön aloittaminen

## <a name="what-is-microsoft-365-for-business"></a>Mikä Microsoft 365 yrityksille?

Microsoft 365 yrityksille on kattava joukko yritysten tuottavuus- ja yhteiskäyttötyökaluja, kuten Outlook, Word, Excel ja muut Office tuotteet, jotka ovat aina ajan tasalla. Voit suojata työtiedostot kaikissa iOS-, Android- ja Windows 10-laitteissa yritystason suojauksen avulla, jota on helppo hallita.

## <a name="watch-what-is-microsoft-365-business-premium"></a>Katso: Mikä on Microsoft 365 Business Premium

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 yrityksille on tarkoitettu enintään 300 käyttöoikeutta. Jos tarvitset enemmän käyttöoikeuksia, saat lisätietoja [Microsoft 365 Enterprise](../enterprise/index.yml) -ohjeista. 
  
## <a name="get-microsoft-365-for-business"></a>Hanki Microsoft 365 yrityksille

- Jos sinulla on kumppani, hän saa Microsoft 365: [Hanki Microsoft 365 yritysasiat Microsoftin kumppanikeskuksesta.](get-microsoft-365-business.md)
    
- Jos sinulla ei ole kumppania ja haluat hankkia Microsoft 365, voit ostaa [sen täältä](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-for-business"></a>Yrityksen Microsoft 365 2010:n määritäminen

 **Microsoft 365 for Business Suiten määritetään yleiskatsaus**
  
Seuraavassa kaaviossa kuvataan, miten järjestelmänvalvojat Microsoft 365 yrityksen käyttöön. Artikkelissa kuvataan myös, miten tietokoneita Windows valmistellaan Microsoft 365 yrityksille. Voit myös lisätä uusia laitteita Microsoft 365 [autopilotin Windows avulla.](add-autopilot-devices-and-profile.md) AutoPilotilla voit määrittää ja määrittää uudet laitteet valmiiksi niin, että ne ovat käyttövalmiita heti, kun käyttäjä kirjautuu sisään Microsoft 365 yritystietoja varten.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

## <a name="watch-set-up-microsoft-365-business"></a>Katso: Microsoft 365 Business

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](../business-video/index.yml).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: yritysportaalin Microsoft 365 (järjestelmänvalvoja)

Kirjaudu Microsoft 365 [hallintakeskukseen yleisen](https://portal.office.com/adminportal/home) järjestelmänvalvojan tunnistetiedoilla ja määritä yritysportaalin asetukset Microsoft 365 ohjeiden mukaisesti. 
  
1. [Laitteiden tietojen suojaamisen edellytykset Microsoft 365 yritysasiat](pre-requisites-for-data-protection.md)
    
    Lue ensin edellytykset, jotta voit varmistaa, että laitteet ovat valmiita Microsoft 365 yritystoimintaa varten.
    
2. [Yrityskäyttöön Microsoft 365 määrittäminen ohjatun määritystoiminnon avulla](set-up.md)
    
    Jos siirryt pysyvästi paikallisesta **Active Directorysta** pilvipalveluun, siirry Microsoft 365-hallintakeskukseen ja lisää käyttäjät manuaalisesti ohjatun määritystoiminnon avulla tai voit tehdä kertasynkronoinnin Azure AD Näyttöyhteys. Tämän voi tehdä kahdella eri tavalla: 
    
    - Jos käytössäsi on myös Exchange 2010-, Exchange 2013- tai Exchange 2016 -palvelin, voit siirtää Exchange postilaatikot [Microsoft 365.](/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate) Minimal Hybrid -vaiheita ovat esimerkiksi käyttäjien kertasynkronoinnin Azure AD:lle ja sähköpostin siirto paikallisesta pilvipalveluun. Kun sähköpostin siirto on valmis, hakemistosynkronointi poistetaan automaattisesti käytöstä, kun käytät tätä menetelmää.
    
    - Synkronoi käyttäjät pilvipalveluun ohjatun hakemistosynkronoinnin avulla. Suorita prosessi [loppuun noudattamalla Microsoft 365](../enterprise/set-up-directory-synchronization.md) hakemistosynkronoinnin määrittäminen. Kun olet synkronoinut käyttäjät pilvipalveluun, sinun on poistettava hakemistosynkronointi [käytöstä Microsoft 365.](../enterprise/turn-off-directory-synchronization.md)
    
    Sinun on myös annettava kullekin tällä tavalla lisätylle käyttäjälle käyttöoikeus Microsoft 365 yrityksille. Voit tehdä tämän ohjatussa [määritystoiminnossa](set-up.md) tai voit [määrittää käyttöoikeuksia käyttäjille.](../admin/manage/assign-licenses-to-users.md)
    
### <a name="2-prepare-mobile-devices"></a>2: Mobiililaitteiden valmistelu

Asenna Office-sovellukset [laitteisiisi noudattamalla](set-up-mobile-devices.md) Microsoft 365 mobiililaitteiden Microsoft 365 yrityskäyttäjille -ohjeen ohjeita. 
  
### <a name="3-prepare-pcs"></a>3: Tietokoneiden valmistelu

Järjestelmänvalvojat voivat valita uusien tietokoneiden asetukset Windows 10 autopilotin Windows [avulla.](add-autopilot-devices-and-profile.md) Käyttäjät voivat määrittää nykyiset tai uudet Windows 10-laitteensa noudattamalla tämän ohjeaiheen ohjeita: Windows tietokoneiden Microsoft 365 [yrityskäyttäjille.](set-up-windows-devices.md) Aiemmin luoduissa laitteissa käyttäjät **voivat halutessaan** [siirtää tiedostoja OneDrive for Business.](move-files-to-onedrive.md) He voivat myös käyttää kolmannen osapuolen työkaluja Windows profiiliin OneDrive.
  
Jos organisaatiosi käyttää Windows Server Active Directorya paikallisesti, voit määrittää Microsoft 365 for Businessin suojaamaan Windows 10-laitteitasi säilyttäen edelleen paikallisen todentamisen edellyttävän paikallisen todentamisen resurssien käyttöoikeuden. Määritä tämä noudattamalla [ohjeita, jotka Windows 10 toimialueisiin](manage-windows-devices.md) liitettyjen laitteiden hallinta Microsoft 365 for Businessissa. Tämä menetelmä on ensisijainen, ja tässä tilassa oleetut laitteet kutsutaan **Azure AD-yhdistelmäympäristön laitteisiin.** 
  
Jos säilytät paikallisen Active Directoryn, joka sisältää paikallisia resursseja (kuten jaetut tiedostot ja tulostimet), voit antaa Azure AD:lle liitettyjen laitteiden käyttöoikeudet näihin resursseihin noudattamalla seuraavia ohjeita: Paikallisten resurssien käyttäminen Azure AD:llä yhdistetystä [laitteesta Microsoft 365 for Businessissa.](access-resources.md) 
  
  
## <a name="contact-support"></a>Ota yhteyttä tukeen

 **Jos sinun täytyy ottaa yhteyttä tukeen:**
  
- Ota yhteyttä kumppaniin.
    
- Yrityksen Microsoft 365 järjestelmänvalvojana voit käyttää asiakastukitiimiämme: Ota yhteyttä **[business-tuotteiden tukeen – järjestelmänvalvojan ohje](../business-video/get-help-support.md)**
    
## <a name="related-content"></a>Aiheeseen liittyvä sisältö

[Microsoft 365 for Businessin ohjeet ja resurssit](./index.yml) (linkkisivu)\
[Hallitse Microsoft 365 yrityksille](manage.md) (artikkeli)\
[Siirtyminen Microsoft 365 yrityksille](migrate-to-microsoft-365-business.md) (artikkeli)\
[Microsoft 365 yrityksille 2010 -koulutusvideoita](../business-video/index.yml) (linkkisivu)