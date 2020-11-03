---
title: Windows-laitteiden määrittäminen Microsoft 365 Business Premium-käyttäjille
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
description: Lue, miten voit määrittää Windows 10 Pro-käyttö järjestelmän Microsoft 365 Business Premium-käyttäjille ja ottaa käyttöön keskitetyn hallinnan ja tieto turvan hallinta toiminnot.
ms.openlocfilehash: c95b9e51c7ec3c440509fe34084d2a030c7f2eec
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841255"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Windows-laitteiden määrittäminen Microsoft 365 Business Premium-käyttäjille

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a>Microsoft 365 Business Premium-käyttäjien Windows-laitteiden määrittämisen edellytykset

Ennen kuin voit määrittää Windows-laitteita Microsoft 365 Business Premium-käyttäjille, varmista, että kaikissa Windows-laitteissa on käytössä Windows 10 Pro, versio 1703 (Creators Update). Windows 10 Pro on Windows 10 Businessin käyttöönoton edellytys, joka on pilvi palveluiden ja laite hallinnan ominaisuuksien joukko, joka täydentää Windows 10 Prota ja mahdollistaa Microsoft 365 Business Premiumin keskitetyn hallinnan ja tieto turvan.
  
Jos käytössäsi on Windows-laite, jossa on Windows 7 Pro, Windows 8 Pro tai Windows 8,1 Pro, Microsoft 365 Business Premium-tilauksesi oikeuttaa sinut Windows 10-päivitykseen.
  
Lisätietoja Windows-laitteiden Windows 10 Pro Creators -päivityksen tekemisestä on tämän aiheen ohjeissa: [Windows Pro Creators -päivityksen tekeminen Windows-laitteisiin](upgrade-to-windows-pro-creators-update.md).
  
Lisä tietoja on kohdassa [Varmista, että laite on yhdistetty Azure](#verify-the-device-is-connected-to-azure-ad) AD:hen, ja tarkista, että päivitys on tehty, tai varmista, että päivitys on toiminut.

Katso lyhyt video, jossa on tietoja Windowsin liittämisestä Microsoft 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Windows 10 -laitteiden liittäminen organisaatiosi Azure AD:hen

Kun kaikki organisaatiosi Windows-laitteet on päivitetty Windows 10 Pro Creators-päivitykseen tai Windows 10 Pro Creators-päivitys on jo asennettu, voit liittää nämä laitteet organisaatiosi Azure Active Directoryyn. Kun laitteet on liitetty, ne päivitetään automaattisesti Windows 10 Business-versioon, joka kuuluu Microsoft 365 Business Premium-tilaukseesi.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Uusi tai päivitetty Windows 10 Pro -laite

Jos laite on uusi laite, jossa on Windows 10 Pro Creators -päivitys, tai laitteeseen on tehty Windows 10 Pro Creators -päivitys, mutta ei vielä Windows 10 -laitemääritystä, noudata seuraavia ohjeita.
  
1. Suorita Windows 10 -laitteen asennus, kunnes näyttöön tulee **Miten haluat määrittää?** -sivu. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Valitse tässä **kohdassa Määritä organisaatiolle** ja anna sitten Microsoft 365 Business Premiumin käyttäjä nimi ja sala sana. 
    
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
  
6. Varmista, että **Tämä on organisaatiosi** -sivulla Tarkista, että tiedot ovat oikein, ja valitse **Liity**.
  
   Valitse **Olet valmis!** sivu, valitse jokin kolmesta **Done**.
  
   ![Valitse Varmista, että tämä on organisaatiosi-näytössä liity](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Jos olet ladannut tiedostoja OneDrive for Businessiin, synkronoi ne takaisin. Jos käytit kolmannen osapuolen työkalua profiilin ja tiedostojen siirtämiseen, synkronoi ne myös uuteen profiiliin.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Laitteen Azure AD -yhteyden tarkistaminen

Jos haluat tarkistaa synkronoinnin tilan, valitse **Asetukset** -kohdan **Käytä työpaikan tai oppi laitoksen** sivulla **yhdistetty** _ _- \<organization name\> alue, jos haluat näyttää painikkeiden **tiedot** ja **katkaista yhteyden**. Saat synkronoinnin tilan valitsemalla **tiedot** . 
  
Valitse **synkronoinnin tila** -sivulla **Synkronoi** , jotta saat uusimmat mobiililaitteiden hallinta käytännöt tieto koneeseen.
  
Voit aloittaa Microsoft 365 Business Premium-tilin käytön siirtymällä Windowsin **Käynnistä** -painikkeeseen, napsauttamalla nykyistä tili kuvaasi hiiren kakkos painikkeella ja **vaihtamalla sitten tilin**. Kirjaudu sisään käyttämällä organisaatiosi sähköpostiosoitetta ja salasanaa.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a>Varmista, että tieto kone on päivitetty Windows 10 Business-versioon

Varmista, että Azure AD on liittynyt Windows 10-laitteisiin Windows 10 Business-versioon osana Microsoft 365 Business Premium-tilausta.
  
1. Valitse **Asetukset** \> **Järjestelmä** \> **Tietoja**.
    
2. Varmista, että **Julkaisu** -kohdassa lukee **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Seuraavat vaiheet

Lisä tietoja mobiililaitteiden määrittämisestä on kohdassa [mobiililaitteiden määrittäminen microsoft 365 Business Premium-käyttäjille](set-up-mobile-devices.md), laitteen suojaus asetusten ja sovellusten suojaus käytäntöjen määrittäminen on kohdassa [Microsoft 365 for Businessin hallinta](manage.md).
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a>Lisä tietoja Microsoft 365 Business Premiumin määrittämisestä ja käyttämisestä

[Microsoft 365 for Business-koulutus videot](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
