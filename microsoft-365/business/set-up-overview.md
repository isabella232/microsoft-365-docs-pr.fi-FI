---
title: Asennuksen yleiskatsaus
f1.keywords:
- NOCSH
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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Lue Tietoja Microsoft 365 Business Premiumin määritysvaiheista, tilaamisesta, toimialueen ja käyttäjien lisäämisestä, suojauskäytäntöjen määrittämisestä ja muusta.
ms.openlocfilehash: 8b26d423d4f62ee8f9ea4a61eb8f7efa72ee26cb
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43633351"
---
# <a name="overview-of-setup"></a>Asennuksen yleiskatsaus

Katso lyhyt video Microsoft 365 Business Premiumin asennuksesta.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

Useimmat asennusvaiheet voidaan tehdä ohjatussa asennustoiminnossa, mutta myös muut asetukset on lueteltu.

## <a name="step-1-add-your-domain-and-users"></a>Vaihe 1: Toimialueen ja käyttäjien lisääminen

   - **[Lisää toimialue (jos](set-up.md#add-your-domain-to-personalize-sign-in)** ostit verkkotunnuksen [rekisteröityessäsi,](sign-up.md)tämä vaihe on jo tehty.)

    - **Lisää käyttäjiä**. Voit lisätä käyttäjiä millä tahansa seuraavista kolmesta tavasta:
        - [Ohjatussa toiminnossa.](set-up.md#add-users-in-the-wizard)
        - Hakemistosynkronoinnin avulla voit [lisätä käyttäjiä Azure AD Connectin avulla,](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) jos käytössäsi on paikallinen Active-hakemisto.
        - Voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallintakeskukseen.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Vaihe 2: Suojauskäytäntöjen määrittäminen ja laitteiden määrittäminen 

  - Määritä laitekäytännöt [ohjatun asennustoiminnon](set-up.md#protect-your-organization) avulla. 
  - Voit myös lisätä niitä tai muokata niitä myöhemmin [hallintakeskuksessa](view-policies-and-devices.md) ja [Intune-portaalissa.](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)
  - Ohjattu asennustoiminto määrittää myös uhkien suojauksen ja tietojen menetyksen estämisen perusasetukset.
  
  Ohjatun asennustoiminnon suojausasetusten lisäksi voit parantaa suojausta lisäämällä seuraavat asetukset:

- **Sähköposti haittaohjelmien torjunta**
- **ATP anti-phishing**
- **Exchange Online Archiving**
- **Azure-tietojen suojaus (suunnitelma1)**

Lisätietoja on ohjeessa [Uhkien suojauksen lisääminen](increase-threat-protection.md) ja [vaatimustenmukaisuusominaisuuksien määrittäminen](set-up-compliance.md).

Katso myös [kymmenen parasta tapaa suojata Microsoft 365 Business Premium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) ja tutustu parhaisiin tietoturvakäytäntöihin.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Vaihe 3: Windows 10 -laitteiden määrittäminen ja hallinta

Kun olet suorittanut ohjatun määritystoiminnon, haluat proctect kaikki Windwos 10 tietokoneet organisaatiossa.
  
- Windows 10 Pro on Microsoft 365 Business Premiumin [edellytys,](pre-requisites-for-data-protection.md) mutta jos sinulla on Windows 7 Pro, Windows 8 Pro tai Windows 8.1 Pro, tilauksesi oikeuttaa [päivittämään Windows 10 Pro -versioon](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Määritä Windows [10 -laitteiden käytännöt noudattamalla suojattujen Windows 10 -tietokoneiden](secure-win-10-pcs.md) ohjeita.

Kun liityt Windows 10 -laitteeseen Azure AD:hen, Windows 10 -tietokoneille määrittämäsi käytännöt otetaan käyttöön. Lisätietoja on ohjeaiheessa [Windows-laitteiden määrittäminen Microsoft 365 -käyttäjille](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Vaihe 4: Asenna Microsoft 365 Apps for Business
- Voit asentaa Officen automaattisesti Windows-laitteisiin [ohjatun asennustoiminnon](set-up.md#deploy-office-365-client-apps)avulla.
- Anna käyttäjien [asentaa Office-sovelluksia](https://docs.microsoft.com/office365/admin/setup/install-applications) Windowsille ja laitteille.
     
## <a name="advanced"></a>Kehittynyt
- **Uusien laitteiden määrittäminen automaattiohjauksen avulla**
            
     [Windowsin automaattiohjauksen](add-autopilot-devices-and-profile.md) avulla voit määrittää **käyttäjälle** automaattisesti uudet Windows 10 -laitteet, mutta voi olla helpompaa saada [kumppani,](https://www.microsoft.com/solution-providers/search) joka voi tehdä tämän puolestasi. Voit myös siirtyä [Microsoft Storeen](https://go.microsoft.com/fwlink/?linkid=874598)ja pyytää pilvitekniikan asiantuntijaa asettamaan ostamasi uudet laitteet.

- **Paikallisten resurssien käyttäminen**

     - Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Business Premiumin suojaamaan Windows 10 -laitteita ja säilyttämään silti paikallisen todennuksen edellyttävien paikallisten resurssien käytön. Määritä tämä noudattamalla kohdan [Microsoft 365 Business Premiumin hallitsemien toimialueeseen liitettyjen Windows 10 -laitteiden ottaminen käyttöön](manage-windows-devices.md) -kohdan ohjeita. Tämä on ensisijainen menetelmä, ja tämän tilan laitteita kutsutaan Hybrid Azure AD -liitetyiksi laiteiksi.

    - Jos yritykselläsi on paikallinen Active Directory, joka sisältää joitakin paikallisia resursseja (kuten jaettuja tiedostoja ja tulostimia), voit antaa Azure AD:hen liitetyille laitteille näiden resurssien käyttöoikeuden noudattamalla seuraavia ohjeita: [Paikallisten resurssien käyttäminen Azure AD:hen liitetystä laitteesta Microsoft 365 Business Premiumissa](access-resources.md).

## <a name="see-also"></a>Tutustu myös seuraaviin ohjeaiheisiin

[Microsoft 365 yrityksille koulutus videoita](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
