---
title: Windows-laitteiden määrittäminen Microsoft 365 Business -käyttäjille
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: 'Opi määrittämään Windows laitteet Windows 10 Pro yrityskäyttäjille Microsoft 365. '
ms.openlocfilehash: 5efe3aa1e329e7a9edcfd49fcc1f1391f95fd97f
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074546"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a>Windows-laitteiden määrittäminen Microsoft 365 Business -käyttäjille

## <a name="prerequisites"></a>Edellytykset

Ennen kuin voit määrittää Windows-laitteet Microsoft 365 Business -käyttäjiä varten, varmista, että kaikissa Windows-laitteissa on Windows 10 Pro -versio 1703 (Creators-päivitys). Windows 10 Pro on edellytys Windows 10 Businessin käyttöönotolle. Se on joukko pilvipalveluja ja laitehallintaominaisuuksia, jotka täydentävät Windows 10 Pro -ohjelmistoa ja mahdollistavat Microsoft 365 Businessin keskitetyn valvonnan ja suojauksen hallinnan.
  
Jos käytössäsi on Windows-laitteita, joissa on Windows 7 Pro, Windows 8 Pro tai Windows 8.1 Pro, Microsoft 365 Business -tilaus oikeuttaa sinut Windows 10 -päivitykseen.
  
Lisätietoja Windows-laitteiden Windows 10 Pro Creators -päivityksen tekemisestä on tämän aiheen ohjeissa: [Windows Pro Creators -päivityksen tekeminen Windows-laitteisiin](upgrade-to-windows-pro-creators-update.md).
  
Lisätietoja, [Tarkista laite on yhdistetty Azure AD](#verify-the-device-is-connected-to-azure-ad) voit varmistaa päivityksen, tai varmista, että päivityksen, toimi. 
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Windows 10 -laitteiden liittäminen organisaatiosi Azure AD:hen

Kun organisaatiosi kaikkiin Windows-laitteisiin on joko päivitetty Windows 10 Pro Creators -päivitys tai niissä on jo alun perin ollut Windows 10 Pro Creators -päivitys, voit liittää kyseiset laitteet organisaatiosi Azure Active Directoryyn. Kun laitteet on liitetty, niihin päivitetään automaattisesti Windows 10 Business, joka on osa Microsoft 365 Business -tilaustasi.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Uusi tai päivitetty Windows 10 Pro -laite

Jos laite on uusi laite, jossa on Windows 10 Pro Creators -päivitys, tai laitteeseen on tehty Windows 10 Pro Creators -päivitys, mutta ei vielä Windows 10 -laitemääritystä, noudata seuraavia ohjeita.
  
1. Suorita Windows 10 -laitteen asennus, kunnes näyttöön tulee **Miten haluat määrittää?** -sivu. 
    
    ![On the How would you like to set up page, choose Set up for an organization](media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Valitse sitten **Määritä organisaatiolle** ja anna Microsoft 365 Business -käyttäjänimesi ja -salasanasi. 
    
3. Viimeistele Windows 10 -laitteen määritys.
    
   Kun olet valmis, käyttäjä yhdistetään organisaatiosi Azure AD:hen. Varmista tämä kohdan [Laitteen Azure AD -yhteyden tarkistaminen](#verify-the-device-is-connected-to-azure-ad) ohjeiden mukaan. 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>Laite, joka on jo määritetty ja jossa on Windows 10 Pro

 **Käyttäjien yhdistäminen Azure AD:hen:**
  
1. Valitse käyttäjän Windows-tietokoneessa, jossa on käytössä Windows 10 Pro -versio 1703 (Creators-päivitys) (katso [edellytykset](pre-requisites-for-data-protection.md)), Windows-näppäin ja valitse sitten Asetukset-kuvake.
  
   ![In the Start menu, click Windows Settings icon](media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. Vallitse **Asetukset** ja valitse sitten **Tilit**.
  
   ![In Windows Settings, go to Accounts](media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. Valitse **Omat tiedot** -sivulla **Käytä työpaikan tai koulun resursseja** \> **Yhdistä**.
  
   ![Choose Connect under Access work or school](media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. Valitse **Määritä työpaikan tai oppilaitoksen tili** -valintaikkunan **Vaihtoehtoiset toimet** -kohdassa **Liitä tämä laite Azure Active Directoryyn**.
  
   ![Click Join this device to Azure Active Directory](media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. Kirjoita **Kirjaudu sisään** -sivulla työpaikan tai oppilaitoksen tili \> **Seuraava**.
  
   Kirjoita salasana **Anna salasana** -sivulla \> **Kirjaudu**.
  
   ![Enter your work or school email on the Let's get you signed in page](media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. **Varmista, että tämä on yrityksen** sivulla Varmista, että tiedot ovat oikein ja valitse **Liity**.
  
   Valitse **Olet valmis!** -sivulla **Valmis**.
  
   ![On the Make sure this is your organization screen, click Join](media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Jos olet ladannut tiedostoja OneDrive for Businessiin, synkronoi ne takaisin. Jos olet siirtänyt profiilin ja tiedostot kolmannen osapuolen työkalun avulla, synkronoi myös ne uuteen profiiliin.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Laitteen Azure AD -yhteyden tarkistaminen

Tarkista synkronointitilasi napsauttamalla **Asetukset**-valintaikkunan **Käytä työpaikan tai koulun resursseja** -sivulla **Yhdistä kohteeseen** _ \<organization name\> _ -alueella, jolloin painikkeet **Tiedot** ja **Katkaise yhteys** tulevat näkyviin. Tuo synkronointitilasi näkyviin valitsemalla **Tiedot**. 
  
Valitse Synkronointitila-sivulla Synkronoi, jolloin saat uusimmat mobiililaitteiden hallintakäytännöt PC-tietokoneeseen.
  
Kun haluat aloittaa Microsoft 365 Business-tilin käyttämisen, valitse Windowsin **Käynnistä**-painike, napsauta hiiren kakkospainikkeella nykyisen tilisi kuvaa ja valitse sitten **Vaihda tiliä**. Kirjaudu sisään käyttämällä organisaatiosi sähköpostiosoitetta ja salasanaa.
  
![Click Info button to view synchronization status](media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a>Windows 10 Business -päivityksen olemassaolon tarkistaminen laitteessa

Varmista, että Azure Active Directoryyn liitettyihin Windows 10 -laitteisiin on päivitetty Windows 10 Business osana Microsoft 365 Business -tilausta.
  
1. Valitse **Asetukset** \> **Järjestelmä** \> **Tietoja**.
    
2. Varmista, että **Julkaisu**-kohdassa lukee **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Seuraavat vaiheet

Mobiililaitteiden määritysohjeet ovat kohdassa [Mobiililaitteiden määrittäminen Microsoft 365 Business -käyttäjille](set-up-mobile-devices.md). Laitteiden ja sovellusten suojauskäytäntöjen määritysohjeet ovat kohdassa [Microsoft 365 Businessin hallinta](manage.md).
  
