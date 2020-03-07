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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Lue, miten voit ottaa Microsoft 365:n suojaamaan paikallisia Active-Directory-liitettyjä Windows 10 -laitteita muutamassa vaiheessa.
ms.openlocfilehash: 625eb7ac344b060409101d650ff30044d073f5bf
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561456"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi

Jos organisaatiosi käyttää paikallista Windows Server In Active Directorya, voit määrittää Microsoft 365 Businessin suojaamaan Windows 10 -laitteita säilyttäen samalla paikallisen todennuksen edellyttävien paikallisten resurssien käytön.
Voit määrittää tämän suojauksen ottaaksesi käyttöön **Hybrid Azure AD :n liitetyt laitteet**. Nämä laitteet on liitetty sekä paikalliseen Active Directoryyn että Azure Active Directoryyn.

Tässä videossa kuvataan, miten tämä määritetään yleisimmissä tilanteissa, jotka on kuvattu myös seuraavissa vaiheissa.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Valmistaudu hakemistosynkronointiin 

Ennen kuin synkronoit käyttäjät ja tietokoneet paikallisesta Active Directory -toimialueesta, tutustu [artikkeliin Hakemistosynkronoinnin valmisteleminen Office 365:een](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Erityisesti:

   - Varmista, että hakemistossa ei ole kaksoiskappaleita seuraaville määritteille: **mail**, **proxyAddresses**ja **userPrincipalName**. Näiden arvojen on oltava yksilöllisiä ja kaksoiskappaleet poistettava.
   
   - Microsoft suosittelee, että määrität **userPrincipalName** (UPN) -määritteen kullekin paikalliselle käyttäjätilille vastaamaan ensisijaista sähköpostiosoitetta, joka vastaa lisensoitua Microsoft 365 -käyttäjää. Esimerkiksi: *mary.shelley@contoso.com* *mary@contoso.local*
   
   - Jos Active Directory -toimialue päättyy ei-reititettävään liitteeseen, kuten *.local* tai *.lan*, ** säädä ensin -toimialueen ** [valmisteleminen hakemistosynkronointia varten"](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)-kohdassa kuvattuun upn-päätettä . 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Azure AD Connectin asentaminen ja määrittäminen

Jos haluat synkronoida käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directoryyn, asenna Azure Active Directory Connect ja määritä hakemistosynkronointi. Lisätietoja [on ohjeaiheessa Hakemistosynkronoinnin määrittäminen Office 365:tä varten.](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)

> [!NOTE]
> Vaiheet ovat täsmälleen samat Microsoft 365 Businessissa. 

Kun määrität Azure AD Connectin asetukset, suosittelemme, että otat **käyttöön salasanan synkronoinnin,** **saumattoman kertakirjautumisen**ja **salasanan palautustoiminnon,** jota tuetaan myös Microsoft 365 Businessissa.

> [!NOTE]
> Azure AD Connectin valintaruudun lisäksi on joitakin lisävaiheita salasanan takaisinkirjoittamiseksi. Lisätietoja on [ohjeaiheessa Toimintaohjeet: salasanan takaisinkirjoituksen määrittäminen](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Määritä Hybridi Azure AD -liity

Ennen kuin otat Windows 10 -laitteiden käyttöön, että Ne liitetään Hybridi Azure AD:hen, varmista, että täytät seuraavat edellytykset:

   - Käytössäsi on Azure AD Connectin uusin versio.

   - Azure AD connect on synkronoinut kaikki sellaisten laitteiden tietokoneobjektit, joihin haluat liittyä Azure AD:n yhdistelmäksi. Jos tietokoneobjektit kuuluvat tiettyihin organisaatioyksiköihin, varmista, että nämä oUs:t on määritetty synkronoitavia varten myös Azure AD connectissa.

Jos haluat rekisteröidä aiemmin luodut toimialueuuteen liitetyt Windows 10 -laitteet Hybrid Azure AD -palveluun liittyneenä, noudata [opetusohjelman ohjeita: Määritä azure Active Directory -yhdistelmäliittymä hallituille toimialueille](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Tämä hybridi mahdollistaa nykyisen paikallisen Active Directoryn windows 10 -tietokoneisiin ja tekee niistä pilvivalmiita.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Ota automaattinen rekisteröinti käyttöön Windows 10:ssä

 Lisätietoja Windows 10 -laitteiden automaattisesta rekisteröimiseksi mobiililaitteiden hallintaa varten Intuniin on ohjeaiheessa [Windows 10 -laitteen rekisteröiminen automaattisesti ryhmäkäytännön avulla](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Voit määrittää ryhmäkäytäntökäytännön paikalliselle tietokonetasolle tai joukkotoiminnoille, voit luoda tämän ryhmäkäytäntöasetuksen toimialueen ohjauskoneeseen ryhmäkäytäntöjen hallintakonsolin ja ADMX-mallien avulla.

## <a name="5-configure-seamless-single-sign-on"></a>5. Määritä saumaton kertakirjautuminen

  Saumaton sso kirjaa käyttäjät automaattisesti Microsoft 365 -pilviresursseihinsa, kun he käyttävät yritystietokoneita. Ota käyttöön toinen [Azure Active Directoryseamless Single Sign-On: Quick start -kohdassa](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature)kuvatuista ryhmäkäytäntövaihtoehdoista. **Ryhmäkäytäntö-asetus** ei salli käyttäjien muuttaa asetuksiaan, kun taas **Ryhmäkäytäntöasetukset-asetus** määrittää arvot, mutta jättää ne myös käyttäjän määritettäviksi.

## <a name="6-set-up-windows-hello-for-business"></a>6. Windows Hello for Businessin määrittäminen

 Windows Hello for Business korvaa salasanat vahvalla kaksiosaisella todennuksella (2FA), joka liittyy paikalliseen tietokoneeseen kirjautumiseen. Yksi tekijä on epäsymmetrinen avainpari ja toinen PIN-koodi tai muu paikallinen ele, kuten sormenjälki tai kasvojentunnistus, jos laitteesi tukee sitä. Suosittelemme, että korvaat salasanat 2FA:lla ja Windows Hello for Businessilla mahdollisuuksien mukaan.

Jos haluat määrittää Hybridi-Windows Hello for Businessin asetukset, tutustu [Hybridiavaimen luottamus Windows Hello for Business -edellytyksiin](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Noudata sitten kohdassa [Windows Hello for Business -avainluottamusasetusten määrittäminen](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings)ohjeita. 
