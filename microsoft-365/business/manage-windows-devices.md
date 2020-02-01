---
title: Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi
f1.keywords:
- NOCSH
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Opi, miten Microsoft 365 voi suojata paikallisen Active Directoryn liittyneen Windows 10-laitteisiin.
ms.openlocfilehash: 170703c7367f9c0e9cb4c10edbd81cb214aa1d3e
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593797"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi

Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Businessin suojaamaan Windows 10-laitteitasi samalla, kun ylläpidämme paikallisen todennuksen edellyttävien paikallisten resurssien käyttö oikeuksia.
Jos haluat määrittää tämän suoja uksen, voit ottaa käyttöön **hybridi Azure AD-liitetyt laitteet**. Nämä laitteet on liitetty sekä paikalliseen Active Directoryyn että Azure Active Directoryyn.

Tässä videossa kerrotaan, miten tämä määritetään tavallisimmille skenaariolle, joka on kuvattu myös seuraavassa kuvatut vaiheet.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Valmistaudu hakemiston synkronointiin 

Ennen kuin synkronoit käyttäjät ja tieto koneet paikallisesta Active Directory-toimi alueesta, tarkista [kansioiden synkronoinnista Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Erityisesti:

   - Varmista, että hakemistossa ei ole kaksoiskappaleita seuraaville määritteille: **Mail**, **Proxyosoitteita**ja **userPrincipalName**. Näiden arvojen on oltava yksilöllisiä, ja mahdolliset kaksoiskappaleet on poistettava.
   
   - Suosittelemme, että määrität kunkin paikallisen käyttäjä tilin **userPrincipalName** (UPN)-määritteen vastaamaan ensisijaista Sähkö posti osoitetta, joka vastaa lisensoitua Microsoft 365-käyttäjää. Esimerkiksi: *Mary.Shelley@contoso.com* sijasta *Mary@contoso. Local*
   
   - Jos Active Directory-toimi alue päättyy ei-reitittävissä olevaan loppu liitteeseen, kuten *. Local* tai *. LAN*, muuta Internet-liitteen, kuten *. com* tai *. org*, sijasta paikallisen käyttäjä tilin UPN-loppu liitettä ensin kuvatulla tavalla, kun [valmistellaan ei-reitittettävä toimi alue kansioiden synkronointia varten](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Azure AD Connectin asentaminen ja määrittäminen

Jos haluat synkronoida käyttäjät, ryhmät ja yhteys tiedot paikallisesta Active Directorysta Azure Active Directoryyn, asenna Azure Active Directory Connect ja määritä hakemiston synkronointi. Lisä tietoja [on kohdassa Määritä hakemiston synkronointi Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) .

> [!NOTE]
> Vaiheet ovat täsmälleen samat Microsoft 365-liike toiminnan osalta. 

Kun määrität Azure AD Connectin vaihto ehtoja, suosittelemme, että otat käyttöön **Sala sanojen synkronoinnin**, **saumattoman kertakirjautumisen**ja **salasanan takaisinkirjoitus** -toiminnon, jota myös tuetaan Microsoft 365 Businessissa.

> [!NOTE]
> Sala sanan takaisinkirjoitus on joitakin lisä vaiheita Azure AD Connectin valinta ruudun ulkopuolella. Lisä tietoja on kohdassa [toiminta ohje: Sala sanan takaisinkirjoitus](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Määritä hybridi Azure AD Join

Ennen kuin otat Windows 10-laitteet käyttöön hybridi-Azure AD-liittymissä, varmista, että seuraavat edellytykset täyttyvät:

   - Käytössäsi on Azure AD Connectin uusin versio.

   - Azure AD Connect on synkronoinut kaikki niiden laitteiden tieto kone objektit, joihin haluat hybridi Azure AD-liittyneen. Jos tieto kone objektit kuuluvat tiettyihin organisaatio yksiköihin (OU), varmista, että ne on määritetty synkronoitaviksi myös Azure AD Connectin avulla.

Jos haluat rekisteröidä aiemmin luotuja toimi alueeseen liitettyä Windows 10-laitetta hybridi-Azure AD-liittymällä, noudata opetus ohjelman ohjeita [: Määritä hybridi Azure Active Directory Join hallittuja toimi alueita varten](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Tämä hybridi-mahdollistaa olemassa olevan paikallisen Active Directoryn liityttyä Windows 10-tieto koneisiin ja tekee niistä pilvi valmiina.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Ota käyttöön automaattinen Ilmoittautuminen Windows 10: lle

 Jos haluat rekisteröidä Windows 10-laitteet automaattisesti mobiililaitteiden hallintaan Intune-laitteella, katso [Windows 10-laitteen automaattinen käyttöönotto ryhmä käytännön avulla](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Voit määrittää ryhmä käytännön paikallisen tieto koneen tasolla tai joukko toimintoja varten käyttämällä ryhmä käytäntöjen hallinta konsolia ja ADMX-malleja, kun haluat luoda tämän ryhmä käytäntö asetuksen toimi alueen ohjaus koneessa.

## <a name="5-configure-seamless-single-sign-on"></a>5. saumattoman kertakirjautumisen määrittäminen

  Saumaton SSO allekirjoittaa käyttäjät automaattisesti Microsoft 365-pilvi resursseissaan, kun he käyttävät yritys tieto koneita. Yksinkertaisesti Ota käyttöön jompikumpi kahdesta Azure Active Directory-palvelussa kuvatusta ryhmä käytäntö vaihtoehdoista [saumaton kertakirjautuminen: Pika-aloitus](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). **Ryhmä käytäntö** -vaihto ehdon avulla käyttäjät eivät voi muuttaa asetuksiaan, kun taas **Ryhmä käytäntö** asetus asettaa arvot, mutta jättää ne myös käyttäjän määritettävissä.

## <a name="6-set-up-windows-hello-for-business"></a>6. Windows Hello for Businessin määrittäminen

 Windows Hello for Business korvaa Sala sanat, joissa on vahva kaksiosainen todennus (2FA) paikalliseen tieto koneeseen kirjautumista varten. Yksi tekijä on epäsymmetrinen avain pari, ja toinen on PIN-koodi tai muu paikallinen ele, kuten sormen jälki tai kasvojen tunnistus, jos laitteesi tukee sitä. Suosittelemme, että vaihdat Sala sanat 2FA-ja Windows Hello-käyttöön mahdollisuuksien mukaan.

Jos haluat määrittää Hybrid Windows Hello for Businessin, tarkista [hybridi avaimen luottamus Windows Hello yrityksille-edellytykset](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Noudata sitten ohjeita kohdassa [Hybrid Windows Hello for Business Key Trust-asetusten määrittäminen](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
