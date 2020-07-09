---
title: Toimialueen käyttäjien synkronoiminen Microsoft 365:ksi
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
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
- MOE150
description: Synkronoi toimialueen hallitut käyttäjät Microsoft 365 for Businessin kanssa.
ms.openlocfilehash: af9cb7c9b2b639edc2375679a73ab41c4cf6de71
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081848"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Toimialueen käyttäjien synkronoiminen Microsoft 365:ksi

## <a name="1-prepare-for-directory-synchronization"></a>1. Hakemistosynkronoinnin valmisteleminen 

Ennen kuin synkronoit käyttäjät ja tietokoneet paikallisesta Active Directory -toimialueesta, tutustu [ohjeaiheeseen Hakemistosynkronoinnin valmisteleminen Microsoft 365:ksi](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Erityisesti:

   - Varmista, että hakemistossasi ei ole kaksoiskappaleita seuraaville määritteille: **sähköposti,** **proxyAddresses**ja **userPrincipalName**. Näiden arvojen on oltava yksilöllisiä ja kaksoiskappaleet on poistettava.
   
   - Microsoft suosittelee, että määrität **userPrincipalName** (UPN) -määritteen kullekin paikalliselle käyttäjätilille vastaamaan lisensoitua Microsoft 365 -käyttäjää vastaavaa ensisijaista sähköpostiosoitetta. Esimerkki: *mary.shelley@contoso.com* *mary@contoso.local*
   
   - Jos Active Directory -toimialue päätyy ei-reititettävään liitteeseen , kuten *.local* tai *.lan*, internet-reititettävän liitteen , kuten *.com* tai *.org*, sijaan , säädä paikallisten käyttäjätilien UPN-liite ensin kohdassa [Ei-reititettävän toimialueen valmisteleminen hakemistosynkronointia varten](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)kuvatulla tavalla . 

**Suorita IdFix** vaiheessa neljä (4) alla, myös varmistaa paikallinen Active Directory on valmis dir sync.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Asenna ja määritä Azure AD Connect

Jos haluat synkronoida paikallisen Active Directoryn käyttäjät, ryhmät ja yhteystiedot Azure Active Directoryyn, asenna Azure Active Directory Connect ja määritä hakemistosynkronointi. 

 1. Valitse hallintakeskuksessa <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Asetukset** vasemmassa siirtymisruudussa.

 2. Valitse **Kirjautumis- ja suojaus -kohdassa** **Synkronoi käyttäjiä organisaatiosi hakemistosta**-kohdassa **Näytä** .

 3. Valitse **Synkronoi käyttäjät organisaatiosi hakemistosivulta** **Aloita**.

 4. Ensimmäisessä vaiheessa suorita IdFix työkalu valmistautua Hakemistosynkronointia.

 5. Lataa Azure AD Connect ohjatun toiminnon ohjeiden avulla ja synkronoi sen avulla toimialueohjatut käyttäjät Microsoft 365:ksi.


Lisätietoja on [ohjeaiheessa Microsoft 365:n hakemistosynkronoinnin määrittäminen.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)

Kun määrität Azure AD Connectin asetukset, suosittelemme, että otat käyttöön **salasanan synkronoinnin,** **saumattoman kertakirjautuksen**ja **salasanan takaisinkirjoitusominaisuuden,** jota myös Microsoft 365 for Business tukee.

> [!NOTE]
> Azure AD Connectin valintaruudun lisäksi salasanan takaisinkirjoituksessa on joitakin lisävaiheita. Lisätietoja on [ohjeaiheessa Toimintaohjeet: salasanan takaisinkirjoituksen määrittäminen](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

Jos haluat hallita myös toimialueeseen liitettyjä Windows 10 -laitteita, katso lisätietoja ohjeaiheesta [Toimialueen käyttöönottamien windows 10 -laitteiden ottaminen käyttöön Microsoft 365 Business Premiumin hallinnassa](manage-windows-devices.md) azure AD -yhdistelmäliitoksen määrittämiseksi. 