---
title: Paikallisten resurssien käyttö Azure AD-liitetystä laitteesta Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Opi, miten voit käyttää paikallisia resursseja, kuten yritys sovelluksia, tiedosto resursseja ja tulostimia Azure Active Directorysta, liittyi Windows 10-laitteeseen.
ms.openlocfilehash: 653b53d29e84bbdc91273cb78b9b8407c0f6a209
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593229"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Paikallisten resurssien käyttö Azure AD-liitetystä laitteesta Microsoft 365 Business

Kaikissa Windows 10-laitteilla, joihin on liitetty Azure Active Directory, on pääsy kaikkiin pilvipohjaisiin resursseihin, kuten Office 365-sovelluksiin, ja ne voidaan suojata Microsoft 365 Businessin avulla. Voit myös sallia paikallisten resurssien, kuten Business Line (LOB)-sovellusten, jaettujen tiedostojen ja tulostimien, käytön. Jos haluat sallia Accessin, synkronoi paikallinen Active Directory Azure Active Directoryn kanssa [Azure AD Connectin](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) avulla. 

Lisä tietoja on kohdassa [laitteen hallinnan esittely Azure Active Directoryssa](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
Vaiheet on myös tiivistetty seuraavissa osissa.

> [!IMPORTANT]
> Tämä toimenpide koskee vain OAuth-ja NTLM-ohjeita. Kerberos-tukea ei tueta.
 
## <a name="run-azure-ad-connect"></a>Suorita Azure AD Connect

Suorita seuraavat vaiheet, jotta organisaatiosi Azure AD-liitetyt laitteet voivat käyttää paikallisia resursseja.
  
1. Jos haluat synkronoida käyttäjät, ryhmät ja yhteys tiedot paikallisesta Active Directorysta Azure Active Directoryyn, suorita ohjattu hakemiston synkronointi ja Azure AD Connect kohdassa [Office 365 Directory-synkronoinnin määrittäminen](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)kuvatulla tavalla.
    
2. Kun hakemiston synkronointi on valmis, varmista, että organisaatiosi Windows 10-laitteet on liitetty Azure AD-palveluun. Tämä vaihe tehdään erikseen kussakin Windows 10-laitteessa. Lisä tietoja on kohdassa [Windows-laitteiden määrittäminen Microsoft 365-yritys käyttäjille](set-up-windows-devices.md) . 
    
3. Kun Windows 10-laitteet ovat liittyneet Azure AD, jokaisen käyttäjän on käynnistettävä laitteensa uudelleen ja kirjauduttava sisään Microsoft 365-yrityksen tunniste tiedoilla. Kaikki laitteet voivat nyt käyttää myös paikallisia resursseja.
    
Azure AD-liitettyjen laitteiden paikallisten resurssien käyttö oikeuksia ei tarvita lisä toimia. Tämä toiminnallisuus on rakennettu Windows 10. 

Jos sinulla on suunnitelmia kirja utua AADJ-laitteeseen kuin salasana menetelmään, kuten PIN/Bio-metric WHFB-tunniste tietojen sisäänkirjautumisen kautta, ja käyttää sitten yrityksen tiloissa käytettäviä resursseja (osakkeita, tulostimia.. jne), noudatahttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Jos organisaatiosi ei ole valmis ottamaan käyttöön yllä kuvattua Azure AD-laitteen kokoonpanoa, harkitse [hybridi Azure AD-laitteen kokoonpanon](manage-windows-devices.md)määrittämistä.
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Huomioitavaa, kun liityt Windows-laitteisiin Azure ADIIN

Jos Azure-AD-liittyneen Windows-laite on aiemmin liittynyt toimi alueeseen tai työryhmään, harkitse seuraavia rajoituksia:
  
- Kun laite Azure AD liittyy, se luo uuden käyttäjän viittaamatta olemassa olevaan profiiliin. Profiilit on siirrettävä manuaalisesti. Käyttäjä profiili sisältää tietoja, kuten Suosikit, paikalliset tiedostot, selaimen asetukset ja Käynnistä-valikon asetukset. Paras tapa on löytää kolmannen osapuolen työkalu, jolla voit yhdistää olemassa olevat tiedostot ja asetukset uuteen profiiliin.

- Jos laite käyttää ryhmä käytäntö objekteja, joissakin GPOs-sovelluksessa ei ehkä ole vastaavaa [määritys palvelun toimittajaa](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) Intune-kohteessa. Suorita [mmat-työkalu](https://www.microsoft.com/download/details.aspx?id=45520) löytääksesi vertailukelpoisia csps-virheitä olemassa oleville ryhmä käytäntö objekteja varten.

- Käyttäjät eivät voi todentaa Active Directory-todennuksesta riippuvaisia sovelluksia. Arvioi vanha sovellus ja harkitse päivittämistä sovellukseen, joka käyttää modernia auth-sovellusta, jos mahdollista.

- Active Directory-tulostimien etsiminen ei toimi. Voit tarjota suoria tulostin polkuja kaikille käyttäjille tai käyttää [Hybrid Cloud Print-palvelun](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)käyttöä.
