---
title: Microsoft 365 Businessin käytön aloittaminen
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Tietoja Microsoftin 365 liiketoiminnan.
ms.openlocfilehash: 78f7360c80667b8d34fad9d849cfc2cf83a8577b
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32278105"
---
# <a name="get-started-with-microsoft-365-business"></a>Microsoft 365 Businessin käytön aloittaminen

## <a name="what-is-microsoft-365-business"></a>Mikä Microsoft 365 Business on?

Microsoft 365 Businessissa on kattava joukko yritysten tuottavuus- ja yhteiskäyttötyökaluja, joihin kuuluvat Outlook, Word, Excel ja muut Office-tuotteet, jotka ovat aina ajan tasalla. Voit suojata työtiedostojasi kaikissa iOS-, Android- ja Windows 10 -laitteissasi yritystason suojauksella, jota on helppo hallita.
  
Microsoft 365 Business on tarkoitettu enintään 300 käyttöoikeudelle. Jos tarvitset lisää käyttöoikeuksia, katso [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) -ohjeista lisätietoja. 
  
## <a name="get-microsoft-365-business"></a>Microsoft 365 Businessin hankkiminen

- Jos sinulla on kumppani, hän saa Microsoft 365 Business:n seuraavasti: [Hanki Microsoft 365 Business Microsoft-kumppanikeskuksesta](get-microsoft-365-business.md).
    
- Jos sinulla ei ole kumppania ja haluat hankkia Microsoft 365 Business:n, [osta se täältä](https://www.microsoft.com/en-us/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Microsoft 365 Businessin määrittäminen

 **Määritä Microsoft 365 Business Suite yleiskatsaus**
  
Seuraavassa kaaviossa kuvataan, miten järjestelmänvalvojat Microsoft 365 Business. Siinä kuvataan myös Windows-tietokoneiden valmistelemisen vaiheet Microsoft 365 Business:ää varten. Voit myös lisätä uusia laitteita Microsoft 365 Business-hallintakeskukseen [Windows AutoPilotin](add-autopilot-devices-and-profile.md) avulla. Voit käyttää AutoPilotia myös uusien laitteiden määrittämiseen ja esimäärittämiseen, jolloin ne ovat käyttövalmiita heti, kun käyttäjä kirjautuu sisään Microsoft 365 Business-tunnistetiedoilla.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Microsoft 365 liiketoiminnan (Admin)

Kirjaudu sisään [Microsoft 365 Business -hallintakeskukseen](https://portal.office.com/adminportal/home) yleisen järjestelmänvalvojan tunnistetiedoillasi ja määritä Microsoft 365 Business noudattamalla seuraavia ohjeita. 
  
1. [Vaatimukset laitteiden tietojen suojaamiselle Microsoft 365 Businessin avulla](pre-requisites-for-data-protection.md)
    
    Lue ensin vaatimukset, jotta voit varmistaa, että laitteet ovat valmiita Microsoft 365 Business -pakettia varten.
    
2. [Microsoft 365 Businessin määrittäminen ohjatun määritystoiminnon avulla](set-up.md)
    
    Jos olet **pysyvästi siirtää pilvipalveluihin paikallisen Active Directory-hakemistopalvelusta**, voit joko lisätä käyttäjiä manuaalisesti Microsoft 365 Business admin Centerin ohjatun asennuksen avulla tai tehdä Azure AD Yhdistä kerta synkronointiin. Tämän voi tehdä kahdella eri tavalla: 
    
  - Jos myös Exchange 2010, Exchange-2013 tai Exchange 2016 server, voit [Käyttää mahdollisimman vähän Hybrid, jos haluat nopeasti siirtää Exchange-postilaatikoista Office 365: ssä](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). Minimal Hybrid -vaiheet sisältävät käyttäjien kertasynkronoinnin Azure AD:hen sekä sähköpostin siirron paikallisista järjestelmistä pilvipalveluun. Kun sähköpostin siirto on suoritettu, hakemistosynkronointi poistetaan automaattisesti käytöstä, kun tätä menetelmää käytetään.
    
  - Synkronoi käyttäjät pilvipalveluun Office 365:n ohjatun hakemistosynkronointitoiminnon avulla. Suorita prosessi loppuun [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) -artikkelin ohjeiden mukaisesti. Kun olet synkronoinut käyttäjät pilvipalveluun, sinun on [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Sinun täytyy myös määrittää kaikille tällä tavalla lisätyille käyttäjille Microsoft 365 Businessin käyttöoikeus. Voit tehdä tämän [ohjatun asennuksen](set-up.md)tai [määrittää käyttöoikeuksia käyttäjille Office 365 yrityksille](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: Valmistele kannettavien laitteiden

Laitteet ja varmista, että ne on suojattu 365 Microsoft Business Office apps asennettavaksi[Mobiililaitteiden käyttäjille Microsoft 365 Business määrittää](set-up-mobile-devices.md) noudattamalla. 
  
### <a name="3-prepare-pcs"></a>3: tietokoneiden valmisteleminen

Valvojat ennalta valita uusia laitteita Windows 10 PC: T-asetukset käyttämällä [Windowsin automaattiohjauksella](add-autopilot-devices-and-profile.md). Käyttäjät voivat määrittää Windows 10 nykyisten tai uusien laitteiden noudattamalla tämän ohjeaiheen: [Windows-tietokoneita Microsoft 365 Business käyttäjien määrittäminen](set-up-windows-devices.md). Olemassa olevat laitteet käyttäjät voivat myös **vaihtoehtoisesti**[siirtää tiedostoja liiketoiminnan OneDrive](move-files-to-onedrive.md). He voivat myös käyttää kolmannen osapuolen työkaluja voit siirtää tiedostoja Windows-profiilin OneDrive.
  
Jos organisaatiossa käytetään Windows Server Active Directory tiloissa, voit määrittää Microsoft 365 liiketoiminnan suojaamaan Windows 10-laitteet, säilyttäen kuitenkin edellyttää paikallista todennusta tiloissa resurssien käytön. Voit määrittää [toimialueeseen liittymistä Windows 10 laitteita voi hallita Microsoft 365 Business käyttöön](manage-windows-devices.md) noudattamalla. Tämä on ensisijainen menetelmä, ja tässä tilassa laitteita kutsutaan **hybridi Azure AD liitetyt laitteet**. 
  
Jos voit säilyttää paikallista Active Directory, joka sisältää joitakin tiloissa (kuten jaettujen tiedostoresurssien ja tulostinten), voit antaa näiden resurssien **Azure AD liittynyt laitteiden** käyttöä noudattamalla tässä: [käyttö paikalliset resurssit Microsoft 365 Business AD liitetty laite Azure](access-resources.md).
  
Sen jälkeen, kun olet määrittänyt Windows 10 PC voit [automaattisesti asentaa Office](auto-install-or-uninstall-office.md) laitteisiin. 
  
## <a name="contact-support"></a>Ota yhteyttä tukeen

 **Jos sinun täytyy ottaa yhteyttä tukeen:**
  
- Ota yhteyttä kumppaniin.
    
- Microsoft 365 Business järjestelmänvalvojana sinulla on pääsy asiakastukeemme, [yhteystieto tuki liiketoiminnan tuotteet - Ohje](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b) ****
    
## <a name="related-topics"></a>Aiheeseen liittyvät artikkelit
[Microsoft 365 Businessin ohjeet ja resurssit](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Microsoft 365 Businessin hallinta](manage.md)[Microsoft 365 Businessin hallinta](migrate-to-microsoft-365-business.md)
  

