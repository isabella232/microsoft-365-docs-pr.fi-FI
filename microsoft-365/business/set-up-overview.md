---
title: Määritä yleiskatsaus
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Yleistä Microsoft 365 Business vaiheiden määrittäminen.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086312"
---
# <a name="overview-of-setup"></a>Asennuksen yleiskuvaus

Ohjattu asennus voidaan tehdä suurimman osan vaiheiden määrittäminen, mutta luetellaan myös muita vaihtoehtoja.


## <a name="step-1-add-your-domain-and-users"></a>Vaihe 1: Lisää toimialue ja käyttäjät

   - **[Toimialueen lisääminen](set-up.md#add-your-domain-to-personalize-sign-in)** (Jos olet ostanut toimialueen aikana [rekisteröityä](sign-up.md), tässä vaiheessa on jo tehty.)

    - **Lisää käyttäjät**. Voit tehdä tämän jossakin seuraavista kolmesta tavasta:
        - [Ohjattu toiminto](set-up.md#add-users-in-the-wizard).
        - Käyttää hakemiston synkronointi [Azure AD-yhteyden avulla käyttäjät](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) lisätään paikalliseen Active Directoryyn.
        - Voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) admin Centerissä.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Vaihe 2: Määritä suojauskäytännöt ja määrittää laitteiden asetuksia 

  - [Ohjatun asennuksen](set-up.md#set-up-security-policies-and-device-configurations) avulla voit määrittää laitteen ja suojauskäytännöt. 
  - Voit lisätä tai muokata niitä myöhemmin [hallintakeskukseen](view-policies-and-devices.md) ja [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Lisäksi suojausasetukset ohjatun asennuksen voit suurentaa tietoturvan lisäämällä seuraavat asetukset:

      - **Sähköposti Suojaus haittaohjelmilta**
      - **Kokeneet Threat Protection (ATP) turvallinen linkit**
      - **ATP-Safe-liitteet**
      - **ATP anti-phishing**
      - **Exchange Online Archiving**
      - **Tietojen menetyksen estäminen (DLP)**
      - **Azure tietojen suojaus (Plan1**)

          Aloita ks- [käytäntöjen suojauksen lisäasetusten määrittäminen](set-up-advanced-security.md).

        Katso myös suojauksen parhaiden käytäntöjen opas [top 10 tapoja suojata yrityksen Microsoft 365](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) .

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Vaihe 3: Määritä ja Hallitse Windows 10-laitteet

   Kun liität laitteen Windows 10 Azure AD, [Vaihe 2](#step-2-set-up-security-policies-and-configure-devices) Määritä käytäntöjä saada käyttöön sitä.

   - Windows 10 Pro on [ennen sähköntoimitustarjoukset, joihin sisältyivät](pre-requisites-for-data-protection.md) Microsoft 365 Business, mutta jos sinulla on Windows 7 Pro, Windows 8 Pro tai Pro Windows 8.1, tilauksesi oikeuttaa asiakkaan [päivitettävä Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
    - Käytännöt Windows 10-laitteiden [ohjatun asennustoiminnon](set-up.md#set-up-security-policies-and-device-configurations) avulla.

## <a name="stes-4-install-office-365-business"></a>Stes 4: Asenna Office 365: n liiketoiminnan
- Voit asentaa Officen Windows-laitteet automaattisesti [ohjatun asennustoiminnon](set-up.md#deploy-office-365-client-apps)avulla.
- Automaattisesti [asentaa Officen](auto-install-or-uninstall-office.md) hallintakeskukseen.
- Antaa käyttäjien [asentaa Office-sovellukset](https://docs.microsoft.com/office365/admin/setup/install-applications) ja laitteet.
     
## <a name="advanced"></a>Lisäasetukset
- **Automaattiohjauksen avulla voit määrittää uusia laitteita**
            
     [Windows automaattiohjauksen](add-autopilot-devices-and-profile.md) avulla voit määrittää käyttäjän **Uusi** Windows 10-laitteet automaattisesti ennalta, mutta voi olla helpompi saada [kumppani](https://www.microsoft.com/solution-providers/search) , jolla voit tehdä tämän sinulle. Voit myös siirtyä [Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) ja pyytää asiantuntija pilvi tekniikka määrittää, ostaa uusia laitteita.

- **Käyttää tiloissa resursseja**

     - Jos organisaatiossa käytetään Windows Server Active Directory tiloissa, voit määrittää Microsoft 365 liiketoiminnan suojaamaan Windows 10-laitteet, säilyttäen kuitenkin edellyttää paikallista todennusta tiloissa resurssien käytön. Voit määrittää [toimialueeseen liittymistä Windows 10 laitteita voi hallita Microsoft 365 Business käyttöön](manage-windows-devices.md) noudattamalla. Tämä on ensisijainen menetelmä, ja tässä tilassa laitteita kutsutaan hybridi Azure AD liitetyt laitteet.

    - Jos yrityksesi on paikallista Active Directory, joka sisältää joitakin tiloissa (kuten jaettujen tiedostoresurssien ja tulostinten), voit antaa Azure AD liittynyt laitteiden käyttöä noudattamalla tässä nämä resurssit: [käyttö paikalliset resurssit Microsoft 365 Business AD liitetty laite Azure](access-resources.md).

  