---
title: Toimialueen käyttöön liitettyjen Windows 10 -laitteiden hallinta Microsoft 365 for Businessissa
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Lue, miten voit ottaa Microsoft 365:n käyttöön paikallisten Active Directoryyn liitettyjen Windows 10 -laitteiden suojaamisessa muutamassa vaiheessa.
ms.openlocfilehash: 7bfe5da8701a17712fa249eac99a22b8d5a1b2d1
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471043"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Toimialueen käyttöön liitettyjen Windows 10 -laitteiden hallinta Microsoft 365 Business Premiumilla

Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Business Premiumin suojaamaan Windows 10 -laitteita säilyttäen samalla paikallisen todennuksen edellyttävien paikallisten resurssien käytön.
Voit määrittää tämän suojauksen mukautuksella **Hybrid Azure AD -liitettyjä laitteita**. Nämä laitteet on liitetty sekä paikalliseen Active Directoryyn että Azure Active Directoryyn.

Tässä videossa kuvataan, miten tämä määritetään yleisin skenaario, joka on myös kuvattu vaiheet, joita seurataan.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Hakemistosynkronoinnin valmisteleminen 

Ennen kuin synkronoit käyttäjät ja tietokoneet paikallisesta Active Directory -toimialueesta, tutustu [hakemistosynkronoinnin valmistelemiseen Office 365:ksi](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Erityisesti:

   - Varmista, että hakemistossasi ei ole kaksoiskappaleita seuraaville määritteille: **sähköposti,** **proxyAddresses**ja **userPrincipalName**. Näiden arvojen on oltava yksilöllisiä ja kaksoiskappaleet on poistettava.
   
   - Microsoft suosittelee, että määrität **userPrincipalName** (UPN) -määritteen kullekin paikalliselle käyttäjätilille vastaamaan lisensoitua Microsoft 365 -käyttäjää vastaavaa ensisijaista sähköpostiosoitetta. Esimerkki: *mary.shelley@contoso.com* *mary@contoso.local*
   
   - Jos Active Directory -toimialue päätyy ei-reititettävään liitteeseen , kuten *.local* tai *.lan*, internet-reititettävän liitteen , kuten *.com* tai *.org*, sijaan , säädä paikallisten käyttäjätilien UPN-liite ensin kohdassa [Ei-reititettävän toimialueen valmisteleminen hakemistosynkronointia varten](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)kuvatulla tavalla . 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Asenna ja määritä Azure AD Connect

Jos haluat synkronoida paikallisen Active Directoryn käyttäjät, ryhmät ja yhteystiedot Azure Active Directoryyn, asenna Azure Active Directory Connect ja määritä hakemistosynkronointi. Lisätietoja on [ohjeaiheessa Hakemistosynkronoinnin määrittäminen Office 365:tä varten.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)

> [!NOTE]
> Vaiheet ovat täsmälleen samat Microsoft 365 for Businessille. 

Kun määrität Azure AD Connectin asetukset, suosittelemme, että otat käyttöön **salasanan synkronoinnin,** **saumattoman kertakirjautuksen**ja **salasanan takaisinkirjoitusominaisuuden,** jota myös Microsoft 365 for Business tukee.

> [!NOTE]
> Azure AD Connectin valintaruudun lisäksi salasanan takaisinkirjoituksessa on joitakin lisävaiheita. Lisätietoja on [ohjeaiheessa Toimintaohjeet: salasanan takaisinkirjoituksen määrittäminen](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Määritä Hybridi Azure AD -liittyminen

Ennen kuin otat Windows 10 -laitteiden käyttöön Hybrid Azure AD :n liittämisen, varmista, että täytät seuraavat edellytykset:

   - Käytössäsi on Azure AD Connectin uusin versio.

   - Azure AD Connect on synkronoinut kaikki tietokoneobjektit laitteista, joihin haluat liittyä azure AD:n yhdistelmäksi. Jos tietokoneobjektit kuuluvat tiettyihin organisaatioyksiköihin, varmista, että nämä organisaatioyksiköt on määritetty synkronoitavaksi myös Azure AD -yhteyden yhteydessä.

Jos haluat rekisteröidä aiemmin luodut toimialueeseen liitetyt Windows 10 -laitteet Hybrid Azure AD:n liittämiseksi, noudata [opetusohjelman: Azure Active Directory -yhdistelmän liittämisen ohjeita hallituille toimialueille](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Tämä yhdistelmä mahdollistaa olemassa olevien paikallisten Active Directory -tiedostojen siirtymisen Windows 10 -tietokoneisiin ja tekee niistä pilvivalmiita.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Ota automaattinen rekisteröinti käyttöön Windows 10:ssä

 Lisätietoja Windows 10 -laitteiden automaattisesta rekisteröimiseksi mobiililaitteiden hallintaan Intunen ohjeaiheessa [Windows 10 -laitteen rekisteröiminen automaattisesti ryhmäkäytännön avulla](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Voit määrittää ryhmäkäytännön paikalliselle tietokonetasolle tai joukkotoiminnoille käyttämällä ryhmäkäytäntöjen hallintakonsolia ja ADMX-malleja tämän ryhmäkäytäntöasetuksen luomiseen toimialueen ohjauskoneeseen.

## <a name="5-configure-seamless-single-sign-on"></a>5. Määritä saumaton kertakirjautuminen

  Saumaton sso kirjaa käyttäjät automaattisesti Microsoft 365 -pilviresursseihin, kun he käyttävät yritystietokoneita. Ota käyttöön toinen [Azure Active Directoryn saumattomassa kertakirjautumisessa kuvatuista ryhmäkäytäntövaihtoehdoista: pikakäynnistys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). **Ryhmäkäytäntö-asetus** ei salli käyttäjien muuttaa asetuksiaan, kun taas **Ryhmäkäytäntöasetukset-asetus** määrittää arvot, mutta jättää heidät myös käyttäjän määritettäviksi.

## <a name="6-set-up-windows-hello-for-business"></a>6. Windows Hello for Businessin määrittäminen

 Windows Hello for Business korvaa salasanat vahvalla kaksivaiheisen todennuksen (2FA) kirjautumista paikalliseen tietokoneeseen kirjautumista varten. Yksi tekijä on epäsymmetrinen avainpari, ja toinen on PIN-koodi tai muu paikallinen ele, kuten sormenjälki tai kasvojen tunnistus, jos laitteesi tukee sitä. Suosittelemme, että vaihdat salasanat 2FA:lla ja Windows Hello for Businessilla mahdollisuuksien mukaan.

Jos haluat määrittää Windows Hello for Businessin yhdistelmäkäyttöisen [yhdistelmäavaimen luotettavuuden Windows Hello for Business -edellytykset](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Noudata sitten kohdassa [Windows Hello for Business -näppäinluottamusasetusten määrittäminen annettuja](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings)ohjeita. 
