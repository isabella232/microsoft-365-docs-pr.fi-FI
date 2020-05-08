---
title: Paikallisten resurssien käyttäminen Azure AD:hen liitetystä laitteesta Microsoft 365 Businessissa
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
description: Lue, miten voit käyttää paikallisia resursseja, kuten liiketoimintasovelluksia, jaettuja tiedostoresursseja ja tulostimia Azure Active Directorysta, joka on liitetty Windows 10 -laitteeseen.
ms.openlocfilehash: 980efbf09349cc0203ac50ae5e028c008d5694ca
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165897"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Paikallisten resurssien käyttäminen Azure AD:hen liitetystä laitteesta Microsoft 365 Business Premiumissa

Kaikilla Windows 10 -laitteilla, joihin on liitetty Azure Active Directory, on pääsy kaikkiin pilvipohjaisiin resursseihin, kuten Microsoft 365 -sovelluksiin, ja ne voidaan suojata Microsoft 365 Business Premiumilla. Voit myös sallia paikallisten resurssien, kuten LOB (Line of Business) -sovellusten, jaettujen tiedostojen ja tulostimien, käytön. Jos haluat sallia käytön, synkronoi paikallinen Active Directory Azure Active Directoryazure Active Directoryn kanssa [Azure AD Connectin](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) avulla. 

Lisätietoja on [ohjeaiheessa Johdanto laitehallintaan Azure Active Directoryssa](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
Vaiheet on myös tiivistetty seuraaviin osiin.

> [!IMPORTANT]
> Tämä menettely koskee vain OAuth- ja NTLM-lukuja. Kerberos ei ole tuettu.
 
## <a name="run-azure-ad-connect"></a>Azure AD Connectin suorittaminen

Noudata seuraavia ohjeita, jotta organisaation Azure AD -liitetyt laitteet voivat käyttää paikallisia resursseja.
  
1. Jos haluat synkronoida käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directoryyn, suorita ohjattu hakemistosynkronointitoiminto ja Azure AD Connect kohdassa [Hakemistosynkronoinnin määrittäminen Office 365:tä varten](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)kuvatulla tavalla.
    
2. Kun hakemistosynkronointi on valmis, varmista, että organisaation Windows 10 -laitteet on liitetty Azure AD:hen. Tämä vaihe tehdään erikseen jokaisessa Windows 10 -laitteessa. Lisätietoja on ohjeaiheessa [Windows-laitteiden määrittäminen Microsoft 365 Business Premium -käyttäjille.](set-up-windows-devices.md) 
    
3. Kun Windows 10 -laitteet on liitetty Azure AD:hen, jokaisen käyttäjän on käynnistettävä laitteensa uudelleen ja kirjauduttava sisään Microsoft 365 Business Premium -tunnistetiedoillaan. Kaikilla laitteilla on nyt myös käytettävissään paikallisia resursseja.
    
Azure AD:n liitettyjen laitteiden paikallisten resurssien käyttäminen ei edellytä lisätoimia. Tämä toiminto sisältyy Windows 10:hen. 

Jos aiot kirjautua AADJ-laitteeseen muulla kuin salasanamenetelmällä Kuten PIN/Bio-metric WHFB-tunnistetietojen kirjautumisen kautta ja käyttää sitten paikallisia resursseja (osakkeita, tulostimia.. jne.), seuraahttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Jos organisaatiosi ei ole valmis ottamaan käyttöön edellä kuvatussa Azure AD:n liitetyssä laitemäärityksessä, harkitse [Hybrid Azure AD Joined -laitekokoonpanon](manage-windows-devices.md)määrittämistä.
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Huomioitavaa, kun liityt Windows-laitteisiin Azure AD:hen

Jos Azure-AD:hen liitetty Windows-laite oli aiemmin liittynyt toimialueeseen tai työryhmään, ota huomioon seuraavat rajoitukset:
  
- Kun laite Azure AD liittyy, se luo uuden käyttäjän viittaamatta aiemmin luotuun profiiliin. Profiilit on siirrettävä manuaalisesti. Käyttäjäprofiili sisältää tietoja, kuten suosikkeja, paikallisia tiedostoja, selaimen asetuksia ja Käynnistä-valikon asetuksia. Paras tapa on löytää kolmannen osapuolen työkalu, jolla voit yhdistää olemassa olevat tiedostot ja asetukset uuteen profiiliin.

- Jos laite käyttää ryhmäkäytäntöobjekteja, joillakin ryhmäkäytäntöobjekteilla ei ehkä ole vastaavaa [määrityspalvelun tarjoajaa](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) Intuessa. Suorita [MMAT-työkalu](https://www.microsoft.com/download/details.aspx?id=45520) löytääksesi vertailukelpoisia csps-organisaatioita olemassa oleville ryhmäkäytäntöobjekteille.

- Käyttäjät eivät voi todentaa active directory -todennuksesta riippuvaisiin sovelluksiin. Arvioi vanha sovellus ja harkitse päivittämistä sovellukseen, joka käyttää nykyaikaista auth-toimintoa, jos mahdollista.

- Active Directory -tulostimen etsintä ei toimi. Voit määrittää suoria tulostinpolkuja kaikille käyttäjille tai käyttää [Hybrid Cloud Print -palvelua.](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)
