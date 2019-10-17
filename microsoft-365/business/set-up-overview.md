---
title: Yleiskatsaus määrittämisestä
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Yleiskatsaus Microsoft 365 Businessin asetus vaiheista.
ms.openlocfilehash: 50f172c235aa06aa78fec60fc119ac7f568df308
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575584"
---
# <a name="overview-of-setup"></a>Yleiskatsaus asennuksesta

Suurin osa määritys vaiheista voidaan tehdä ohjatussa asennus toiminnossa, mutta muut vaihto ehdot luetellaan myös.


## <a name="step-1-add-your-domain-and-users"></a>Vaihe 1: Lisää verkko tunnuksesi ja käyttäjät

   - **[Lisää verkko tunnuksesi](set-up.md#add-your-domain-to-personalize-sign-in)** (jos ostit verkko tunnuksesi [rekisteröitymistä](sign-up.md)varten, tämä vaihe on jo tehty.)

    - **Lisää käyttäjiä**. Voit tehdä tämän jollakin kolmella tavalla:
        - [Ohjatussa toiminnossa](set-up.md#add-users-in-the-wizard).
        - Käytä hakemiston synkronointia [lisätäksesi käyttäjiä Azure AD Connectin avulla](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) , jos sinulla on paikallinen Active Directory.
        - Voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallinta keskukseen.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Vaihe 2: suojaus käytäntöjen määrittäminen ja laitteiden määrittäminen 

  - Määritä laite-ja suojaus käytännöt [ohjatun asennus toiminnon](set-up.md#protect-data-and-devices) avulla. 
  - Voit myös lisätä tai muokata niitä myöhemmin [hallinta keskuksessa](view-policies-and-devices.md) ja [Intune-portaalissa](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Ohjatun asennus toiminnon suojaus asetusten lisäksi voit lisätä suojausta lisäämällä seuraavat asetukset:

      - **Sähkö postin haitta ohjelmien torjunta**
      - **Kehittyneet uhkien torjunta (ATP) turvalliset linkit**
      - **ATP turvalliset liitteet**
      - **ATP anti-phishing**
      - **Exchange Online Archiving**
      - **Tietojen menetyksen estäminen (DLP)**
      - **Azure-tietojen suojaus (Plan1**)

          Jos haluat aloittaa, Katso, [Määritä suoja uksen lisä käytännöt](set-up-advanced-security.md).

        Katso myös [Top 10-tapoja suojata Microsoft 365-liike toiminnan](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) etenemis suunnitelma parhaista tieto turva käytännöistä.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Vaihe 3: Windows 10-laitteiden määrittäminen ja hallinta

   Kun liityt Windows 10-laitteeseen Azure ADIIN, [vaiheessa 2](#step-2-set-up-security-policies-and-configure-devices) käyttöön asettamat käytännöt kohdistetaan siihen.

   - Windows 10 Pro on Microsoft 365 [Businessin edellytys](pre-requisites-for-data-protection.md) , mutta jos sinulla on Windows 7 Pro, Windows 8 Pro tai Windows 8,1 Pro, tilauksesi oikeuttaa sinut [päivittämään Windows 10 Pro-versioon](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
    - Määritä Windows 10-laitteiden käytännöt [ohjatun asennus toiminnon](set-up.md#protect-data-and-devices) avulla.

## <a name="stes-4-install-office-365-business"></a>STES 4: Asenna Office 365 Business
- Voit asentaa Officen automaattisesti Windows-laitteisiin [ohjatun asennus toiminnon](set-up.md#deploy-office-365-client-apps)avulla.
- [Asenna Office](auto-install-or-uninstall-office.md) automaattisesti hallinta keskuksesta.
- Anna käyttäjien [asentaa Office-sovelluksia](https://docs.microsoft.com/office365/admin/setup/install-applications) Windowsille ja laitteille.
     
## <a name="advanced"></a>Kehittynyt
- **Uusien laitteiden määrittäminen automaatti ohjauksen avulla**
            
     [Windows auto pilotin](add-autopilot-devices-and-profile.md) avulla voit määrittää käyttäjälle automaattisesti **uusia** Windows 10-laitteita, mutta [kumppanin](https://www.microsoft.com/solution-providers/search) , joka voi tehdä tämän puolestasi, on ehkä helpompi hankkia se. Voit myös siirtyä [Microsoft Storeen](https://go.microsoft.com/fwlink/?linkid=874598) ja pyytää pilvi teknologian asiantuntijaa hankkimaan sinulle uusia laitteita.

- **Paikallisten resurssien käyttö**

     - Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Businessin suojaamaan Windows 10-laitteitasi samalla, kun ylläpidämme paikallisen todennuksen edellyttävien paikallisten resurssien käyttö oikeuksia. Määritä Microsoft 365 Business, jotta voit määrittää tämän noudattamalla [toimi alueeseen liittyneiden Windows 10-laitteiden käyttöönotto](manage-windows-devices.md) ohjeita. Tämä on ensisijainen menetelmä ja laitteet tässä tilassa kutsutaan hybridi Azure AD liitetyt laitteet.

    - Jos yrityksessasi on paikallinen Active Directory, joka sisältää joitakin paikallisia resursseja (kuten tiedosto resursseja ja tulostimia), voit antaa Azure AD-liitettyjen laitteiden käyttää näitä resursseja noudattamalla seuraavia ohjeita: [paikallisten resurssien käyttö Azure AD-liitetty laite Microsoft 365 Business](access-resources.md).

  