---
title: Asennuksen yleiskatsaus
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
description: Tutustu Microsoft 365 Business Premiumin määritysvaiheisiin, kuten tilaamiseen, toimialueen ja käyttäjien lisäämiseen, suojauskäytäntöjen määrittämiseen ja paljon muuta.
ms.openlocfilehash: 749acbfdbde92ad97b09dc720c85dd850b76c9cf
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579930"
---
# <a name="overview-of-setup"></a>Asennuksen yleiskatsaus

Katso lyhyt video Microsoft 365 Business Premiumin määrityksestä.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Jos tämä video on mielestäsi hyödyllinen, tutustu [täydelliseen koulutussarjaan pienyrityksille ja uusille Microsoft 365 -käyttäjille](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

Useimmat määritysvaiheet voidaan tehdä ohjatussa määrityksessä, mutta myös muut vaihtoehdot on lueteltu.

## <a name="step-1-add-your-domain-and-users"></a>Vaihe 1: Toimialueen ja käyttäjien lisääminen

   - **[Lisää toimialue](set-up.md#add-your-domain-to-personalize-sign-in)** (jos ostit toimialueen rekisteröitymisen [aikana,](sign-up.md)tämä vaihe on jo valmis.)

   - **Lisää käyttäjiä.** Voit lisätä käyttäjiä kolmella tavalla:
        - Ohjatussa [määrityksessä.](set-up.md#add-users-in-the-wizard)
        - Hakemistosynkronoinnin [avulla voit lisätä käyttäjiä Azure AD Connectin](../enterprise/set-up-directory-synchronization.md) avulla, jos käytössäsi on paikallinen Active Directory.
        - Voit myös [lisätä käyttäjiä myöhemmin](../admin/add-users/add-users.md) hallintakeskuksessa.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Vaihe 2: Suojauskäytäntöjen määrittäminen ja laitteiden määrittäminen 

  - Määritä [laitekäytännöt ohjatun](set-up.md#protect-your-organization) asennuksen avulla. 
  - Voit myös lisätä tai muokata niitä myöhemmin [hallintakeskuksessa ja](view-policies-and-devices.md) [Intune-portaalissa.](/intune/tutorial-walkthrough-intune-portal)
  - Ohjattu määritystoiminto määrittää myös uhkien ja tietojen menetyksen estämisen perusasetukset.
  
  Ohjatun määritystoiminnon suojausasetusten lisäksi voit parantaa suojausta lisäämällä seuraavat asetukset:

- **Sähköpostin haittaohjelmasuojaus**
- **Tietojen kalastelun esto Office 365:n Defenderissä**
- **Exchange Online Archiving**
- **Azure Information Protection (Plan1)**

Aloita tutustumaan [uhkien suojauksen lisäämis-](increase-threat-protection.md) [ja yhteensopivuusominaisuuksien ominaisuuksiin.](set-up-compliance.md)

Katso myös [10 parasta tapaa suojata Microsoft 365 Business Premium](/office365/admin/security-and-compliance/secure-your-business-data) parhaat suojauskäytännöt.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Vaihe 3: Windows 10 -laitteiden määritäminen ja hallinta

Kun olet suorittanut ohjatun määrityksen, haluat suojata kaikki organisaatiosi Windows 10 -tietokoneet.
  
- Windows 10 Pro [](pre-requisites-for-data-protection.md) on Microsoft 365 Business Premiumin edellytys, mutta jos sinulla on Windows 7 Pro, Windows 8 Pro tai Windows 8.1 Pro, tilauksesi oikeuttaa sinut päivittämään [Windows 10 Pro -versioon.](./upgrade-to-windows-pro-creators-update.md)
- Määritä Windows [10 -laitteiden käytännöt](secure-win-10-pcs.md) noudattamalla suojattujen Windows 10 -tietokoneiden ohjeita.

Kun liityt Windows 10 -laitteeseen Azure AD:ssä, Windows 10 -tietokoneille määritettyjä käytäntöjä sovelletaan siihen. Lisätietoja on kohdassa [Windows-laitteiden asennus Microsoft 365 -käyttäjille.](set-up-windows-devices.md)

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Vaihe 4: Microsoft 365 -sovellusten asentaminen yrityksille
- Voit asentaa Officen automaattisesti Windows-laitteisiin [ohjatun määritystoiminnon avulla.](set-up.md#deploy-office-365-client-apps)
- Anna käyttäjien [asentaa Office-sovelluksia](/office365/admin/setup/install-applications) Windowsille ja laitteille.
     
## <a name="advanced"></a>Tarkennettu
- **Uusien laitteiden määritäminen Autopilotilla**
            
     Voit käyttää [Windows Autopilotia](add-autopilot-devices-and-profile.md) uusien **Windows** 10 -laitteiden automaattiseen esimääritykseen käyttäjälle, mutta voi olla helpompaa saada kumppani, joka voi tehdä tämän. [](https://www.microsoft.com/solution-providers/search) Voit myös mennä [Microsoft Storeen](https://go.microsoft.com/fwlink/?linkid=874598)ja pyytää pilvitekniikan asiantuntijaa asettamaan ostamiesi uusien laitteiden ylle.

- **Käytä paikallisia resursseja**

     - Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Business Premiumin suojaamaan Windows 10 -laitteitasi säilyttäen edelleen paikallisen todentamisen edellyttävän paikallisen todentamisen resurssien käyttöoikeuden. Määritä tämä asetus noudattamalla ohjeita, jotka on annettu microsoft [365 Business Premiumin](manage-windows-devices.md) hallitsemaan toimialueisiin liitettyjen Windows 10 -laitteiden käyttöönotto. Tämä on ensisijainen menetelmä, ja tässä tilassa laitteita kutsutaan Azure AD:n yhdistelmäympäristön laitteisiin.

    - Jos yritykselläsi on paikallinen Active Directory, joka sisältää paikallisia resursseja (kuten jaetut tiedostot ja tulostimet), voit antaa Azure AD:lle liitettyjen laitteiden käyttöoikeudet näihin resursseihin seuraavasti: Käytä paikallisia resursseja Azure AD:llä yhdistetystä laitteesta [Microsoft 365 Business Premiumissa.](access-resources.md)

## <a name="see-also"></a>Tutustu myös seuraaviin ohjeartikkeleihin:

[Microsoft 365 for Business -koulutusvideot](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)