---
title: Yleistä asennuksesta
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
description: Lisä tietoja on artikkelissa Microsoft 365 Business Premiumin määritys ohjeet, tila uksen tilaaminen, toimi alueen ja käyttäjien lisääminen, tieto turva käytäntöjen määrittäminen ja paljon muuta.
ms.openlocfilehash: fa9c02fa9546437c83b9cc6c1f1e6e0d723ec868
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306465"
---
# <a name="overview-of-setup"></a>Yleistä asennuksesta

Katso lyhyt video Microsoft 365 Business Premium-asennuksesta.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

Useimmat määritys vaiheet voidaan tehdä ohjatussa määritys toiminnossa, mutta myös muut asetukset on lueteltu.

## <a name="step-1-add-your-domain-and-users"></a>Vaihe 1: toimi alueen ja käyttäjien lisääminen

   - **[Toimi alueen lisääminen](set-up.md#add-your-domain-to-personalize-sign-in)** (jos olet ostanut toimi alueen rekisteröitymisen [yhteydessä,](sign-up.md)tämä vaihe on jo suoritettu.)

   - **Lisää käyttäjiä**. Voit lisätä käyttäjiä kolmella eri tavalla:
        - [Ohjatussa toiminnossa](set-up.md#add-users-in-the-wizard).
        - Hakemisto synkronoinnin avulla voit [lisätä käyttäjiä Azure AD Connectin avulla](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) , jos käytössäsi on paikallinen Active Directory.
        - Voit myös [lisätä käyttäjiä myöhemmin](add-users-m365b.md) hallinta keskuksessa.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Vaihe 2: Määritä käyttö oikeus käytännöt ja Määritä laitteet 

  - Määritä laite käytännöt [ohjatun määritys toiminnon](set-up.md#protect-your-organization) avulla. 
  - Voit myös lisätä tai muokata niitä myöhemmin [hallinta keskuksessa](view-policies-and-devices.md) ja [Intune-portaalissa](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Ohjattu määritys toiminto määrittää myös uhkien suojaamisen ja tietojen menetyksen estämisen asetukset.
  
  Ohjatun määritys toiminnon turva-asetusten lisäksi voit lisätä suojausta lisäämällä seuraavat asetukset:

- **Sähkö postin haitta ohjelmien torjunta**
- **ATP anti-phishing**
- **Exchange Online Archiving**
- **Azure Information Protectionin (toimintasuunnitelma1**)

Lisä tietoja on Ohje aiheissa [uhkien suojaamisen lisääminen](increase-threat-protection.md) ja [yhteensopivuus ominaisuuksien määrittäminen](set-up-compliance.md).

Katso myös [kymmenen parasta tapaa, joilla voit suojata Microsoft 365 Business Premiumin](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) parhaiden tieto turva käytäntöjen etenemis suunnitelmaksi.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Vaihe 3: Windows 10-laitteiden määrittäminen ja hallinta

Kun olet suorittanut ohjatun määritys toiminnon, haluat proctect kaikki organisaatiosi Windwos 10-tieto koneet.
  
- Windows 10 Pro on Microsoft 365 Business Premiumin [edellytys](pre-requisites-for-data-protection.md) , mutta jos käytössäsi on Windows 7 Pro, Windows 8 Pro tai Windows 8,1 Pro, tilauksesi oikeuttaa [päivittämään Windows 10 Pro-versioon](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Määritä Windows 10-laitteiden käytännöt noudattamalla ohjeita kohdassa [suojatun Windows 10-tieto koneiden](secure-win-10-pcs.md) määrittäminen.

Kun liityt Windows 10-laitteeseen Azure AD:hen, Windows 10-tieto koneille määritetyt käytännöt tulevat käyttöön. Lisä tietoja on Ohje aiheessa [Windows-laitteiden määrittäminen Microsoft 365-käyttäjille](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Vaihe 4: Asenna Microsoft 365-sovellukset yrityksille
- Voit asentaa Officen automaattisesti Windows-laitteisiin [ohjatun määritys toiminnon](set-up.md#deploy-office-365-client-apps)avulla.
- Anna käyttäjien [asentaa Office-sovelluksia](https://docs.microsoft.com/office365/admin/setup/install-applications) Windowsia ja laitteita varten.
     
## <a name="advanced"></a>Lisä
- **Uusien laitteiden määrittäminen Autopilot-toiminnolla**
            
     [Windowsin Autopilot](add-autopilot-devices-and-profile.md) -toiminnon avulla voit määrittää käyttäjän **uudet** Windows 10-laitteet automaattisesti valmiiksi, mutta sinun on ehkä helpompi hankkia [kumppaneita](https://www.microsoft.com/solution-providers/search) , jotka voivat tehdä sen puolestasi. Voit myös siirtyä [Microsoft Storeen](https://go.microsoft.com/fwlink/?linkid=874598)ja pyytää pilvi tekniikan asiantuntijaa määrittämään uusia laitteita, jotka ostat.

- **Paikallisten resurssien käyttäminen**

     - Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Business Premiumin suojaamaan Windows 10-laitteitasi säilyttäen kuitenkin paikalliset resurssit, jotka vaativat paikallisen todennuksen. [Ota Microsoft 365 Business Premium-hallinta käyttöön](manage-windows-devices.md) , jotta voit määrittää tämän, noudattamalla ohjeita kohdassa toimi alueen liittyminen Windows 10-laitteisiin. Tämä on suositeltava menetelmä, ja tämän tilan laitteet ovat nimeltään Hybrid Azure AD-yhdistetyt laitteet.

    - Jos yrityksessä on paikallinen Active Directory-hakemisto, joka sisältää joitakin paikallisia resursseja (kuten jaetut tiedosto resurssit ja tulostimet), voit antaa Azure AD:hen liittyneille laitteillesi oikeuden käyttää näitä resursseja noudattamalla seuraavia ohjeita: paikallisten [resurssien käyttäminen Azure AD-liitetyssä laitteessa Microsoft 365 Business Premiumissa](access-resources.md).

## <a name="see-also"></a>Tutustu myös seuraaviin ohjeartikkeleihin:

[Microsoft 365 for Business-koulutus videot](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
