---
title: Paikallisten resurssien käyttäminen Azure AD-liitetystä laitteesta Microsoft 365 Businessissa
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Lue, miten voit käyttää paikallisia resursseja, kuten yrityssovelluksia, jaettuja tiedostoresursseja ja tulostimia Azure Active Directorysta, joka liittyi Windows 10 -laitteeseen.
ms.openlocfilehash: 9615ecc9469992d3e5a7479f4799c610db11fb41
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471247"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Paikallisten resurssien käyttäminen Azure AD -liitetystä laitteesta Microsoft 365 Business Premiumissa

Tämä artikkeli koskee Microsoft 365 Business Premiumia.

Kaikilla Windows 10 -laitteilla, joihin On liitetty Azure Active Directory, on pääsy kaikkiin pilvipohjaisiin resursseihin, kuten Microsoft 365 -sovelluksiin, ja Microsoft 365 Business Premium voi suojata sen. Voit myös sallia paikallisten resurssien, kuten lob-sovellusten, jaettujen tiedostojen ja tulostimien, käytön. Jos haluat sallia käytön, synkronoi paikallinen Active Directory Azure Active Directoryn kanssa [Azure AD Connectin](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) avulla. 

Lisätietoja on [ohjeaiheessa Johdanto laitehallintaan Azure Active Directoryssa](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
Vaiheet on myös yhteenveto seuraavissa osissa.

> [!IMPORTANT]
> Tämä menettely koskee vain OAuth- ja NTLM-menetelmää. Kerberos ei ole tuettu.
 
## <a name="run-azure-ad-connect"></a>Azure AD Connectin suorittaminen

Toimi seuraavasti, jotta organisaation Azure AD -liitetyt laitteet voivat käyttää paikallisia resursseja.
  
1. Jos haluat synkronoida paikallisen Active Directoryn käyttäjät, ryhmät ja yhteystiedot Azure Active Directoryyn, suorita ohjattu hakemistosynkronointitoiminto ja Azure AD Connect kohdassa [Hakemistosynkronoinnin määrittäminen Office 365:tä varten](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)kuvatulla tavalla.
    
2. Kun hakemistosynkronointi on valmis, varmista, että organisaation Windows 10 -laitteet on liitetty Azure AD:hen. Tämä vaihe tehdään erikseen jokaisessa Windows 10 -laitteessa. Lisätietoja [on ohjeaiheessa Windows-laitteiden määrittäminen Microsoft 365 Business Premium -käyttäjille.](set-up-windows-devices.md) 
    
3. Kun Windows 10 -laitteet on liitetty Azure AD:hen, jokaisen käyttäjän on käynnistettävä laitteensa uudelleen ja kirjauduttava sisään Microsoft 365 Business Premium -tunnistetiedoillaan. Kaikilla laitteilla on nyt pääsy myös paikallisiin resursseihin.
    
Azure AD -liitettyjen laitteiden paikallisia resursseja ei tarvita lisätoimia. Tämä toiminto sisältyy Windows 10:een. 

Jos sinulla on suunnitelmia kirjautua AADJ-laitteeseen muuhun kuin salasanamenetelmään, kuten PIN/Bio-metric WHFB-tunnistetietojen kirjautumisen kautta ja käyttää sitten paikallisia resursseja (jaetut resurssit,tulostimet. jne.), noudatahttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Jos organisaatiosi ei ole valmis ottamaan käyttöön edellä kuvatussa Azure AD:n liitetyn laitteen kokoonpanossa, harkitse [Hybrid Azure AD Joined -laitteen määrityksen](manage-windows-devices.md)määrittämistä .
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Huomioitavaa, kun liityt Windows-laitteisiin Azure AD:hen

Jos Azure-AD:hen liitetty Windows-laite on aiemmin liitetty toimialueeseen tai työryhmään, ota huomioon seuraavat rajoitukset:
  
- Kun laite, johon Azure AD liittyy, se luo uuden käyttäjän viittaamatta aiemmin luotuun profiiliin. Profiilit on siirrettävä manuaalisesti. Käyttäjäprofiili sisältää tietoja, kuten suosikkeja, paikallisia tiedostoja, selaimen asetuksia ja Käynnistä-valikon asetuksia. Paras tapa on löytää kolmannen osapuolen työkalu, jolla voit yhdistää olemassa olevat tiedostot ja asetukset uuteen profiiliin.

- Jos laite käyttää ryhmäkäytäntöobjekteja, joillakin ryhmäkäytäntöobjekteilla ei ehkä ole vastaavaa [määrityspalvelun tarjoajaa](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) Intutuessa. Suorita [MMAT-työkalu](https://www.microsoft.com/download/details.aspx?id=45520) löytääksesi vertailukelpoisia asiakaspalvelijaa nykyisille ryhmäkäytäntöobjekteille.

- Käyttäjät eivät voi todentaa sovelluksia, jotka ovat riippuvaisia Active Directory -todennuksesta. Arvioi vanha sovellus ja harkitse päivittämistä sovellukseen, joka käyttää modernia Authia, jos mahdollista.

- Active Directory -tulostimen etsintä ei toimi. Voit tarjota suoria tulostinpolkuja kaikille käyttäjille tai käyttää [Hybrid Cloud Print -toimintoa.](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)
