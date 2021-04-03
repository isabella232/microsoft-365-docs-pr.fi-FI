---
title: Microsoft 365 for Businessin käytön aloittaminen
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
description: Lue lisää Microsoft 365 for Businessista, sen määritämisistä ja käyttäjien laitteiden ja tietokoneiden valmistelemista sen varmistamiseksi, että Microsoft 365 for Business suojaa heitä.
ms.openlocfilehash: 83bd2ff87683c1ad810d20658ba20f3229408968
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580090"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Microsoft 365 for Businessin käytön aloittaminen

## <a name="what-is-microsoft-365-for-business"></a>Mikä on Microsoft 365 for Business?

Microsoft 365 for Business on kattava joukko yritysten tuottavuus- ja yhteiskäyttötyökaluja, kuten Outlook, Word, Excel ja muut Office-tuotteet, jotka ovat aina ajan tasalla. Voit suojata työtiedostot kaikissa iOS-, Android- ja Windows 10 -laitteissa yritystason suojauksen avulla, jota on helppo hallita.

Tässä videossa on lyhyt yleiskuvaus Microsoft 365 for Businessista.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 for Business on tarkoitettu enintään 300 käyttöoikeutta varten. Jos tarvitset enemmän käyttöoikeuksia, saat lisätietoja [Microsoft 365 Enterprise](../enterprise/index.yml) -ohjeista. 
  
## <a name="get-microsoft-365-for-business"></a>Hanki Microsoft 365 for Business

- Jos sinulla on kumppani, hän saa Microsoft 365 for Businessin: [Hanki Microsoft 365 for Business Microsoft-kumppanikeskuksesta.](get-microsoft-365-business.md)
    
