---
title: Yleistietoja määrityksestä
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
description: Opi ohjeet esimerkiksi Microsoft 365 Business Premium tilaamiseen, toimialueen ja käyttäjien lisäämiseen, suojauskäytäntöjen määrittämiseen ja paljon muuta.
ms.openlocfilehash: 7c09dca354781bf92f6bbecca0f3fb9875fb654515fe35c2f96cc780a894a764
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53803218"
---
# <a name="overview-of-setup"></a>Yleistietoja määrityksestä

Katso lyhyt video Microsoft 365 Business Premium määrityksestä.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](../business-video/index.yml).

Useimmat määritysvaiheet voidaan tehdä ohjatussa määrityksessä, mutta myös muut vaihtoehdot on lueteltu.

## <a name="step-1-add-your-domain-and-users"></a>Vaihe 1: Toimialueen ja käyttäjien lisääminen

   - **[Lisää toimialue](set-up.md#add-your-domain-to-personalize-sign-in)** (jos ostit toimialueen [rekisteröitymisen aikana,](sign-up.md)tämä vaihe on jo valmis.)

   - **Käyttäjien lisääminen**. Voit lisätä käyttäjiä kolmella tavalla:
        - Ohjatussa [määrityksessä](set-up.md#add-users-in-the-wizard).
        - Hakemistosynkronoinnin [avulla voit lisätä käyttäjiä Azure AD Näyttöyhteys,](../enterprise/set-up-directory-synchronization.md) jos käytössäsi on paikallinen Active Directory.
        - Voit myös [lisätä käyttäjiä myöhemmin](../admin/add-users/add-users.md) hallintakeskuksessa.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Vaihe 2: Suojauskäytäntöjen määrittäminen ja laitteiden määrittäminen 

  - Voit määrittää [laitekäytännöt ohjatun](set-up.md#protect-your-organization) asennuksen avulla. 
  - Voit myös lisätä tai muokata niitä myöhemmin [hallintakeskuksessa ja](view-policies-and-devices.md) [Intune-portaalissa.](/intune/tutorial-walkthrough-intune-portal)
  - Ohjattu määritystoiminto määrittää myös uhkien ja tietojen menetyksen estämisen perusasetukset.
  
  Ohjatun määritystoiminnon suojausasetusten lisäksi voit parantaa suojaustasi lisäämällä seuraavat asetukset:

- **Sähköpostin haittaohjelmien torjunta**
- **Defender for Office 365**
- **Exchange Online Archiving**
- **Azure Information Protection (Palvelupaketti1)**

Aloita tutustumaan [uhkien uhkien suojauksen](increase-threat-protection.md) [lisäämis- ja yhteensopivuusominaisuuksien määritettyihin ominaisuuksiin.](set-up-compliance.md)

Katso myös [10 tapaa suojata Microsoft 365 Business Premium,](/office365/admin/security-and-compliance/secure-your-business-data) joissa on parhaat suojauskäytännöt.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Vaihe 3: Laitteiden Windows 10 hallinta

Kun olet suorittanut ohjatun määrityksen, haluat suojata Windows 10 tietokoneita organisaatiossasi.
  
- Windows 10 Pro on edellytys [](pre-requisites-for-data-protection.md) Microsoft 365 Business Premium:lle, mutta jos sinulla on Windows 7 Pro, Windows 8 Pro tai Windows 8.1 Pro, tilauksesi oikeuttaa sinut päivittämään [Windows 10 Pro.](./upgrade-to-windows-pro-creators-update.md)
- Määritä käytännöt [mobiililaitteille Windows 10](secure-win-10-pcs.md) tietokoneissa noudattamalla Windows 10 ohjeita.

Kun liityt Windows 10 Azure AD:iin, Windows 10-tietokoneillesi määrittäjät käytännöt otetaan käyttöön. Lisätietoja on kohdassa Laitteiden [Windows Microsoft 365 käyttäjille.](set-up-windows-devices.md)

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Vaihe 4: Microsoft 365 -sovellukset yrityksille
- Voit asentaa Office automaattisesti Windows -laitteisiin ohjatun [määritystoiminnon avulla.](set-up.md#deploy-office-365-client-apps)
- Anna käyttäjien [asentaa Office sovelluksia](/office365/admin/setup/install-applications) Windows ja laitteisiin.
     
## <a name="advanced"></a>Tarkennettu
- **Uusien laitteiden määritäminen Autopilotin avulla**
            
     Voit käyttää [Windows Autopilotia](add-autopilot-devices-and-profile.md) uusien **Windows 10** esimääritykseen automaattisesti käyttäjälle, mutta voi olla helpompaa saada [](https://www.microsoft.com/solution-providers/search) kumppani, joka voi tehdä tämän. Voit myös Microsoft Store [](https://go.microsoft.com/fwlink/?linkid=874598)-sovellukselle ja pyytää pilvitekniikan asiantuntijaa asettamaan uudet laitteet, jotka ostat.

- **Käytä paikallisia resursseja**

     - Jos organisaatiosi käyttää Windows Server Active Directorya paikallisesti, voit määrittää Microsoft 365 Business Premium:n suojaamaan Windows 10-laitteitasi säilyttäen edelleen paikallisen todentamisen edellyttävän paikallisen todentamisen resurssien käyttöoikeuden. Määritä tämä noudattamalla [ohjeita, jotka Windows 10 toimialueisiin](manage-windows-devices.md) liitettyjen laitteiden Microsoft 365 Business Premium hallitaan. Tämä on ensisijainen menetelmä, ja tässä tilassa oleetut laitteet ovat Azure AD:n yhdistelmälaitteisiin liitettyjä laitteita.

    - Jos yritykselläsi on paikallinen Active Directory, joka sisältää paikallisia resursseja (kuten jaetut tiedostoresurssit ja tulostimet), voit antaa Azure AD:lle liitettyjen laitteiden käyttöoikeudet näihin resursseihin noudattamalla seuraavia ohjeita: Paikallisten resurssien käyttäminen Azure AD:llä yhdistetystä [laitteesta Microsoft 365 Business Premium.](access-resources.md)

## <a name="related-content"></a>Aiheeseen liittyvä sisältö

[Microsoft 365 yrityksille 2010 -koulutusvideoita](../business-video/index.yml) (linkkisivu)