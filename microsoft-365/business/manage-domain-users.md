---
title: Toimialuekäyttäjien synkronoiminen Microsoft 365
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Synkronoi toimialueohjatut käyttäjät Microsoft 365 for Businessin kanssa.
ms.openlocfilehash: 468fa943df55b12573f0a4f595294e39a146b1850f3c430ac2088a30991c0e60
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809308"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Toimialuekäyttäjien synkronoiminen Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. Hakemistosynkronoinnin valmistelu 

Ennen kuin synkronoit käyttäjät ja tietokoneet paikallisesta Active Directory -toimialueesta, lue artikkeli [Hakemistosynkronoinnin valmisteleminen Microsoft 365.](../enterprise/prepare-for-directory-synchronization.md) Erityisesti:

   - Varmista, että hakemistossa ei ole kaksoiskappaleita seuraaville määritteet: **mail,** **proxyAddresses** ja **userPrincipalName.** Näiden arvojen on oltava yksilöllisiä ja kaksoiskappaleet on poistettava.
   
   - Suosittelemme, että määrität kunkin paikallisen **käyttäjätilin userPrincipalName** (UPN) -määritteen vastaamaan ensisijaista sähköpostiosoitetta, joka vastaa Microsoft 365 sähköpostiosoitetta. Esimerkki:  mary.shelley@contoso.com.local mary@contoso *sijaan*
   
   - Jos Active Directory -toimialueen loppuliite päättyy ei-reititettävään jälkiliitteeseen, kuten *.local* tai *.lan*, internet-reititettävän jälkiliitteen, kuten *.com* tai *.org,* sijaan, muuta paikallisten käyttäjätilien UPN-jälkiliitettä ensin artikkelissa Ei-reititystäisen toimialueen valmisteleminen hakemistosynkronointia varten kuvatulla [tavalla.](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md) 

Suorita **IdFix alla** olevassa vaiheessa 4 (4) varmistaa myös, että paikallinen Active Directory on valmis hakemistosynkronointia varten.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Azure AD -määrityksen Näyttöyhteys

Jos haluat synkronoida käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directory, asenna Azure Active Directory Näyttöyhteys ja määritä hakemistosynkronointi. 

 1. Valitse [hallintakeskuksessa](https://go.microsoft.com/fwlink/p/?linkid=2024339) **Asetukset** vasemmassa siirtymisruudussa.

 2. Valitse **Kirjautumis- ja suojaus -kohdassa** **Näytä**  kohdassa **Synkronoi käyttäjät organisaatiosi hakemistosta**.

 3. Valitse **Synkronoi käyttäjät organisaatiosi hakemistosta** -sivulla **Aloita.**

 4. Suorita ensimmäisessä vaiheessa IdFix-työkalu hakemistosynkronointia varten.

 5. Lataa Azure AD Näyttöyhteys noudattamalla ohjatun toiminnon ohjeita ja synkronoi toimialueohjatut käyttäjät Microsoft 365.


Katso [lisätietoja artikkelista Hakemistosynkronoinnin Microsoft 365](../enterprise/set-up-directory-synchronization.md) määrittäminen.

Kun määrität Azure AD Näyttöyhteys -asetuksia, on suositeltavaa ottaa käyttöön salasanasynkronointi  **,** saumaton kertakirjautuminen ja salasanan takaisinkirjaintoiminto, jota tuetaan myös Microsoft 365 for Businessissa. 

> [!NOTE]
> Salasanalla kirjoitettavalle ruudulle on muutamia lisävaiheita Azure AD Näyttöyhteys. Lisätietoja on kohdassa Ohjeet [salasanan takaisin kirjoittautumista varten.](/azure/active-directory/authentication/howto-sspr-writeback) 

Jos haluat myös hallita toimialueeseen liitettyjä Windows 10-laitteita, katso kohta Toimialueeseen liitettyjen Windows 10 -laitteiden hallinnan salliminen [Microsoft 365 Business Premium](manage-windows-devices.md) Azure AD Join -yhdistelmäympäristön hallittavaksi.