---
title: Toimi alueen käyttäjien synkronoiminen Microsoft 365
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
description: Synkronoi toimi alueen valvottavat käyttäjät Microsoft 365 for Businessin kanssa.
ms.openlocfilehash: 9495d893eb6870ef7c417a78f921296bfc0e6705
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306445"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Toimi alueen käyttäjien synkronoiminen Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. hakemisto synkronoinnin valmisteleminen 

Ennen kuin synkronoit käyttäjät ja tieto koneet paikallisesta Active Directory-toimi alueesta, tarkista [Hakemisto synkronoinnin valmisteleminen Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization). Erityisesti:

   - Varmista, ettei hakemistossasi ole kaksoiskappaleita seuraavista määritteistä: **Sähkö posti**, **proxyAddresses**ja **userPrincipalName**. Näiden arvojen on oltava yksilöllisiä, ja kaikki kaksoiskappaleet on poistettava.
   
   - Suosittelemme määrittämään kunkin paikallisen käyttäjä tilin **userPrincipalName** (UPN)-määritteen vastaamaan Microsoft 365-käyttö oikeutta vastaavaa pääsähkö posti osoitetta. Esimerkki: *Mary.Shelley@contoso.com* sen sijaan, että *Mary@contoso. Local*
   
   - Jos Active Directory-toimi alueen pääte on muu kuin reititettävissä oleva jälki liite (esimerkiksi. *Local* tai *. LAN*) sen sijaan, että käytössä olisi Internet-reititettävissä oleva jälki liite, kuten *. com* tai *. org*, voit muuttaa paikallisten käyttäjä tunnusten UPN-jälki liitettä ensin, kun [olet kuvannut ei-reititettävän toimi alueen määrittäminen hakemisto synkronointia](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization) 

Vaiheen neljä (4) **Suorita IdFix-korjaus** varmistaa myös, että paikallinen Active Directory on valmiina dir-synkronointia varten.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Azure AD Connectin asentaminen ja määrittäminen

Jos haluat synkronoida paikallisen Active Directoryn käyttäjät, ryhmät ja yhteys tiedot Azure Active Directoryyn, asenna Azure Active Directory Connect ja Määritä hakemisto synkronointi. 

 1. Valitse hallinta keskuksessa <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> vasemmanpuoleisen siirtymis palkin **Asetukset** -kohdassa.

 2. Valitse **Kirjautuminen ja tieto turva**-kohdassa **oman organisaatiosi hakemiston Synkronoi käyttäjät**-kohdassa **Näytä** .

 3. Valitse organisaatiosi **hakemisto-sivun Synkronoi käyttäjät** -kohdassa **aloittaminen**.

 4. Voit valmistella hakemisto synkronoinnin ensimmäisessä vaiheessa suorittamalla IdFix-työkalun.

 5. Lataa Azure AD Connect noudattamalla ohjatun toiminnon ohjeita ja synkronoi toimi alueen hallitsemat käyttäjät Microsoft 365-palvelussa sen avulla.


Lisä tietoja on artikkelissa [Hakemisto synkronoinnin määrittäminen Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) -käyttöön.

Kun määrität asetukset Azure AD Connect-sovelluksessa, suosittelemme, että otat käyttöön **Sala sanojen synkronoinnin**, **saumattoman kertakirjautumisen**ja **Sala sanan takaisinkirjoitusominaisuuden** , jota tuetaan myös Microsoft 365 for Businessissa.

> [!NOTE]
> Sala sanan takaisinkirjoitus on käytettävissä myös muilla tavoilla Azure AD Connectin valinta ruudun ulkopuolella. Lisä tietoja on Ohje aiheessa [toiminta ohjeet: Sala sanan takaisinkirjoitus-kohdan määrittäminen](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

Jos haluat hallita toimi alueen mukaan liitetyissä Windows 10-laitteissa, Katso lisä tietoja artikkelista [Microsoft 365 Business Premiumin hallinnoitava toimi alue-yhdistetyt Windows 10-laitteet](manage-windows-devices.md) , jotta voit määrittää yhdistelmä ympäristön Azure AD Join. 