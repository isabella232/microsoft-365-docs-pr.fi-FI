---
title: Käyttää tiloissa Azure AD liitetty laite 365 Microsoft Business resurssit
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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Opi hyödyntämään tiloissa resurssien käyttöä, kuten Windows 10-laite on liitetty liiketoiminnan rivin apps, jaettujen tiedostojen ja tulostimien Azure Active Directory-hakemistopalvelusta.
ms.openlocfilehash: fa3cf640e799feb81ff08c5b7b81d57f707e0152
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072026"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Käyttää tiloissa Azure AD liitetty laite 365 Microsoft Business resurssit

Windows 10-laitteeseen, joka on liittynyt Azure Active Directory on käsitellä kaikkia pilvi-pohjainen Office 365-apps ja suojataan Microsoft 365 Business. Voit myös sallia pääsyn paikalliseen resursseja, kuten viiva, Business (LOB) apps, jaettujen tiedostojen ja tulostimien, synkronoi paikallisen Active Directory Azure Active Directoryn kanssa [Azure AD-yhteyden](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect)avulla. Katso lisätietoja [Azure Active Directoryn hallinta esittely](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) . 
  
## <a name="run-azure-ad-connect"></a>Suorita Azure AD muodostaa

Tee seuraavat toimet organisaation Azure AD liittynyt laitteissa tiloissa resurssien käytön.
  
1. Synkronoi käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directoryyn, ohjatun kansion synkronoinnin ja Azure AD Yhdistä [Office 365 directory-synkronoinnin määrittäminen](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)kuvataan.
    
2. Kun directory-synkronointi on valmis, varmista, että organisaation Windows 10 laitteet liitetty Azure AD. Tämä vaihe tehdään erikseen kunkin Windows 10-laitteen. Lisätietoja [laitteiden Windows Microsoft 365 Business käyttäjien määrittäminen](set-up-windows-devices.md) . 
    
3. Kun Windows 10-laitteet on liitetty Azure AD, jokaisella käyttäjällä tulisi uudelleen niiden laitteiden ja kirjautumisen käyttäjätiedot Microsoft 365 Business kanssa. Kaikki laitteet on nyt omissa tiloissa sekä resurssien käytön.
    
Ei lisätoimia pääsyä tiloissa Azure AD resurssit on liitetty laitteita. Tämä on sisäinen toiminto käytettävissä Windows 10. 
  
Jos organisaatiosi ei ole valmis ottamaan Azure AD liittynyt laitteen kokoonpanosta edellä kuvatun, kannattaa asentaa [hybridi Azure AD Joined laitteen kokoonpanotietoja](manage-windows-devices.md).
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a>Huomioon otettavia laitteita Windows Azure AD liittäminen

Azure AD liittäminen Windows-laite, joka on aiemmin ollut toimialueeseen liittymistä tai työryhmässä, sinun on otettava huomioon seuraavat rajoitukset:
  
- Azure AD laite liitetään, se luo uuden käyttäjän ei viittaa olemassa olevaan profiiliin. Voit korjata tämän ongelman profiilit on siirrettävä manuaalisesti. Käyttäjäprofiili sisältää tietoja, kuten Suosikit, paikallisia tiedostoja, selaimesi asetuksia, Käynnistä-valikkoasetukset jne. Paras tapa on löytää kolmannen osapuolen työkalu yhdistää olemassa olevat tiedostot ja asetukset uuteen profiiliin

- Jos laite käyttää ryhmän Policy Objects (GPO), joitakin ryhmäkäytäntöobjekteja ei ole välttämättä verrattavissa [Kokoonpano tarjoaja](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) Intune. Löydä vastaavaa CSP aiemmin ryhmäkäytäntöobjekteja [MMAT työkalun](https://www.microsoft.com/download/details.aspx?id=45520) suorittaminen

- Käyttäjät eivät voi todentaa Active Directory-todennus riippuvat sovellukset. Tämä vanha app käytön arvioiminen ja harkitse päivittämistä app, joka käyttää nykyaikaisia Auth Jos mahdollista.

- Active Directory-tulostimen etsimisen ei toimi. Voit korjata tämän ongelman suoraan tulostimen polut tarjoavat kaikille käyttäjille tai hyödyntää [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