- Jos sinulla ei ole kumppania ja haluat hankkia Microsoft 365 for Businessin, voit [ostaa sen täältä.](https://www.microsoft.com/microsoft-365/business)
    
## <a name="set-up-microsoft-365-for-business"></a>Microsoft 365 for Businessin määritäminen

 **Yleistä Microsoft 365 for Business Suite - määritästä**
  
Seuraavassa kaaviossa kuvataan, miten järjestelmänvalvojat ovat määrittänyt Microsoft 365 for Businessin. Artikkelissa kerrotaan myös vaiheista, miten Windows-tietokoneet valmistellaan Microsoft 365 for Businessia varten. Voit myös lisätä uusia laitteita Microsoft 365 -hallintakeskuksessa [Windows AutoPilotilla.](add-autopilot-devices-and-profile.md) Voit käyttää AutoPilotia uusien laitteiden määrittämiseen ja esimääritykseen, jotta ne ovat valmiina tuottavaan käyttöön heti, kun käyttäjä kirjautuu sisään Microsoft 365 for Business -tunnistetiedoillaan.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Tässä videossa on yleiskatsaus Microsoft 365 for Businessin määrityksestä.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: Microsoft 365 for Businessin määritäminen (järjestelmänvalvoja)

Kirjaudu [Microsoft 365](https://portal.office.com/adminportal/home) -hallintakeskukseen yleisen järjestelmänvalvojan tunnistetiedoilla ja määritä Microsoft 365 for Business noudattamalla seuraavia ohjeita. 
  
1. [Laitteiden tietojen suojaamisen edellytykset Microsoft 365 for Businessin avulla](pre-requisites-for-data-protection.md)
    
    Lue ensin edellytykset, jotta voit varmistaa, että laitteet ovat valmiina Microsoft 365 for Businessia varten.
    
2. [Microsoft 365 for Businessin määrittäminen ohjatun määritystoiminnon avulla](set-up.md)
    
    Jos olet siirtymässä pysyvästi paikallisesta **Active Directorysta** pilvipalveluun, siirry Microsoft 365 -hallintakeskukseen ja lisää käyttäjät manuaalisesti ohjatun määritystoiminnon avulla tai voit tehdä kertasynkronoinnin Azure AD Connectin kanssa. Tämän voi tehdä kahdella eri tavalla: 
    
    - Jos sinulla on myös Exchange 2010-, Exchange 2013- tai Exchange 2016 -palvelin, voit siirtää Exchange-postilaatikot [nopeasti Microsoft 365:lle Minimal Hybridin avulla.](/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate) Minimal hybrid steps include a one-time sync of users to Azure AD, and email migration from on-premises to the cloud. Kun sähköpostin siirto on valmis, hakemistosynkronointi poistetaan automaattisesti käytöstä, kun käytät tätä menetelmää.
    
    - Synkronoi käyttäjät pilvipalveluun ohjatun hakemistosynkronoinnin avulla. Suorita prosessi loppuun [noudattamalla microsoft 365:n](../enterprise/set-up-directory-synchronization.md) hakemistosynkronoinnin määrittäminen -kohdan ohjeita. Kun olet synkronoinut käyttäjät pilvipalveluun, sinun täytyy poistaa hakemistosynkronointi käytöstä [Microsoft 365:ssä.](../enterprise/turn-off-directory-synchronization.md)
    
    Sinun on myös annettava kullekin tällä tavalla lisätylle käyttäjälle Microsoft 365 for Business -käyttöoikeus. Voit tehdä tämän ohjatussa [määritystoiminnossa](set-up.md) tai [määrittää käyttäjille käyttöoikeuksia.](../admin/manage/assign-licenses-to-users.md)
    
### <a name="2-prepare-mobile-devices"></a>2: Mobiililaitteiden valmistelu

Asenna Office-sovellukset laitteisiin ja varmista, että [Microsoft 365 for](set-up-mobile-devices.md) Business on suojattu mobiililaitteille Microsoft 365 for Businessin avulla noudattamalla ohjeita. 
  
### <a name="3-prepare-pcs"></a>3: Tietokoneiden valmisteleminen

Järjestelmänvalvojat voivat valita uusien Windows 10 -tietokoneiden asetukset valmiiksi [Windows AutoPilotilla.](add-autopilot-devices-and-profile.md) Käyttäjät voivat määrittää nykyiset tai uudet Windows 10 -laitteensa noudattamalla tämän ohjeaiheen ohjeita: Windows-tietokoneiden määritetään [Microsoft 365 for Business -käyttäjille.](set-up-windows-devices.md) Aiemmin luoduissa laitteissa käyttäjät **voivat halutessaan** [siirtää tiedostoja OneDrive for Business -palveluun.](move-files-to-onedrive.md) He voivat myös siirtää Windows-profiiliin liittyviä tiedostoja OneDriveen kolmannen osapuolen työkalujen avulla.
  
Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 for Businessin suojaamaan Windows 10 -laitteitasi säilyttäen edelleen paikallisen todentamisen edellyttävän paikallisen todentamisen resurssien käyttöoikeuden. Määritä tämä noudattamalla ohjeita, jotka on annettu microsoft [365 for Businessin](manage-windows-devices.md) hallitsemaan toimialueeseen liittyneissä Windows 10 -laitteissa. Tämä menetelmä on ensisijainen, ja tässä tilassa laitteita kutsutaan Yhdistelmä azure AD:ksi **liitettyihin laitteisiin.** 
  
Jos säilytät paikallisen Active Directoryn, joka sisältää paikallisia resursseja (kuten jaetut tiedostot ja tulostimet), voit antaa **Azure AD:lle** liitettyjen laitteiden käyttöoikeudet näihin resursseihin seuraavasti: Käytä paikallisia resursseja Azure AD:llä yhdistetystä laitteesta Microsoft [365 for Businessissa.](access-resources.md)
  
  
## <a name="contact-support"></a>Ota yhteyttä tukeen

 **Jos sinun täytyy ottaa yhteyttä tukeen:**
  
- Ota yhteyttä kumppaniin.
    
- Microsoft 365 for Business -järjestelmänvalvojana voit käyttää asiakastukitiimiämme: ota yhteyttä **[yritystuotteiden tukeen – järjestelmänvalvojan ohje](../admin/contact-support-for-business-products.md)**
    
## <a name="see-also"></a>Tutustu myös seuraaviin ohjeartikkeleihin:

[Microsoft 365 for Businessin dokumentaatio ja resurssit](./index.yml)
  
[Microsoft 365 for Businessin hallinta Microsoft](manage.md)[365 for Businessiin](migrate-to-microsoft-365-business.md) siirtäminen

[Microsoft 365 for Business -koulutusvideot](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)