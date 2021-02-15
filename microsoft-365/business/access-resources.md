---
title: Paikallisen resurssien käyttö Azure AD:stä yhdistetystä laitteesta Microsoft 365 Businessissa
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
description: Lue, miten voit käyttää paikallisia resursseja, kuten yrityssovelluksia, jaellisia tiedostoja ja tulostimia Azure Active Directoryyn yhdistetystä Windows 10 -laitteesta.
ms.openlocfilehash: fc02fd30f41f25f52e653e750a6bdfd1bd7f800e
ms.sourcegitcommit: a62ac3c01ba700a51b78a647e2301f27ac437c5a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2021
ms.locfileid: "50233836"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Käytä paikallisia resursseja Azure AD:llä yhdistetystä laitteesta Microsoft 365 Business Premiumissa

Tämä artikkeli koskee Microsoft 365 Business Premiumia.

Kaikki Azure Active Directoryyn yhdistetyt Windows 10 -laitteet voivat käyttää kaikkia pilvipohjaisia resursseja, kuten Microsoft 365 -sovelluksia, ja ne voidaan suojata Microsoft 365 Business Premiumilla. Voit myös sallia pääsyn paikallisiin resursseihin, kuten liiketoiminta-sovelluksiin, jaekkeisiin ja tulostimien. Jos haluat sallia käytön, synkronoi paikallinen Active Directory Azure Active Directoryn kanssa Azure [AD Connectin](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) avulla. 

Lisätietoja on ohjeaiheessa Johdanto Azure [Active Directoryn laitehallintaan.](https://docs.microsoft.com/azure/active-directory/device-management-introduction)
Vaiheiden yhteenveto on myös seuraavissa osissa.
 
## <a name="run-azure-ad-connect"></a>Azure AD Connectin käyttö

Noudata seuraavia ohjeita, jotta organisaatiosi Azure AD:ssä olevat laitteet voivat käyttää paikallisia resursseja.
  
1. Jos haluat synkronoida käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directoryyn, suorita ohjattu hakemistosynkronointitoiminto ja Azure AD Connect artikkelissa Hakemistosynkronoinnin määrittäminen [Office 365:lle kuvatulla tavalla.](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization)
    
2. Kun hakemistosynkronointi on valmis, varmista, että organisaatiosi Windows 10 -laitteet on liitetty Azure AD:n kanssa. Tämä vaihe tehdään yksitellen kussakin Windows 10 -laitteessa. Lisätietoja [on kohdassa Windows-laitteiden määritäminen Microsoft 365 Business Premium](set-up-windows-devices.md) -käyttäjille. 
    
3. Kun Windows 10 -laitteet on liitetty Azure AD:llä, kunkin käyttäjän on käynnistettävä laitteensa uudelleen ja kirjauduttava sisään Microsoft 365 Business Premium -tunnistetiedoillaan. Kaikilla laitteilla on nyt myös pääsy paikallisiin resursseihin.
    
Azure AD:ssä liitettyjen laitteiden paikallisiin resursseihin pääsy ei vaadi lisätoimia. Tämä toiminto on integroitu Windows 10:ssä. 

Jos sinun on suunnitelmissa kirjautua AADJ-laitteeseen muulla kuin salasanamenetelmällä, kuten PIN/Bio-metrinen, WHFB-tunnistetietokirjautumisen kautta ja käyttää sitten paikallisia resursseja (jakamia, tulostimia. jne.), seuraa https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Jos organisaatiosi ei ole valmis ottamaan käyttöön edellä kuvatun Azure AD:n liitettyjen laitteiden määrityksessä, harkitse [Azure AD:ksi](manage-windows-devices.md)liitettyjen yhdistelmälaitemääritysten käyttöönottoa.
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Huomioon otettavia seikkoja liittyessäsi Windows-laitteisiin Azure AD:ssä

Jos Azure-AD:llä liitetty Windows-laite on aiemmin liitetty toimialueeseen tai työryhmään, ota huomioon seuraavat rajoitukset:
  
- Kun Azure AD -laite liittyy, se luo uuden käyttäjän viittaamatta aiemmin luotuun profiiliin. Profiilit on siirrettävä manuaalisesti. Käyttäjäprofiili sisältää tietoja, kuten suosikit, paikalliset tiedostot, selaimen asetukset ja aloitusvalikon asetukset. Paras tapa on etsiä kolmannen osapuolen työkalu olemassa olevien tiedostojen ja asetusten kartoittamiseen uuteen profiiliin.

- Jos laite käyttää ryhmäkäytäntöobjekteja (GPO), joillakin ryhmäkäytäntöobjekteilla ei ehkä ole vastaavaa kokoonpanopalveluntarjoajaa Intunessa. [](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) Suorita [MMAT-työkalu löytääksesi](https://www.microsoft.com/download/details.aspx?id=45520) vastaavat CSPs:t olemassa oleville ryhmäkäytäntöobjekteille.

- Käyttäjät eivät ehkä voi todentaa Sovelluksia, jotka ovat riippuvaisia Active Directory -todennuksista. Arvioi vanha sovellus ja harkitse päivittämistä sovellukseen, joka käyttää modernia todnttia, jos mahdollista.

- Active Directory -tulostimen etsintä ei toimi. Voit määrittää suoran tulostimen polut kaikille käyttäjille tai käyttää [universaalia tulostusta.](https://aka.ms/UPDocs)
