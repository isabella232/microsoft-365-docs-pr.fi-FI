---
title: Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi
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
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Lue lisä tietoja siitä, miten Microsoft 365 voi suojata paikallisia mainoksia, jotka on liitetty Windows 10-laitteisiin.
ms.openlocfilehash: 9bfd540c0ff113762485f62707f1975ff53accc4
ms.sourcegitcommit: 1162d676b036449ea4220de8a6642165190e3398
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068101"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi

Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Businessin suojaamaan Windows 10-laitteitasi samalla, kun ylläpidämme paikallisen todennuksen edellyttävien paikallisten resurssien käyttö oikeuksia. Voit määrittää tämän ensin synkronoimalla Active Directory-hakemisto palvelun Azure Active Directoryn kanssa, jonka jälkeen rekisteröit Windows 10-laitteet Azure AD:N avulla ja rekisteröimällä ne mobiililaitteiden hallintaan Microsoft 365 Businessilla.
Seuraavassa videossa kerrotaan, miten tämä määritetään tavallisimmille skenaariolle.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Toimi alueeseen liitettyjen laitteiden määrittäminen Microsoft 365 Businessin hallitsemista varten

Jos haluat määrittää organisaatiosi toimi alueeseen liitetyt laitteet hyödyntämään Azure Active Directoryn tarjoamia ominaisuuksia paikallisen Active Directoryn lisäksi, voit ottaa käyttöön **hybridi Azure AD-liitetyt laitteet**. Nämä ovat laitteita, jotka on liitetty paikalliseen Active Directoryyn ja Azure Active Directoryyn. Hybridi-Azure AD liitetyt laitteet voidaan suojata ja hallita Microsoft 365 Business. 
  
Suorita seuraavat vaiheet, jotta Windows 10-laitteesi hybridi-Azure AD yhdistetään ja sitä hallinnoi Microsoft 365 Business.
  
1. **Valmisteleminen hakemiston synkronointia varten**: ennen kuin synkronoit käyttäjät ja tieto koneet paikallisesta Active Directory-toimi alueesta, tarkista [kansioiden synkronoinnista Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Erityisesti:

   - Varmista, että hakemistossa ei ole kaksoiskappaleita seuraaville määritteille: **Mail**, **proxyosoitteita**ja **userPrincipalName**. Näiden arvojen on oltava yksilöllisiä ja kaksoiskappaleet poistettava..
   
   - Suosittelemme, että kunkin paikallisen käyttäjä tilin **userPrincipalName** (UPN)-määrite on määritetty vastaamaan ensisijaista Sähkö posti osoitetta, joka vastaa lisensoitua Microsoft 365-käyttäjää. Esimerkiksi **Mary.Shelley@contoso.com** eikä **Mary @ contoso. Local**
   
   - Jos Active Directory-toimi alue päättyy ei-reitittävissä olevan liitteen, kuten **. Local** tai **. LAN**, sijasta, sinun on ensin MUUTETTAVA paikallisten käyttäjä tilien UPN-loppu liitettä, kuten. **com** tai **. org**, sen sijaan, että olet kuvattu [Valmistele ei-reitittävissä oleva toimi alue kansioiden synkronointia varten](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

2. **Asenna ja määritä Azure AD Connect**: Synkronoi käyttäjät, ryhmät ja yhteys tiedot paikallisesta Active Directorysta Azure Active Directoryyn suorittamalla ohjattu hakemiston synkronointi Azure Active Directory Connectin avulla. Lisä tietoja [on kohdassa Määritä hakemiston synkronointi Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) .
    
    > [!NOTE]
    > Vaiheet ovat täsmälleen samat Microsoft 365-liike toiminnan osalta. 
    
Kun määrität Azure AD Connect-vaihto ehtoja, suosittelemme, että otat käyttöön **Sala sanojen synkronoinnin** ja **saumattoman kertakirjautumisen**sekä **Sala sanan takaisinkirjoitus** -ominaisuuden, jota tuetaan myös Microsoft 365 Businessissa.

> [!NOTE]
> Sala sanan takaisinkirjoitus on joitakin lisä vaiheita Azure AD Connectin valinta ruudun ulkopuolella. Katso [ohjeet: Määritä Sala sanan takaisinkirjoitus](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 
     
3. **Määritä hybridi-Azure AD Join**: ennen kuin otat Windows 10-laitteet käyttöön hybridi Azure AD liittynyt, varmista, että olet täyttää seuraavat edellytykset:

   - Käytössäsi on Azure AD Connectin uusin versio.

   - Azure AD Connect on synkronoinut kaikki niiden laitteiden tieto kone objektit, joihin haluat hybridi Azure AD-liittyneen. Jos tieto kone objektit kuuluvat tiettyihin organisaatio yksiköihin (OU), varmista, että ne on määritetty synkronoitaviksi myös Azure AD Connectin avulla.

Jos haluat rekisteröidä aiemmin luotuja toimi alueeseen liitettyä Windows 10-laitetta hybridi-Azure AD-liittymällä, noudata opetus ohjelman ohjeita [: Määritä hybridi Azure Active Directory Join hallittuja toimi alueita varten](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Tämä tekee hybridi-mahdollistaa olemassa olevan paikallisen Active Directory liittynyt Windows 10-tieto koneisiin ja tehdä niistä pilvi valmiina.
    
4. **Ota automaattinen rekisteröinti käyttöön Windows 10**: Jos haluat rekisteröidä Windows 10-laitteet mobiililaitteiden hallintaan Intune-laitteella, katso [Windows 10-laitteen rekisteröiminen automaattisesti ryhmä käytännön avulla](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Voit määrittää ryhmä käytännön paikallisen tieto koneen tasolla tai joukko toimintoja varten luomalla ryhmä käytäntö asetuksen toimi alueen ohjaus koneeseen ryhmä käytäntöjen hallinta konsolin ja ADMX-mallien avulla.

5. **Konfiguroi saumaton kertakirjautuminen**: saumaton SSO allekirjoittaa käyttäjät automaattisesti Microsoft 365-pilvi resursseissaan, kun he käyttävät yritys tieto koneita. Yksinkertaisesti Ota käyttöön jompikumpi kahdesta Azure Active Directory-palvelussa kuvatusta ryhmä käytäntö vaihtoehdoista [saumaton kertakirjautuminen: Pika-aloitus](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). **Ryhmä käytäntö** asetus ei salli käyttäjien muuttaa asetuksia, kun taas **Ryhmä käytäntö** asetus asettaa arvot, mutta jättää ne myös käyttäjän määritettävissä.

6. **Windows Hello for Businessin määrittäminen**: Windows Hello for Business korvaa Sala sanat, joissa on vahva kaksiosainen todennus (2FA) paikalliseen tieto koneeseen kirjautumista varten. Yksi tekijä on epäsymmetrinen avain pari, ja toinen on PIN-koodi tai muu paikallinen ele, kuten sormen jälki tai kasvojen tunnistus, jos laitteesi tukee sitä. Suosittelemme, että vaihdat Sala sanat 2FA:N ja Windows Hello for Businessin kanssa mahdollisuuksien mukaan.

Jos haluat määrittää Hybrid Windows Hello for Businessin, tarkista [hybridi avaimen luottamus Windows Hello yrityksille-edellytykset](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). [Määritä sitten Business Key trustin asetukset noudattamalla ohjeita hybridi-Windows Hello-asetusten määrittämiseen](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
