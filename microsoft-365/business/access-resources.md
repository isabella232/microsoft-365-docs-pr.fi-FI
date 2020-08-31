---
title: Paikallisten resurssien käyttäminen Azure AD-liitetyissä laitteissa Microsoft 365 Business-sovelluksessa
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
description: Opi, miten voit käyttää paikallisia resursseja, kuten yritys sovelluksia, jaettuja tiedostoja ja tulostimia Azure Active Directorysta, jotka liittyivät Windows 10-laitteeseen.
ms.openlocfilehash: 9b83781afee746b06bbdf90962de0f55ffbcb118
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/29/2020
ms.locfileid: "47307489"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Paikallisten resurssien käyttäminen Azure AD-liitetyissä laitteissa Microsoft 365 Business Premiumissa

Tämä artikkeli koskee Microsoft 365 Business Premiumia.

Mikä tahansa Windows 10-laite, joka on Azure Active Directory liitetty, voi käyttää kaikkia pilvipohjaisia resursseja, kuten Microsoft 365-sovelluksia, ja se on suojattu Microsoft 365 Business Premiumin avulla. Voit myös sallia paikallisten resurssien, kuten yritys sovellusten, jaettujen tiedostojen ja tulostimien, käytön. Jos haluat sallia käyttö oikeuden, synkronoi paikallinen Active Directory Azure Active Directoryssa Azure [AD Connectin](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) avulla. 

Lisä tietoja on artikkelissa [Johdatus laite hallintaan Azure Active Directoryssa](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
Vaiheet on koottu myös seuraaviin kohtiin.

> [!IMPORTANT]
> Tämä toiminto on käytettävissä vain OAuth-ja NTLM-muodoissa. Kerberos-protokollaa ei voi käyttää.
 
## <a name="run-azure-ad-connect"></a>Azure AD Connectin suorittaminen

Noudata seuraavia vaiheita, jotta organisaatiosi Azure AD-laitteet voivat käyttää paikallisia resursseja.
  
1. Synkronoi käyttäjät, ryhmät ja yhteys tiedot paikallisesta Active Directorysta Azure Active Directoryyn suorittamalla ohjattu hakemisto synkronointi ja Azure AD Connect kohdassa [Office 365-hakemisto synkronoinnin määrittäminen](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization)kuvatulla tavalla.
    
2. Kun hakemisto synkronointi on valmis, varmista, että organisaatiosi Windows 10-laitteet on liitetty Azure AD:hen. Tämä vaihe suoritetaan yksitellen kaikissa Windows 10-laitteissa. Lisä tietoja on Ohje aiheessa [Windows-laitteiden määrittäminen Microsoft 365 Business Premium-käyttäjille](set-up-windows-devices.md) . 
    
3. Kun Windows 10-laitteet on liitetty Azure AD:hen, jokaisen käyttäjän on käynnistettävä laitteensa uudelleen ja kirjauduttava sisään Microsoft 365 Business Premium-tunniste tiedoillaan. Kaikki laitteet voivat nyt käyttää myös paikallisia resursseja.
    
Muita vaiheita ei tarvita, jotta voit käyttää paikallisia resursseja Azure AD-laitteeseen liitetyissä laitteissa. Tämä toiminto on sisällytetty Windows 10: een. 

Jos haluat kirja utua AADJ-laitteeseen, joka ei ole sama kuin salasana menetelmä, kuten PIN/Bio-metric WHFB-tunniste tietojen kirjautumistoiminnolla, ja sitten käyttää paikallisia resursseja (osakkeita, tulostimia... jne.), noudata seuraavia ohjeita. https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Jos organisaatiosi ei ole valmis ottamaan käyttöön edellä kuvattua Azuren Active Device-määritystä, harkitse [yhdistelmä Azure AD-liitetyn laite kokoonpanon](manage-windows-devices.md)määrittämistä.
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Huomioitavaa, kun liityt Windows-laitteisiin Azure AD:hen

Jos Windows-laite, jonka Azure-AD on liittynyt aiemmin toimi alueen mukaan tai työryhmään, huomioi seuraavat rajoitukset:
  
- Kun laite Azure AD liittyy, se luo uuden käyttäjän viittaamatta olemassa olevaan profiiliin. Profiilit on siirrettävä manuaalisesti. Käyttäjä profiili sisältää tietoja, kuten Suosikit, paikalliset tiedostot, selaimen asetukset ja aloitus valikon asetukset. Paras tapa on löytää kolmannen osapuolen työkalu, jonka avulla voit yhdistää nykyiset tiedostot ja asetukset uuteen profiiliin.

- Jos laite käyttää ryhmä käytäntö objekteja, joillakin ryhmä käytäntö objekteilla ei ehkä ole vastaavaa [määritys palveluiden tarjoajaa](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) Intunella. Jos haluat etsiä olemassa olevia ryhmä käytäntö objekteja, käytä [mmat-työkalua](https://www.microsoft.com/download/details.aspx?id=45520) .

- Käyttäjät eivät pysty todentamaan sovelluksia, jotka ovat riippuvaisia Active Directory-todennuksesta. Voit arvioida vanhaa sovellusta ja päivittää sitä sovellukseen, joka käyttää modernia todennus ohjelmaa, jos se on mahdollista.

- Active Directory-tulostimen etsintä ei toimi. Voit määrittää kaikille käyttäjille suorat tulostus polut tai käyttää [yhdistelmä pilvi tulostusta](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
