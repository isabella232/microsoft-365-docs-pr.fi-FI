---
title: Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Lue lisä tietoja siitä, miten Microsoft 365 voi suojata paikallisia mainoksia, jotka on liitetty Windows 10-laitteisiin.
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992225"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi

Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Businessin suojaamaan Windows 10-laitteitasi samalla, kun ylläpidämme paikallisen todennuksen edellyttävien paikallisten resurssien käyttö oikeuksia. Voit määrittää tämän ensin synkronoimalla Active Directory-hakemisto palvelun Azure Active Directoryn kanssa, jonka jälkeen rekisteröit Windows 10-laitteet Azure AD:N avulla ja rekisteröimällä ne mobiililaitteiden hallintaan Microsoft 365 Businessilla.
Seuraavassa videossa kerrotaan, miten tämä määritetään tavallisimmille skenaariolle.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Toimi alueeseen liitettyjen laitteiden määrittäminen Microsoft 365 Businessin hallitsemista varten

Jos haluat määrittää organisaatiosi toimi alueeseen liitetyt laitteet hyödyntämään Azure Active Directoryn tarjoamia ominaisuuksia paikallisen Active Directoryn lisäksi, voit ottaa käyttöön **hybridi Azure AD-liitetyt laitteet**. Nämä ovat laitteita, jotka on liitetty paikalliseen Active Directoryyn ja Azure Active Directoryyn. Hybridi-Azure AD liitetyt laitteet voidaan suojata ja hallita Microsoft 365 Business. 
  
Suorita seuraavat vaiheet, jotta Windows 10-laitteesi hybridi-Azure AD yhdistetään ja sitä hallinnoi Microsoft 365 Business.
  
1. Synkronoi käyttäjät, ryhmät ja yhteys tiedot paikallisesta Active Directorysta Azure Active Directoryyn suorittamalla ohjattu hakemiston synkronointi ja Azure Active Directory Connect kuvatulla tavalla kohdassa [Office 365 Directory-synkronointi](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
    > [!NOTE]
    > Vaiheet ovat täsmälleen samat Microsoft 365-liike toiminnan osalta. 
  
2. Ennen kuin suoritat vaiheen 3, jotta Windows 10-laitteet voivat olla hybridi-Azure AD liittynyt, sinun on varmistettava, että seuraavat edellytykset täyttyvät:

   - Käytössäsi on Azure AD Connectin uusin versio.

   - Azure AD Connect on synkronoinut kaikki niiden laitteiden tieto kone objektit, joihin haluat hybridi Azure AD-liittyneen. Jos tieto kone objektit kuuluvat tiettyihin organisaatio yksiköihin (OU), varmista, että ne on määritetty synkronoitaviksi myös Azure AD Connectin avulla.
    
3. Rekisteröi olemassa olevat toimi alue-liitetyt Windows 10-laitteet hybridi-Azure AD-Liittymiksi ja rekisteröimällä ne mobiililaitteiden hallintaan Intune-laitteella (Microsoft 365 Business):
    
4. Noudata vaiheittaisia ohjeita [hybridi Azure Active Directoryn liitettyjen laitteiden määrittämisestä](https://go.microsoft.com/fwlink/p/?linkid=872870). Tämä mahdollistaa paikallisen Active Directory-synkronoinnin liityttyä Windows 10-tieto koneisiin ja tekee niistä pilvi valmiina.
    
5. Jos haluat rekisteröidä Windows 10-laitteen mobiililaitteiden hallintaa varten, Katso ohjeet [Windows 10-laitteen ilmoittamisen Intune-toiminnolla ryhmä käytännön avulla](https://go.microsoft.com/fwlink/p/?linkid=872871) . Voit määrittää ryhmä käytännön paikallisen tieto koneen tasolla tai joukko toimintoja varten, voit luoda tämän ryhmä käytäntö asetuksen toimi alueen ohjaus kone palvelimessa.