---
title: Toimialuekäyttäjien synkronoiminen Microsoft 365:lle
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
description: Synkronoi toimialueohjatut käyttäjät Microsoft 365 for Businessin kanssa.
ms.openlocfilehash: 1c939dec7229f02991b15f08c48f184efecaddb0
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913250"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Toimialuekäyttäjien synkronoiminen Microsoft 365:lle

## <a name="1-prepare-for-directory-synchronization"></a>1. Hakemistosynkronoinnin valmisteleminen 

Ennen kuin synkronoit käyttäjät ja tietokoneet paikallisesta Active Directory -toimialueesta, tarkista Hakemistosynkronoinnin [valmisteleminen Microsoft 365:lle.](../enterprise/prepare-for-directory-synchronization.md) Erityisesti:

   - Varmista, että hakemistossa ei ole kaksoiskappaleita seuraaville määritteille: **mail,** **proxyAddresses** ja **userPrincipalName.** Näiden arvojen on oltava yksilöllisiä ja kaksoiskappaleet on poistettava.
   
   - Suosittelemme, että määrität kunkin paikallisen **käyttäjätilin userPrincipalName** (UPN) -määritteen vastaamaan ensisijaista sähköpostiosoitetta, joka vastaa lisensoituta Microsoft 365 -käyttäjää. Esimerkki: *mary.shelley@contoso.com.mary@contoso* *sijaan*
   
   - Jos Active Directory -toimialue päättyy ei-reititettävään jälkiliitteeseen, kuten *.local* tai *.lan,* internet-reititettävän jälkiliitteen, kuten *.com* tai *.org,* sijaan, muokkaa ensin paikallisten käyttäjätilien UPN-jälkiliitettä kohdassa Valmistele ei-reititettävä toimialue hakemistosynkronointia varten kuvatulla [tavalla.](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md) 

Suorita **IdFix vaiheessa** 4 (4) alla varmistaa myös, että paikallinen Active Directory on valmis hakemistosynkronointia varten.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Azure AD Connectin asentaminen ja määrittäminen

Jos haluat synkronoida käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directoryyn, asenna Azure Active Directory Connect ja määritä hakemistosynkronointi. 

 1. Valitse [hallintakeskuksessa](https://go.microsoft.com/fwlink/p/?linkid=2024339)Asetukset **vasemmassa** siirtymisruudussa.

 2. Valitse **Sisäänkirjautuminen ja suojaus -kohdassa** **Näytä** kohdassa Synkronoi **käyttäjät organisaatiosi hakemistosta.**

 3. Valitse **Organisaation hakemistosivun Synkronoi** käyttäjät -sivulla **Aloittaminen.**

 4. Suorita ensimmäisessä vaiheessa IdFix-työkalu hakemistosynkronointia varten.

 5. Lataa Azure AD Connect ohjatun toiminnon ohjeiden mukaisesti ja synkronoi sen avulla toimialueohjatut käyttäjät Microsoft 365:lle.


Lisätietoja [on kohdassa Hakemistosynkronoinnin](../enterprise/set-up-directory-synchronization.md) määrittäminen Microsoft 365:lle.

Kun määrität Azure AD Connectin asetukset, suosittelemme, että otat käyttöön salasanojen  synkronoinnin,  **saumattoman** kertakirjautunnin ja salasanan takaisinkirjaamista varten, jota tuetaan myös Microsoft 365 for Businessissa.

> [!NOTE]
> On joitakin lisävaiheita salasanan palautusta varten Azure AD Connectin valintaruudun ulkopuolella. Lisätietoja on ohjeaiheessa Ohjeet: salasanan [palautusten määrittäminen.](/azure/active-directory/authentication/howto-sspr-writeback) 

Jos haluat myös hallita toimialueeseen liitettyjä Windows 10 -laitteita, katso kohta Ota toimialueeseen yhdistetyt Windows 10 -laitteet käyttöön, joita [Microsoft 365 Business Premium hallitsee](manage-windows-devices.md) Azure AD -yhdistelmäympäristön liittämistä varten.