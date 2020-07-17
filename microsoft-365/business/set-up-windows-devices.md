---
title: Windows-laitteiden määrittäminen Microsoft 365 Business Premium -käyttäjille
f1.keywords:
- CSH
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
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Lue, miten voit määrittää Windows 10 Pro for Microsoft 365 Business Premium -käyttäjille -laitteiden määrittämisen keskitetyn hallinnan ja suojauksen valvonnan avulla.
ms.openlocfilehash: 85ac3c964792a132d5699703e543289020e38f57
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785848"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Windows-laitteiden määrittäminen Microsoft 365 Business Premium -käyttäjille

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a>Edellytykset Windows-laitteiden määrittämiselle Microsoft 365 Business Premium -käyttäjille

Ennen kuin voit määrittää Windows-laitteita Microsoft 365 Business Premium -käyttäjille, varmista, että kaikissa Windows-laitteissa on Windows 10 Pron versio 1703 (Creators Update). Windows 10 Pro on edellytys Windows 10 Businessin käyttöönotolle, joka on joukko pilvipalveluita ja laitehallintaominaisuuksia, jotka täydentävät Windows 10 Prota ja mahdollistavat Microsoft 365 Business Premiumin keskitetyt hallinta- ja suojaustoiminnot.
  
Jos käytössäsi on Windows-laitteet, joissa on Windows 7 Pro, Windows 8 Pro tai Windows 8.1 Pro, Microsoft 365 Business Premium -tilauksesi oikeuttaa Windows 10 -päivitykseen.
  
Lisätietoja Windows-laitteiden Windows 10 Pro Creators -päivityksen tekemisestä on tämän aiheen ohjeissa: [Windows Pro Creators -päivityksen tekeminen Windows-laitteisiin](upgrade-to-windows-pro-creators-update.md).
  
Lisätietoja [on ohjeaiheessa Tarkista, että laite on yhdistetty Azure AD:hen,](#verify-the-device-is-connected-to-azure-ad) jotta voit varmistaa, että päivitys on sinulla, tai varmista, että päivitys toimi.

Katso lyhyt video Windowsin yhdistämisestä Microsoft 365:iin.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Windows 10 -laitteiden liittäminen organisaatiosi Azure AD:hen

Kun kaikki organisaatiosi Windows-laitteet on joko päivitetty Windows 10 Pro Creators -päivitykseen tai windows 10 Pro Creators Update on jo käytössä, voit liittyä näihin laitteisiin organisaatiosi Azure Active Directoryyn. Kun laitteet on liitetty, ne päivitetään automaattisesti Windows 10 Businessiin, joka on osa Microsoft 365 Business Premium -tilaustasi.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Uusi tai päivitetty Windows 10 Pro -laite

Jos laite on uusi laite, jossa on Windows 10 Pro Creators -päivitys, tai laitteeseen on tehty Windows 10 Pro Creators -päivitys, mutta ei vielä Windows 10 -laitemääritystä, noudata seuraavia ohjeita.
  
1. Suorita Windows 10 -laitteen asennus, kunnes näyttöön tulee **Miten haluat määrittää?** -sivu. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Valitse tässä **Määritä organisaatiolle** ja kirjoita sitten Microsoft 365 Business Premiumin käyttäjänimi ja salasana. 
    
3. Viimeistele Windows 10 -laitteen määritys.
    
   Kun olet valmis, käyttäjä yhdistetään organisaatiosi Azure AD:hen. Varmista tämä kohdan [Laitteen Azure AD -yhteyden tarkistaminen](#verify-the-device-is-connected-to-azure-ad) ohjeiden mukaan. 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>Laite, joka on jo määritetty ja jossa on Windows 10 Pro

 **Käyttäjien yhdistäminen Azure AD:hen:**
  
1. Valitse käyttäjän Windows-tietokoneessa, jossa on käytössä Windows 10 Pro -versio 1703 (Creators-päivitys) (katso [edellytykset](pre-requisites-for-data-protection.md)), Windows-näppäin ja valitse sitten Asetukset-kuvake.
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. Vallitse **Asetukset** ja valitse sitten **Tilit**.
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. Valitse **Omat tiedot** -sivulla **Käytä työpaikan tai koulun resursseja** \> **Yhdistä**.
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. Valitse **Määritä työpaikan tai oppilaitoksen tili** -valintaikkunan **Vaihtoehtoiset toimet** -kohdassa **Liitä tämä laite Azure Active Directoryyn**.
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. Kirjoita **Kirjaudu sisään** -sivulla työpaikan tai oppilaitoksen tili \> **Seuraava**.
  
   Kirjoita salasana **Anna salasana** -sivulla \> **Kirjaudu**.
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. Varmista **Varmista, että tämä on organisaatiosi** -sivulla, että tiedot ovat oikein, ja valitse **Liity**.
  
   Valitse **Olet valmis!** -sivulla **Valmis**.
  
   ![On the Make sure this is your organization screen, click Join](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Jos olet ladannut tiedostoja OneDrive for Businessiin, synkronoi ne takaisin. Jos käytit kolmannen osapuolen työkalua profiilin ja tiedostojen siirtämiseen, synkronoi ne myös uuteen profiiliin.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Laitteen Azure AD -yhteyden tarkistaminen

Voit tarkistaa synkronoinnin tilan valitsemalla **Asetukset-ikkunan** **Access-työpaikan tai oppilaitoksen** -sivulla **Yhdistetty** _ \<organization name\> _ -painikkeet, jos haluat näyttää **tiedot** ja **Katkaise yhteys**-painikkeet. Tuo synkronointitilasi näkyviin valitsemalla **Tiedot**. 
  
Valitse Synkronointitila-sivulla Synkronoi, jolloin saat uusimmat mobiililaitteiden hallintakäytännöt PC-tietokoneeseen.
  
Voit aloittaa Microsoft 365 Business Premium -tilin **Start** käyttämisen siirtymällä Windowsin Käynnistä-painikkeeseen, napsauttamalla nykyistä tilikuvaasi hiiren kakkospainikkeella ja **vaihtamalla tiliä**. Kirjaudu sisään käyttämällä organisaatiosi sähköpostiosoitetta ja salasanaa.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a>Windows 10 Business -päivityksen olemassaolon tarkistaminen laitteessa

Varmista, että Azure AD liittyi Windows 10 -laitteisiin, on päivitetty Windows 10 Businessiksi osana Microsoft 365 Business Premium -tilaustasi.
  
1. Valitse **Asetukset** \> **Järjestelmä** \> **Tietoja**.
    
2. Varmista, että **Julkaisu**-kohdassa lukee **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Seuraavat vaiheet

Lisätietoja mobiililaitteiden määrittämisestä on ohjeaiheessa [Mobiililaitteiden määrittäminen Microsoft 365 Business Premium -käyttäjille](set-up-mobile-devices.md), Laitteen suojauksen tai sovellusten suojauskäytäntöjen määrittäminen on [ohjeaiheessa Microsoft 365 for Businessin hallinta](manage.md).
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a>Lisätietoja Microsoft 365 Business Premiumin määrittämisestä ja käyttämisestä

[Microsoft 365 yritysten koulutus videoita](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
