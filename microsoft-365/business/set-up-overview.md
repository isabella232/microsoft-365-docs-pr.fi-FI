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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Tutustu Microsoft 365 Business Premiumin asennusvaiheisiin tilaamisesta toimialueen ja käyttäjien lisäämiseen, suojauskäytäntöjen määrittämiseen ja paljon muuta.
ms.openlocfilehash: a808ae5761c1bc5706966a3f7de95f96f8f7c8c8
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785808"
---
# <a name="overview-of-setup"></a>Asennuksen yleiskatsaus

Katso lyhyt video Microsoft 365 Business Premiumin asennuksesta.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

Useimmat asennusvaiheet voidaan tehdä ohjatussa asennustoiminnossa, mutta myös muut asetukset näkyvät luettelossa.

## <a name="step-1-add-your-domain-and-users"></a>Vaihe 1: Toimialueen ja käyttäjien lisääminen

   - **[Lisää toimialueesi](set-up.md#add-your-domain-to-personalize-sign-in)** (jos ostit verkkotunnuksesi [rekisteröitymisen](sign-up.md)aikana, tämä vaihe on jo tehty.)

   - **Lisää käyttäjiä**. Voit lisätä käyttäjiä jollakin seuraavista tavoista:
        - [Ohjatussa toiminnossa.](set-up.md#add-users-in-the-wizard)
        - Hakemistosynkronoinnin avulla voit [lisätä käyttäjiä Azure AD Connectin avulla,](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) jos sinulla on paikallinen Active-hakemisto.
        - Voit [myös lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallintakeskuksessa.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Vaihe 2: Suojauskäytäntöjen määrittäminen ja laitteiden määrittäminen 

  - Määritä laitekäytännöt [ohjatun asennustoiminnon](set-up.md#protect-your-organization) avulla. 
  - Voit myös lisätä tai muokata niitä myöhemmin [hallintakeskuksessa](view-policies-and-devices.md) ja [Intune-portaalissa](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Ohjattu asennustoiminto määrittää myös uhkien suojauksen perus- ja tietojen menetyksen estoasetukset.
  
  Ohjatun asennustoiminnon suojausasetusten lisäksi voit parantaa suojausta lisäämällä seuraavat asetukset:

- **Sähköposti haittaohjelmien torjunta**
- **ATP-tietojenkalastelun torjunta**
- **Exchange Online Archiving**
- **Azure-tietojen suojaus (plan1)**

Lisätietoja on ohjeaiheessa [Uhkien suojauksen lisääminen](increase-threat-protection.md) ja [yhteensopivuusominaisuuksien määrittäminen](set-up-compliance.md).

Katso myös [kymmenen parasta tapaa suojata Microsoft 365 Business Premium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) parhaiden suojauskäytäntöjen etenemissuunnitelma.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Vaihe 3: Windows 10 -laitteiden määrittäminen ja hallinta

Kun olet suorittanut ohjatun asennustoiminnon, haluat käyttää kaikkia organisaatiosi Windwos 10 -tietokoneita.
  
- Windows 10 Pro on Microsoft 365 Business Premiumin [edellytys,](pre-requisites-for-data-protection.md) mutta jos sinulla on Windows 7 Pro, Windows 8 Pro tai Windows 8.1 Pro, tilauksesi oikeuttaa [päivittämään Windows 10 Pro -versioon.](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)
- Määritä Windows [10 -laitteiden käytännöt noudattamalla suojattujen Windows](secure-win-10-pcs.md) 10 -tietokoneiden ohjeita.

Kun liityt Windows 10 -laitteeseen Azure AD:hen, Windows 10 -tietokoneille määrittämäsi käytännöt otetaan käyttöön. Lisätietoja on ohjeaiheessa [Windows-laitteiden määrittäminen Microsoft 365 -käyttäjille](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Vaihe 4: Asenna Microsoft 365 -sovellukset yrityksille
- Voit asentaa Officen automaattisesti Windows-laitteisiin [ohjatun asennustoiminnon](set-up.md#deploy-office-365-client-apps)avulla.
- Anna käyttäjien [asentaa Office-sovelluksia](https://docs.microsoft.com/office365/admin/setup/install-applications) Windowsille ja laitteille.
     
## <a name="advanced"></a>Kehittynyt
- **Uusien laitteiden määrittäminen automaattiohjauksen avulla**
            
     [Windowsin automaattiohjauksen](add-autopilot-devices-and-profile.md) avulla voit määrittää automaattisesti **uusien** Windows 10 -laitteiden määrittämisen käyttäjälle, mutta voi olla helpompaa saada [kumppani,](https://www.microsoft.com/solution-providers/search) joka voi tehdä tämän puolestasi. Voit myös siirtyä [Microsoft Storeen](https://go.microsoft.com/fwlink/?linkid=874598)ja pyytää pilvitekniikan asiantuntijaa määrittämään uusia laitteita, jotka ostat.

- **Paikallisten resurssien käyttäminen**

     - Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Business Premiumin suojaamaan Windows 10 -laitteita säilyttäen samalla paikallisen todennuksen edellyttävien paikallisten resurssien käytön. Määritä tämä noudattamalla kohdan [Salli toimialueisiin liitettyjen Windows 10 -laitteiden hallintaa .](manage-windows-devices.md) Tämä on ensisijainen menetelmä, ja tämän tilan laitteita kutsutaan Hybrid Azure AD -liitetyiksi laitteeksi.

    - Jos yritykselläsi on paikallinen Active Directory, joka sisältää joitakin paikallisia resursseja (kuten jaettuja tiedostoresursseja ja tulostimia), voit antaa Azure AD -liitetyille laitteillesi näiden resurssien käyttöoikeuden noudattamalla seuraavia ohjeita: [Azure AD-liitetyn laitteen paikallisten resurssien käyttäminen Microsoft 365 Business Premiumissa](access-resources.md).

## <a name="see-also"></a>Tutustu myös seuraaviin ohjeaiheisiin

[Microsoft 365 yritysten koulutus videoita](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
