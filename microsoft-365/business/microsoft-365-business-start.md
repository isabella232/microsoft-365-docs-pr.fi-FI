---
title: Microsoft 365 Businessin käytön aloittaminen
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
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Lue tietoja Microsoft 365 Businessista, sen määrittämisestä ja käyttäjien laitteiden ja tietokoneiden valmistelemisesta varmistamaan, että Microsoft 365 Business suojaa niitä.
ms.openlocfilehash: 220fb747e2bc501f3f6d46d967b30d2e5fd79a4a
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561436"
---
# <a name="get-started-with-microsoft-365-business"></a>Microsoft 365 Businessin käytön aloittaminen

## <a name="what-is-microsoft-365-business"></a>Mikä Microsoft 365 Business on?

Microsoft 365 Business on kattava joukko liiketoiminnan tuottavuus- ja yhteistyötyökaluja, kuten Outlook, Word, Excel ja muut Office-tuotteet, jotka ovat aina ajan tasalla. Voit suojata työtiedostosi kaikissa iOS-, Android- ja Windows 10 -laitteissa sijaisena, jota on helppo hallita yritystason suojauksella.

Tämä video opastaa nopeasti Microsoft 365 Businessissa.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 Business on tarkoitettu enintään 300 lisenssille. Jos tarvitset lisää käyttöoikeuksia, katso lisätietoja [Microsoft 365 Enterprisen](https://go.microsoft.com/fwlink/p/?linkid=860986) ohjeista. 
  
## <a name="get-microsoft-365-business"></a>Microsoft 365 Businessin hankkiminen

- Jos sinulla on kumppani, he saavat Microsoft 365 Business: [Hanki Microsoft 365 Business Microsoft Partner Centeristä](get-microsoft-365-business.md).
    
- Jos sinulla ei ole kumppania ja haluat hankkia Microsoft 365 Business:n, [osta se täältä](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Microsoft 365 Businessin määrittäminen

 **Microsoft 365 Business Suiten esittely**
  
Seuraavassa kaaviossa kuvataan, miten järjestelmänvalvojat ovat määrittänyt Microsoft 365 Businessin. Siinä kuvataan myös Windows-tietokoneiden valmistelemisen vaiheet Microsoft 365 Business:ää varten. Voit myös lisätä uusia laitteita Microsoft 365 Business -hallintakeskukseen [Windowsin automaattiohjauksen](add-autopilot-devices-and-profile.md)avulla. AutoPilotin avulla voit määrittää ja esimäärittää uusia laitteita niin, että ne ovat valmiita tuottavaan käyttöön heti, kun käyttäjä kirjautuu sisään Microsoft 365 Business -tunnistetiedoillaan.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Tämä video on yleiskuvaus Microsoft 365 Businessin asennuksesta.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Microsoft 365 Businessin määrittäminen (järjestelmänvalvoja)

Kirjaudu [Microsoft 365 Business -hallintakeskukseen](https://portal.office.com/adminportal/home) yleisillä järjestelmänvalvojan tunnistetiedoilla ja määritä Microsoft 365 Business seuraavasti. 
  
1. [Laitteiden tietojen suojaamisen edellytykset Microsoft 365 Businessilla](pre-requisites-for-data-protection.md)
    
    Lue ensin edellytykset ja varmista, että laitteesi ovat valmiita Microsoft 365 Businessiin.
    
2. [Microsoft 365 Businessin määrittäminen ohjatun asennustoiminnon avulla](set-up.md)
    
    Jos **siirryt pysyvästi paikallisesta Active Directorysta pilveen**, voit siirtyä Microsoft 365 Business -hallintakeskukseen ja lisätä käyttäjät ohjatun asennustoiminnon avulla manuaalisesti tai voit synkronoida azure AD Connectin kerran. Tämän voi tehdä kahdella eri tavalla: 
    
    - Jos käytössäsi on myös Exchange 2010-, Exchange 2013- tai Exchange 2016 -palvelin, voit [siirtää Exchange-postilaatikot nopeasti Office 365:een käyttämällä vähimmäishybridiä.](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef) Minimaalisiin hybridivaiheisiin kuuluu käyttäjien kertasynkronointi Azure AD:hen ja sähköpostin siirto paikallisesta pilveen. Kun sähköpostin siirto on valmis, hakemistosynkronointi poistetaan automaattisesti käytöstä, kun käytät tätä menetelmää.
    
    - Synkronoi käyttäjät pilveen käyttämällä office 365:n ohjatun kansion synkronointitoimintoa. Suorita prosessi loppuun [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) -artikkelin ohjeiden mukaisesti. Kun olet synkronoinut käyttäjät pilveen, sinun on [poistatava Office 365:n hakemistosynkronointi käytöstä](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Sinun on myös annettava jokaiselle käyttäjälle, joka on lisätty tällä tavalla, Microsoft 365 Business -käyttöoikeuden. Voit tehdä tämän [ohjatussa asennustoiminnossa](set-up.md) tai [määrittää käyttöoikeuksia käyttäjille Office 365 for Businessissa](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: Mobiililaitteiden valmisteleminen

Noudata ohjeita kohdassa [Mobiililaitteiden määrittäminen Microsoft 365 Business -käyttäjille,](set-up-mobile-devices.md) jotta Office-sovellukset voidaan asentaa laitteisiin, ja varmista, että Microsoft 365 Business suojaa niitä. 
  
### <a name="3-prepare-pcs"></a>3: Tietokoneiden valmisteleminen

Järjestelmänvalvojat voivat esivalita uusien Windows 10 -tietokoneiden asetukset [Windowsin automaattiohjauksen](add-autopilot-devices-and-profile.md)avulla. Käyttäjät voivat määrittää aiemmin luodut tai uudet Windows 10 -laitteensa noudattamalla tämän ohjeaiheen ohjeita: [Windows-tietokoneiden määrittäminen Microsoft 365 Business -käyttäjille](set-up-windows-devices.md). Käyttäjät voivat **halutessaan** [siirtää tiedostoja OneDrive for Businessiin olemassa olevissa](move-files-to-onedrive.md)laitteissa. He voivat myös käyttää kolmannen osapuolen työkaluja Windows-profiiliin liittyvien tiedostojen siirtämiseen OneDriveen.
  
Jos organisaatiosi käyttää paikallista Windows Server In Active Directorya, voit määrittää Microsoft 365 Businessin suojaamaan Windows 10 -laitteita säilyttäen samalla paikallisen todennuksen edellyttävien paikallisten resurssien käytön. Määritä tämä [noudattamalla kohdan Microsoft 365 Business hallinnoimien toimialueeseen liitettyjen Windows 10 -laitteiden ottaminen käyttöön.](manage-windows-devices.md) Tämä menetelmä on ensisijainen, ja tämän tilan laitteita kutsutaan **Hybridi Azure AD -liitetyiksi laitteiksi**. 
  
Jos säilytät paikallisen Active Directoryn, joka sisältää joitakin paikallisia resursseja (kuten jaettuja resursseja ja tulostimia), voit antaa **Azure AD-liitettyjen laitteiden** käyttää näitä resursseja noudattamalla seuraavia ohjeita: [Käytä paikallisia resursseja Microsoft 365 Businessin Azure AD-liitetystä laitteesta.](access-resources.md)
  
  
## <a name="contact-support"></a>Ota yhteyttä tukeen

 **Jos sinun täytyy ottaa yhteyttä tukeen:**
  
- Ota yhteyttä kumppaniin.
    
- Microsoft 365 Business -järjestelmänvalvojana voit käyttää asiakastukitiimiämme: ** [Ota yhteyttä yritystuotteiden tukeen - Järjestelmänvalvojan ohjeet](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="see-also"></a>Tutustu myös seuraaviin ohjeaiheisiin

[Microsoft 365 Businessin ohjeet ja resurssit](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Microsoft 365 Businessin hallinta](manage.md)[Microsoft 365 Businessin hallinta](migrate-to-microsoft-365-business.md)

[Microsoft 365 Business -koulutusvideot](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
