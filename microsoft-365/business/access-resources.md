---
title: Käytä paikallisia resursseja Azure AD:llä yhdistetystä laitteesta Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Opi käyttämään yrityksen sovelluksia, jaetut tiedostoresurssit ja tulostimet tai muut paikallisen Azure Active Directory Windows 10 avulla.
ms.openlocfilehash: 72b3c5ae538cad24fc12e25717dedccb2fdc9017
ms.sourcegitcommit: 4fb1226d5875bf5b9b29252596855a6562cea9ae
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/08/2021
ms.locfileid: "52843318"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Käytä paikallisia resursseja Azure AD:llä yhdistetystä laitteesta Microsoft 365 Business Premium

Tämä artikkeli koskee Microsoft 365 Business Premium.

Kaikki Windows 10, Azure Active Directory liitettyihin sovelluksiin, voivat käyttää kaikkia pilvipohjaisia resursseja, kuten Microsoft 365-sovelluksia, ja ne voidaan suojata Microsoft 365 Business Premium. Voit myös sallia pääsyn paikallisiin resursseihin, kuten liiketoiminta-sovelluksiin, jaekkeisiin ja tulostimien. Salli käyttö käyttämällä [Azure AD Näyttöyhteys:tä](/azure/active-directory/connect/active-directory-aadconnect) paikallisen Active Directoryn synkronoinnissa Azure Active Directory.

Lisätietoja on ohjeaiheessa Johdanto [laitehallintaan Azure Active Directory.](/azure/active-directory/device-management-introduction)
Vaiheiden yhteenveto on myös seuraavissa osissa.

## <a name="run-azure-ad-connect"></a>Azure AD -Näyttöyhteys

Suorita seuraavat vaiheet, jotta organisaatiosi Azure AD:llä yhdistetyt laitteet voivat käyttää paikallisia resursseja.

1. Jos haluat synkronoida käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directory, suorita ohjattu hakemistosynkronointitoiminto ja Azure AD Näyttöyhteys artikkelissa Hakemistosynkronoinnin määrittäminen [Office 365.](../enterprise/set-up-directory-synchronization.md)

2. Kun hakemistosynkronointi on valmis, varmista, että organisaation Windows 10 Azure AD:n liittäminen. Tämä vaihe tehdään yksitellen kussakin Windows 10 laitteessa. Lisätietoja [on Windows laitteiden Microsoft 365 Business Premium käyttäjille.](set-up-windows-devices.md)

3. Kun Windows 10 Azure AD:iin, jokaisen käyttäjän on käynnistettävä laitteensa uudelleen ja kirjauduttava Microsoft 365 Business Premium tunnistetiedoilla. Kaikilla laitteilla on nyt myös paikallisen resurssin käyttöoikeus.

Azure AD:ssä liitettyjen laitteiden paikallisen resurssien käyttö ei vaadi lisätoimia. Tämä toiminto on integroitu Windows 10.

Jos haluat kirjautua AADJ-laitteeseen muulla kuin salasanamenetelmällä, kuten PIN-/Bio-metrijärjestelmän kanssa WHFB-tunnistetietokirjautumisen kautta ja käyttää sitten paikallisia resursseja (jakoresursseja, tulostimia jne.), noudata tätä [artikkelia.](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

Jos organisaatiosi ei ole valmis ottamaan käyttöön edellä kuvatun Azure AD:n liitettyjen laitteiden määrityksessä, harkitse [Azure AD:llä yhdistetyn laitteen yhdistelmäkokoonpanon käyttöönottoa.](manage-windows-devices.md)

### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Huomioon otettavia asioita, kun Windows laitteisiin Azure AD:ssä

Jos Windows laite, jonka kanssa Azure-AD on liitetty, oli aiemmin liitetty toimialueeseen tai työryhmään, ota seuraavat rajoitukset huomioon:

- Kun azure AD -laite liittyy, se luo uuden käyttäjän viittaamatta aiemmin luotuun profiiliin. Profiilit on siirrettävä manuaalisesti. Käyttäjäprofiili sisältää tietoja, kuten suosikit, paikalliset tiedostot, selaimen asetukset ja aloitusvalikon asetukset. Paras tapa on etsiä kolmannen osapuolen työkalu, jolla olemassa olevat tiedostot ja asetukset voidaan yhdistää uuteen profiiliin.

- Jos laite käyttää ryhmäkäytäntöobjekteja (GPO), joillakin ryhmäkäytäntöobjekteilla ei välttämättä ole vastaavaa kokoonpanopalveluntarjoajaa Intunessa. [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) Suorita [MMAT-työkalu löytääksesi](https://www.microsoft.com/download/details.aspx?id=45520) vastaavat CSPs olemassa oleville ryhmäkäytäntöobjekteille.

- Käyttäjät eivät ehkä voi todentaa Sovelluksia, jotka ovat riippuvaisia Active Directory -todennuksista. Arvioi vanha sovellus ja harkitse päivitystä sovellukseen, joka käyttää modernia todnttia, jos mahdollista.

- Active Directory -tulostimen etsintä ei toimi. Voit määrittää suoran tulostimen polut kaikille käyttäjille tai käyttää [universaalia tulostusta.](/universal-print/)

### <a name="related-articles"></a>Aiheeseen liittyvät artikkelit

[Azure AD :n käytön edellytykset Näyttöyhteys](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
