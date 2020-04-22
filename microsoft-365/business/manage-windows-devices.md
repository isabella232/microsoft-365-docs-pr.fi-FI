---
title: Microsoft 365 for Businessin hallitseman toimialueeseen liitettyjen Windows 10 -laitteiden hallinnan ottaminen käyttöön
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
description: Lue, miten voit antaa Microsoft 365:n suojata paikallisia Active-Directoryyn liitettyjä Windows 10 -laitteita muutamassa vaiheessa.
ms.openlocfilehash: 431c1be74723e156befb13ffe1ed98b48b9a23cb
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43633279"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-for-business"></a>Microsoft 365 for Businessin hallitseman toimialueeseen liitettyjen Windows 10 -laitteiden hallinnan ottaminen käyttöön

Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 for Businessin suojaamaan Windows 10 -laitteita ja säilyttämään silti paikallisen todennuksen edellyttävien paikallisten resurssien käytön.
Voit määrittää tämän suojauksen käyttöön **hybridiazure AD-liitetyillä laitteilla.** Nämä laitteet on liitetty sekä paikalliseen Active Directoryyn että Azure Active Directoryyn.

Tässä videossa kuvataan, miten tämä määritetään yleisimpää skenaariota varten, joka on kuvattu myös seuraavissa vaiheissa.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Valmistele hakemistosynkronointiin 

Ennen kuin synkronoit käyttäjät ja tietokoneet paikallisesta Active Directory -toimialueesta, tutustu artikkeliin [Hakemistosynkronoinnin valmisteleminen Office 365:een](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Erityisesti:

   - Varmista, että hakemistossa ei ole kaksoiskappaleita seuraaville määritteille: **mail**, **proxyAddresses**ja **userPrincipalName**. Näiden arvojen on oltava yksilöllisiä, ja kaksoiskappaleet on poistettava.
   
   - Suosittelemme, että määrität kullekin paikalliselle käyttäjätilille **upn (userPrincipalName)** -määritteen vastaamaan ensisijaista sähköpostiosoitetta, joka vastaa lisensoitua Microsoft 365 -käyttäjää. Esimerkki: *mary.shelley@contoso.com* mary@contoso *sijaan.local*
   
   - Jos Active Directory -toimialue päättyy ei-reititettävään jälkiliitteeseen, kuten *.local* tai *.lan*, voit muuttaa internetin reititettävän liitteen, kuten *.com* tai *.org*, sijaan paikallisten käyttäjätilien UPN-liitettä ensin kohdassa [Ei-reititettävän toimialueen valmisteleminen hakemistosynkronointia varten](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Azure AD Connectin asentaminen ja määrittäminen

Jos haluat synkronoida käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directoryyn, asenna Azure Active Directory Connect ja määritä hakemistosynkronointi. Lisätietoja on [ohjeaiheessa Hakemistosynkronoinnin määrittäminen Office 365:tä varten.](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)

> [!NOTE]
> Vaiheet ovat täsmälleen samat Microsoft 365 for Businessille. 

Kun määrität Azure AD Connect -asetuksia, suosittelemme, että otat käyttöön **salasanan synkronoinnin,** **saumattoman kertakirjautumisen**ja **salasanan takaisinkirjoitusominaisuuden,** jota tuetaan myös Microsoft 365 for Businessissa.

> [!NOTE]
> Azure AD Connectin valintaruudun lisäksi salasanan takaisinkirjoitukselle on joitakin lisävaiheita. Lisätietoja on [ohjeaiheessa Toimintaohjeet: salasanan takaisinkirjoituksen määrittäminen](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Määritä Hybrid Azure AD Join

Ennen kuin otat Windows 10 -laitteiden käyttöön Hybrid Azure AD-versioon liittyen, varmista, että täytät seuraavat edellytykset:

   - Käytössäsi on Azure AD Connectin uusin versio.

   - Azure AD connect on synkronoinut kaikki sellaisten laitteiden tietokoneobjektit, jotka haluat yhdistää Azure AD:hen. Jos tietokoneobjektit kuuluvat tiettyihin organisaatioyksiköihin, varmista, että nämä organisaatioyksiköt on määritetty synkronoitavia varten myös Azure AD connect -yhteyden yhteydessä.

Jos haluat rekisteröidä olemassa olevat toimialueeseen liitetyt Windows 10 -laitteet Hybrid Azure AD -palveluksi, noudata [opetusohjelman Azure Active Directory -hybridiliitoksen määrittäminen hallituille toimialueille](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join)ohjeita. Tämä yhdistelmämahdollistaa nykyisen paikallisen Active Directoryn liitettyjen Windows 10 -tietokoneiden kanssa ja pilvipalvelun valmiiksi.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Ota automaattinen rekisteröinti Käyttöön Windows 10:ssä

 Jos haluat rekisteröidä Windows 10 -laitteet automaattisesti mobiililaitteiden hallintaa varten Intunen käyttöön, katso Windows [10 -laitteen rekisteröiminen automaattisesti ryhmäkäytännön avulla](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Voit määrittää ryhmäkäytännön paikalliselle tietokonetasolle tai joukkotoiminnoille käyttämällä ryhmäkäytäntöjen hallintakonsolia ja ADMX-malleja tämän ryhmäkäytäntöasetuksen luomiseen toimialueen ohjauskoneeseen.

## <a name="5-configure-seamless-single-sign-on"></a>5. Määritä saumaton kertakirjautuminen

  Saumaton SSO kirjaa käyttäjät automaattisesti Microsoft 365 -pilviresursseihinsa, kun he käyttävät yritystietokoneita. Ota käyttöön jompaakumpaa [azure Active Directoryn saumaton tavasta Single Sign-On: Quick start -kohdassa](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature)kuvatuista kahdesta ryhmäkäytäntövaihtoehdosta. **Ryhmäkäytäntö-asetus** ei salli käyttäjien muuttaa asetuksiaan, kun taas **Ryhmäkäytäntöasetukset-asetus** määrittää arvot, mutta jättää heidät myös käyttäjän määritettäviksi.

## <a name="6-set-up-windows-hello-for-business"></a>6. Windows Hello for Businessin määrittäminen

 Windows Hello for Business korvaa salasanat vahvalla kaksivaiheisella todennuksella (2FA) paikalliseen tietokoneeseen kirjautumista varten. Yksi tekijä on epäsymmetrinen avainpari ja toinen PIN-koodi tai muu paikallinen ele, kuten sormenjälki tai kasvojentunnistus, jos laite tukee sitä. Suosittelemme, että korvaat salasanat 2FA: lla ja Windows Hello for Businessilla, jos mahdollista.

Voit määrittää Windows Hello for Businessin yhdistelmätoiminnon [tutustuessa hybridiavaimeen, joka luottaa Windows Hello for Business -edellytyksiin](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Noudata sitten ohjeaiheen [Systematistisen Windows Hello for Business -näppäinluottamusasetusten määrittäminen](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings)ohjeita. 
