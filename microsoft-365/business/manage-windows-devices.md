---
title: Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
description: Microsoft suojaa 365 käyttöönotto paikallisen AD liittynyt Windows 10-laitteita.
ms.openlocfilehash: 661e5bf8205a661eb4382b4bdd8fcf3a54ecc12f
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660305"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi

Jos organisaatiossa käytetään Windows Server Active Directory tiloissa, voit määrittää Microsoft 365 liiketoiminnan suojaamaan Windows 10-laitteet, säilyttäen kuitenkin edellyttää paikallista todennusta tiloissa resurssien käytön. Voit tehdä tämän ensimmäisen synkronoida Active Directoryn Azure Active Directoryn, rekisteröitymisestä Azure AD Windows 10-laitteiden ja ei tarvitse ottaa niitä mukaan 365 Microsoft Business management kannettavan laitteen kanssa.
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Määritä laitteet toimialueeseen liittymistä hallinnoi 365 Microsoft Business

Määrittämään organisaation toimialueeseen liittymistä laitteet hyötyvät Azure Active Directoryssa paikallisen Active Directoryn lisäksi annettuja ominaisuuksia voit toteuttaa **hybridi Azure AD liitetyt laitteet**. Nämä ovat laitteita, jotka on liitetty toisiinsa sekä paikalliseen Active Directory-ja Azure-Active Directory. Hybrid liittynyt Azure AD laitteet on suojattu ja hallinnoi 365 Microsoft Business. 
  
Noudattamalla alla tehdä laitteiden Windows 10 Azure AD liittynyt ja hallitsema Microsoft 365 Business hybridi.
  
1. Synkronoi käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directoryyn, suorita ohjattu synkronoinnin Directory ja Azure Active Directory muodostaa yhteyden [Office 365: ssä directory-synkronoinnin määrittäminen](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)kuvatulla.
    
    > [!NOTE]
    > Vaiheet ovat täsmälleen samat 365 Microsoft Business. 
  
2. Ennen kuin suoritat vaiheen 3 Windows 10 Azure AD liittynyt Hybrid on laitteissa, sinun on Varmista, että tietokoneen on täytettävä seuraavat edellytykset:

   - Käytössäsi on uusin versio Azure AD muodosta.

   - Azure AD yhdistää kaikki tietokoneen haluat hybridi Azure AD liittynyt laitteiden objektit on synkronoitu. Jos tietokoneen objektit kuuluvat tietyn organisaation yksiköt (OU), varmista, että nämä organisaatioyksiköiden määritetään synkronoitaviksi Azure AD muodostaa myös.
    
3. Aiemmin toimialueeseen liittymistä Windows 10 laitteet hybridi Azure AD Joined ja rekisteröityvän Intune (Microsoft Business-365) hallinnoinnin kannettavan laitteen rekisteröiminen:
    
4. Vaihe vaiheelta ohjeiden mukaisesti- [hybridi Azure liitetty Active Directory-laitteiden määrittämisestä](https://go.microsoft.com/fwlink/p/?linkid=872870). Tämä mahdollistaa paikallisen Active Directory synkronointi liittynyt Windows 10-tietokoneisiin ja ne cloud valmis.
    
5. Jotta voit rekisteröidä Windows 10-laitteen kannettavan laitteen hallintaan, katso ohjeet [Windows 10 Intune ryhmäkäytännön avulla laitteen rekisteröiminen](https://go.microsoft.com/fwlink/p/?linkid=872871) . Voit määrittää ryhmäkäytännön paikallisen tietokoneen ääressä tasolla tai voit luoda joukkotoiminnot-palvelimen toimialueen ohjauskoneen tämän ryhmäkäytännön asetus.