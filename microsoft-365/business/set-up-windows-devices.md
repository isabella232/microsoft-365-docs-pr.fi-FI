---
title: Laitteiden Windows käyttäjien Microsoft 365 Business Premium käyttöön
f1.keywords:
- CSH
ms.author: sharik
author: skjerland
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
- okr_smb
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Opi, miten voit Windows Windows 10 Pro käyttäjille Microsoft 365 Business Premium ja ottaa käyttöön keskitetyt hallinta- ja suojaustoiminnot.
ms.openlocfilehash: 3e268d81ff6fb7113b7e0b0fe5d0545ff5c72b1e
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/06/2021
ms.locfileid: "52244772"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Laitteiden Windows käyttäjien Microsoft 365 Business Premium käyttöön

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a>Laitteiden määrittämisen edellytykset Windows käyttäjille Microsoft 365 Business Premium käyttäjille

Ennen kuin voit määrittää Windows -Microsoft 365 Business Premium käyttäjille, varmista, että kaikissa Windows -laitteissa Windows 10 Pro versio 1703 (Creators-päivitys). Windows 10 Pro käyttöönotto edellyttää Windows 10 Business:n käyttöönottoa. Se on joukko pilvipalveluja ja laitteiden hallintaominaisuuksia, jotka täydentävät Windows 10 Pro ja mahdollistavat Microsoft 365 Business Premium:
  
Jos Windows on Windows 7 Pro-, Windows 8 Pro- tai Windows 8.1 Pro-käyttöjärjestelmä, Microsoft 365 Business Premium oikeuttaa sinut Windows 10 päivitykseen.
  
Lisätietoja Windows-laitteiden Windows 10 Pro Creators -päivityksen tekemisestä on tämän aiheen ohjeissa: [Windows Pro Creators -päivityksen tekeminen Windows-laitteisiin](upgrade-to-windows-pro-creators-update.md).
  
Voit [tarkistaa päivityksen toimiminen tai varmistaa,](#verify-the-device-is-connected-to-azure-ad) että laite on yhdistetty Azure AD:iin kohdassa Laitteen Azure AD-yhteyden tarkistaminen.

Katso lyhyt video yhteyden muodostamisesta Windows Microsoft 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](../business-video/index.yml).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Windows 10 -laitteiden liittäminen organisaatiosi Azure AD:hen

Kun Windows kaikki organisaatiosi laitteet on joko päivitetty Windows 10 Pro Creators -päivitykseen tai ne ovat jo Windows 10 Pro Creators -päivitystä, voit liittää nämä laitteet organisaatiosi Azure Active Directory. Kun laitteet on liitetty, ne päivitetään automaattisesti Windows 10 Business, joka on osa Microsoft 365 Business Premium tilaustasi.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Uusi tai päivitetty Windows 10 Pro -laite

Jos laite on uusi laite, jossa on Windows 10 Pro Creators -päivitys, tai laitteeseen on tehty Windows 10 Pro Creators -päivitys, mutta ei vielä Windows 10 -laitemääritystä, noudata seuraavia ohjeita.
  
1. Suorita Windows 10 -laitteen asennus, kunnes näyttöön tulee **Miten haluat määrittää?** -sivu. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Valitse tässä **Määritä organisaatiolle ja** kirjoita sitten organisaation käyttäjänimi ja Microsoft 365 Business Premium. 
    
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
  
   Valitse **Olet valmis!** -sivu, chosse **Valmis**.
  
   ![Valitse Varmista, että tämä on organisaatiosi -näytössä Liity](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Jos olet ladannut tiedostoja OneDrive for Businessiin, synkronoi ne takaisin. Jos käytit kolmannen osapuolen työkalua profiilin ja tiedostojen siirtämiseen, myös ne synkronoidaan uuteen profiiliin.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Laitteen Azure AD -yhteyden tarkistaminen

Voit tarkistaa synkronoinnin tilan valitsemalla **Accessin** työ- tai koulusivulla **Asetukset** **_,** jotta näet painikkeet Tiedot ja Katkaise \<organization name\> **yhteys**  . Saat **synkronoinnin** tilan valitsemalla Tiedot. 
  
Valitse **Synkronoinnin tila** -sivulla **Synkronoi,** jotta saat uusimmat mobiililaitteiden hallintakäytännöt tietokoneeseen.
  
Jos haluat aloittaa Microsoft 365 Business Premium tilin käytön, siirry aloituspainikkeeseen Windows aloituspainike, napsauta nykyisen tilisi kuvaa hiiren kakkospainikkeella ja valitse **Sitten Vaihda tili**.  Kirjaudu sisään käyttämällä organisaatiosi sähköpostiosoitetta ja salasanaa.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a>Varmista, että tietokone on päivitetty Windows 10 Business

Varmista, että Azure AD:Windows 10 liitettyihin laitteisiin on Windows 10 Business osana Microsoft 365 Business Premium tilaustasi.
  
1. Valitse **Asetukset** \> **Järjestelmä** \> **Tietoja**.
    
2. Varmista, että **Julkaisu**-kohdassa lukee **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Seuraavat vaiheet

Jos haluat määrittää mobiililaitteet, katso mobiililaitteiden Microsoft 365 Business Premium [-käyttäjille](set-up-mobile-devices.md). Lisätietoja laitteiden tai sovellusten suojauskäytäntöjen määrittämiskäytännöistä on kohdassa [Microsoft 365 yrityskäyttäjien tietojen hallinta.](manage.md)
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a>Lisätietoja asetusten määrittämisestä ja Microsoft 365 Business Premium

[Microsoft 365 yrityksille -koulutusvideoita](../business-video/index.yml)
