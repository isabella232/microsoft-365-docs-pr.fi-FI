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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Opettele Microsoft 365 Businessin perustamista.
ms.openlocfilehash: 52e3167986bb7ed835762540e8076a3b9b2a0b56
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287631"
---
# <a name="get-started-with-microsoft-365-business"></a>Microsoft 365 Businessin käytön aloittaminen

## <a name="what-is-microsoft-365-business"></a>Mikä Microsoft 365 Business on?

Microsoft 365 Businessissa on kattava joukko yritysten tuottavuus- ja yhteiskäyttötyökaluja, joihin kuuluvat Outlook, Word, Excel ja muut Office-tuotteet, jotka ovat aina ajan tasalla. Voit suojata työtiedostojasi kaikissa iOS-, Android- ja Windows 10 -laitteissasi yritystason suojauksella, jota on helppo hallita.
  
Microsoft 365 Business on tarkoitettu enintään 300 käyttöoikeudelle. Jos tarvitset lisää käyttöoikeuksia, katso [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) -ohjeista lisätietoja. 
  
## <a name="get-microsoft-365-business"></a>Microsoft 365 Businessin hankkiminen

- Jos sinulla on kumppani, hän saa Microsoft 365 Business:n seuraavasti: [Hanki Microsoft 365 Business Microsoft-kumppanikeskuksesta](get-microsoft-365-business.md).
    
- Jos sinulla ei ole kumppania ja haluat hankkia Microsoft 365 Business:n, [osta se täältä](https://www.microsoft.com/en-us/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Microsoft 365 Businessin määrittäminen

 **Yleistä Microsoft 365 Business Suiten määrittämisestä**
  
Seuraavassa kaaviossa kerrotaan, miten järjestelmänvalvojat voivat määrittää Microsoft 365 Businessin. Siinä kuvataan myös Windows-tietokoneiden valmistelemisen vaiheet Microsoft 365 Business:ää varten. Voit myös lisätä uusia laitteita Microsoft 365 Business-hallintakeskukseen [Windows AutoPilotin](add-autopilot-devices-and-profile.md) avulla. Voit käyttää AutoPilotia myös uusien laitteiden määrittämiseen ja esimäärittämiseen, jolloin ne ovat käyttövalmiita heti, kun käyttäjä kirjautuu sisään Microsoft 365 Business-tunnistetiedoilla.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Määritä Microsoft 365 Business (järjestelmänvalvoja)

Kirjaudu sisään [Microsoft 365 Business -hallintakeskukseen](https://portal.office.com/adminportal/home) yleisen järjestelmänvalvojan tunnistetiedoillasi ja määritä Microsoft 365 Business noudattamalla seuraavia ohjeita. 
  
1. [Vaatimukset laitteiden tietojen suojaamiselle Microsoft 365 Businessin avulla](pre-requisites-for-data-protection.md)
    
    Lue ensin vaatimukset, jotta voit varmistaa, että laitteet ovat valmiita Microsoft 365 Business -pakettia varten.
    
2. [Microsoft 365 Businessin määrittäminen ohjatun määritystoiminnon avulla](set-up.md)
    
    Jos **siirrät pysyvästi paikallisesta Active Directorysta pilvi palveluun**, voit joko lisätä käyttäjät manuaalisesti Microsoft 365 Business-hallinta keskukseen ohjatun asennus toiminnon avulla tai voit tehdä yhden kerran synkronoinnin Azure AD Connectin kanssa. Tämän voi tehdä kahdella eri tavalla: 
    
  - Jos sinulla on myös Exchange 2010-, Exchange 2013-tai Exchange 2016-palvelin, voit [nopeasti siirtää Exchange-posti laatikot Office 365-palvelimeen minimaalisen hybridi](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef)-sovelluksen avulla. Minimal Hybrid -vaiheet sisältävät käyttäjien kertasynkronoinnin Azure AD:hen sekä sähköpostin siirron paikallisista järjestelmistä pilvipalveluun. Kun sähköpostin siirto on suoritettu, hakemistosynkronointi poistetaan automaattisesti käytöstä, kun tätä menetelmää käytetään.
    
  - Synkronoi käyttäjät pilvipalveluun Office 365:n ohjatun hakemistosynkronointitoiminnon avulla. Suorita prosessi loppuun [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) -artikkelin ohjeiden mukaisesti. Kun olet synkronoinut käyttäjät pilvipalveluun, sinun on [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Sinun täytyy myös määrittää kaikille tällä tavalla lisätyille käyttäjille Microsoft 365 Businessin käyttöoikeus. Voit tehdä tämän [ohjatussa asennus toiminnossa](set-up.md)tai [Määritä käyttö oikeudet käyttäjille Office 365 for Businessissa](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: mobiililaitteiden valmisteleminen

Noudata[microsoft 365-yritys käyttäjien mobiililaitteiden määrittäminen](set-up-mobile-devices.md) -ohjeita ja asenna Office-sovellukset laitteisiin ja varmista, että ne on suojattu Microsoft 365 Business-tieto koneessa. 
  
### <a name="3-prepare-pcs"></a>3: Valmistele tieto koneet

Järjestelmänvalvojat voivat valita uusien laitteiden asetukset Windows 10-tieto koneille [Windows AutoPilot](add-autopilot-devices-and-profile.md)-toiminnolla. Käyttäjät voivat määrittää nykyiset tai uudet Windows 10-laitteet noudattamalla tämän ohje aiheen ohjeita: [Windows-tieto koneiden määrittäminen Microsoft 365-yritys käyttäjille](set-up-windows-devices.md). Olemassa oleville laitteille käyttäjät voivat myös **valinnaisesti**[siirtää tiedostoja OneDrive for Business](move-files-to-onedrive.md). He voivat myös käyttää kolmannen osapuolen työkaluja siirtää tiedostoja, jotka liittyvät Windows-profiilin OneDrive.
  
Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Businessin suojaamaan Windows 10-laitteitasi samalla, kun ylläpidämme paikallisen todennuksen edellyttävien paikallisten resurssien käyttö oikeuksia. Määritä Microsoft 365 Business, jotta voit määrittää tämän noudattamalla [toimi alueeseen liittyneiden Windows 10-laitteiden käyttöönotto](manage-windows-devices.md) ohjeita. Tämä on ensisijainen menetelmä ja laitteet tässä tilassa kutsutaan **hybridi Azure AD liitetyt laitteet**. 
  
Jos säilytät paikallisen Active Directoryn, joka sisältää joitakin paikallisia resursseja (kuten tiedosto resursseja ja tulostimia), voit antaa **Azure AD-liitettyjen laitteiden** käyttää näitä resursseja noudattamalla seuraavia ohjeita: [paikallisten resurssien käyttö Azure AD-liitetty laite Microsoft 365 Business](access-resources.md).
  
Kun olet määrittänyt Windows 10-tieto koneet, voit [asentaa Officen automaattisesti](auto-install-or-uninstall-office.md) laitteisiin. 
  
## <a name="contact-support"></a>Ota yhteyttä tukeen

 **Jos sinun täytyy ottaa yhteyttä tukeen:**
  
- Ota yhteyttä kumppaniin.
    
- Microsoft 365 Business Adminissa voit käyttää asiakas tuki tiimiä, ** [ottaa yhteyttä yritys tuotteiden tukeen-järjestelmänvalvojan ohje](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="related-topics"></a>Aiheeseen liittyviä ohjeita
[Microsoft 365 Businessin ohjeet ja resurssit](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Microsoft 365 Businessin hallinta](manage.md)[Microsoft 365 Businessin hallinta](migrate-to-microsoft-365-business.md)
  

