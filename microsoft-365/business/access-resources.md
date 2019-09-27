---
title: Paikallisten resurssien käyttö Azure AD-liitetystä laitteesta Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Opi, miten voit käyttää paikallisia resursseja, kuten yritys sovelluksia, tiedosto resursseja ja tulostimia Azure Active Directorysta, liittyi Windows 10-laitteeseen.
ms.openlocfilehash: 26ba0ffb64ddce32369002120657456e47ac0c7f
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287351"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Paikallisten resurssien käyttö Azure AD-liitetystä laitteesta Microsoft 365 Business

Kaikissa Windows 10-laitteilla, joihin on liitetty Azure Active Directory, on pääsy kaikkiin pilvipohjaisiin resursseihin, kuten Office 365-sovelluksiin, ja ne voidaan suojata Microsoft 365 Businessin avulla. Jos haluat sallia myös paikallisten resurssien, kuten Business Line (LOB)-sovellusten, jaettujen tiedostojen ja tulostimien käytön, synkronoi paikallinen Active Directory Azure Active Directoryn kanssa [Azure AD Connectin](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect)avulla. 

Lisä tietoja on kohdassa [laitteen hallinnan esittely Azure Active Directoryssa](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) .
Vaiheet on myös tiivistetty seuraavissa osissa.

## <a name="run-azure-ad-connect"></a>Suorita Azure AD Connect

Suorita seuraavat vaiheet, jotta organisaatiosi Azure AD-liitetyt laitteet voivat käyttää paikallisia resursseja.
  
1. Jos haluat synkronoida käyttäjät, ryhmät ja yhteys tiedot paikallisesta Active Directorysta Azure Active Directoryyn, suorita ohjattu hakemiston synkronointi ja Azure AD Connect kuvatulla tavalla kohdassa [Office 365 Directory-synkronointi](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Kun hakemiston synkronointi on suoritettu, varmista, että organisaatiosi Windows 10-laitteet on liitetty Azure AD-palveluun. Tämä vaihe tehdään erikseen kussakin Windows 10-laitteessa. Lisä tietoja on kohdassa [Windows-laitteiden määrittäminen Microsoft 365-yritys käyttäjille](set-up-windows-devices.md) . 
    
3. Kun Windows 10-laitteet ovat liittyneet Azure AD, jokaisen käyttäjän tulee käynnistää laitteensa uudelleen ja kirja utua sisään Microsoft 365-yrityksen tunniste tiedoilla. Kaikki laitteet saavat nyt käyttöönsä myös paikallisia resursseja.
    
Azure AD-liitettyjen laitteiden paikallisten resurssien käyttö oikeuksia ei tarvita lisä toimia. Tämä on Windows 10: ssä käytettävissä oleva sisäänrakennettu toiminto. 
  
Jos organisaatiosi ei ole valmis ottamaan käyttöön yllä kuvattua Azure AD Joined-laitteen kokoonpanoa, harkitse [hybridi Azure AD-laitteen kokoonpanon](manage-windows-devices.md)määrittämistä.
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a>Windows-laitteisiin Azure ADIIN liittyessään liittyvät seikat

Jos olet Azure AD, joka liittyy sellaiseen Windows-laitteeseen, joka on aiemmin ollut toimi alueeseen liitetty tai työryhmässä, sinun on otettava huomioon seuraavat rajoitukset:
  
- Kun laite Azure AD liittyy, se luo uuden käyttäjän viittaamatta olemassa olevaan profiiliin. Profiilien korjaaminen edellyttää, että profiilit siirretään manuaalisesti. Käyttäjä profiili sisältää tietoja, kuten Suosikit, paikalliset tiedostot, selaimen asetukset, Käynnistä-valikon asetukset jne. Paras tapa on löytää kolmannen osapuolen työkalu, jolla voit yhdistää olemassa olevat tiedostot ja asetukset uuteen profiiliin

- Jos laite käyttää ryhmä käytäntö objekteja, joissakin GPOs-sovelluksessa ei ehkä ole vastaavaa [määritys palvelun toimittajaa](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) Intune-kohteessa. Suorita [mmat-työkalu](https://www.microsoft.com/download/details.aspx?id=45520) löytääksesi vertailukelpoisia csps-virheitä olemassa oleville ryhmä käytäntö objekteja varten.

- Käyttäjät eivät voi todentaa Active Directory-todennuksesta riippuvaisia sovelluksia. Voit käsitellä tätä arvioida vanhan sovelluksen avulla ja harkita päivittämistä sovellukseen, joka käyttää modernia auth jos mahdollista.

- Active Directory-tulostimien etsiminen ei toimi. Voit korjata tämän, tarjota suorat tulostus polut kaikille käyttäjille tai hyödyntää [Hybrid Cloud Print-palvelun](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
