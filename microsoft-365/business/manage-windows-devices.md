---
title: Toimialueen liitettyjen Windows 10 -laitteiden ottaminen käyttöön Microsoft 365 for Businessin hallinnassa
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Opi, miten voit ottaa Microsoft 365:n käyttöön paikallisten Active Directoryyn liitettyjen Windows 10 -laitteiden suojaamisessa muutamalla vaiheella.
ms.openlocfilehash: 8a45c6959bee368491c5c6424e3713300c443779
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580130"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Toimialueen liitettyjen Windows 10 -laitteiden ottaminen käyttöön Microsoft 365 Business Premiumin hallinnassa

Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Business Premiumin suojaamaan Windows 10 -laitteitasi säilyttäen edelleen paikallisen todentamisen edellyttävän paikallisen todentamisen resurssien käyttöoikeuden.
Voit määrittää tämän suojauksen laitteella, joka on liitetty **Azure AD-yhdistelmäympäristön laitteisiin.** Nämä laitteet liitetään sekä paikalliseen Active Directoryyn että Azure Active Directoryyn.

Tässä videossa kerrotaan, miten voit määrittää tämän yleisimpään tilanteeseen, joka on myös kuvattu seuraavissa vaiheissa.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Varmista ennen aloittamista, että olet suorittanut seuraavat vaiheet:
- Synkronoi käyttäjät Azure AD:n kanssa Azure AD Connectin avulla.
- Viimeistele Azure AD Connectin organisaatioyksikön (OU) synkronointi.
- Varmista, että kaikilla synkronoiduilla toimialuekäyttäjillä on Microsoft 365 Business Premiumin käyttöoikeudet.

Katso [ohjeet toimialuekäyttäjien synkronoinnin ohjeesta Microsoftin](manage-domain-users.md) kanssa.

## <a name="1-verify-mdm-authority-in-intune"></a>1. MDM-myöntäjän tarkistaminen Intunessa

Siirry [Endpoint Manageriin](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) ja valitse Microsoft Intune -sivulla Laitteen  rekisteröinti ja varmista Sitten Yleiskatsaus-sivulla, että **MDM-myöntäjä** on **Intune.**

- Jos **MDM-myöntäjä** **on** Ei mitään, määritä sen arvoksi Intune napsauttamalla **MDM-myöntäjää.** 
- Jos **MDM-myöntäjä** on Microsoft Office  **365,** siirry Laitteet-rekisteröintilaitteisiin ja lisää Intune MDM -myöntäjä oikealla olevan Lisää MDM -myöntäjä -valintaikkunan avulla (Lisää MDM-myöntäjä -valintaikkuna on käytettävissä vain, jos  >    **MDM-myöntäjäksi** on määritetty Microsoft Office 365).  

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Tarkista, että Azure AD on otettu käyttöön tietokoneisiin liittymistä varten

- Siirry hallintakeskukseen ja valitse Hallintakeskukset-luettelosta Näytä kaikki, jos Azure Active Directory ei ole <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> näkyvissä.   
- Siirry **Azure Active Directory -hallintakeskuksessa** **Azure Active Directoryyn,** valitse **Laitteet** ja sitten **Laiteasetukset.**
- Varmista,**että käyttäjät voivat liittyä laitteisiin Azure AD:ssä** on otettu käyttöön 
    1. Jos haluat ottaa kaikki käyttäjät käyttöön, määritä arvoksi **Kaikki.**
    2. Jos haluat ottaa tietyt käyttäjät käyttöön, **määritä** se valituiksi, jotta tietty käyttäjäryhmä otetaan käyttöön.
        - Lisää haluamasi Azure AD:ssä synkronoidut toimialuekäyttäjät [käyttöoikeusryhmään.](../admin/create-groups/create-groups.md)
        - Ota **MDM-käyttäjäalue** käyttöön tässä käyttöoikeusryhmässä valitsemalla Valitse ryhmät.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Tarkista, että Azure AD on otettu käyttöön MDM:ssä

- Siirry hallintakeskukseen ja valitse <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Endpoint Managemen** t (Valitse **Näytä** kaikki, jos **Endpoint Manager** ei ole näkyvissä)
- Valitse **Microsoft Endpoint Manager -hallintakeskuksessa** Laitteet,   >  **joissa**  >  **Windows Windows -rekisteröinti on**  >  **automaattinen rekisteröinti.**
- Tarkista, että MDM-käyttäjän laajuus on otettu käyttöön.

    1. Rekisteröi kaikki tietokoneet asettamalla Kaikki-asentoon kaikki käyttäjät, jotka on liitetty Azure AD:han ja uusiin tietokoneisiin, kun käyttäjät lisäävät työtilin Windowsiin. 
    2. Määritä Osa **tietyn** käyttäjäryhmän tietokoneiden rekisteröintiä varten.
        -  Lisää haluamasi Azure AD:ssä synkronoidut toimialuekäyttäjät [käyttöoikeusryhmään.](../admin/create-groups/create-groups.md)
        -  Ota **MDM-käyttäjäalue** käyttöön tässä käyttöoikeusryhmässä valitsemalla Valitse ryhmät.

## <a name="4-create-the-required-resources"></a>4. Tarvittavien resurssien luominen 

[Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) -yhdistelmäliitoksen määrittämiseen tarvittavien tehtävien suorittamista on yksinkertaistettu [Käyttämällä SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell -moduulin [Initialize-SecMgmtHybirdDeviceEnrollment-cmdlet-komentoa.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Kun käynnistät tämän cmdlet-komentoa, se luo ja määrittää tarvittavan palveluyhteyspisteen ja ryhmäkäytännön.

Voit asentaa tämän moduulin käyttämällä Seuraavaa PowerShell-esiintymää:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> On suositeltavaa asentaa tämä moduuli Windows Serveriin, jossa on Käytössä Azure AD Connect.

Jos haluat luoda vaaditun palveluyhteyspisteen ja ryhmäkäytännön, [käynnistä Initialize-SecMgmtHybirdDeviceEnrollment-cmdlet-komento.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Tämän tehtävän suorittamiseen tarvitaan yleisen Microsoft 365 Business Premium -järjestelmänvalvojan tunnistetiedot. Kun olet valmis luomaan resurssit, käynnistä seuraava komento:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

Ensimmäinen komento muodostaa yhteyden Microsoftin pilvipalveluun, ja kun sinua pyydetään, määritä Microsoft 365 Business Premiumin yleisen järjestelmänvalvojan tunnistetiedot.

## <a name="5-link-the-group-policy"></a>5. Linkitä ryhmäkäytäntö

1. Napsauta ryhmäkäytäntöjen hallintakonsolissa hiiren kakkospainikkeella sijaintia, johon haluat linkittää  käytännön, ja valitse pikavalikosta Linkitä aiemmin luotu ryhmäkäytäntöobjekti...
2. Valitse yllä olevassa vaiheessa luotu käytäntö ja valitse **sitten OK.**

## <a name="get-the-latest-administrative-templates"></a>Uusimmat hallintamallit

Jos et näe käytäntöä Ota automaattinen **MDM-rekisteröinti** käyttöön Azure AD:n oletustunnuksilla, tämä voi olla mahdollista, koska ADMX:ää ei ole asennettu Windows 10:tä, versiota 1803 tai uudempaa versiota varten. Voit korjata ongelman seuraavasti (Huomautus: uusin MDM.admx on yhteensopiva aiempien versioiden kanssa):

1.  Lataa: [Windows 10:n hallintamallit (.admx) lokakuun 2020 päivitys (20H2).](https://www.microsoft.com/download/102157)
2.  Asenna paketti toimialueen ohjauskoneeseen.
3.  Siirry kansioon hallintamallien version mukaan: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.
4.  Nimeä yllä **olevassa** polussa oleva Käytäntömääritelmät-kansio uudelleen **PolicyDefinitions-kansioon.**
5.  Kopioi **PolicyDefinitions-kansio** SYSVOL-jakamaan, oletusarvoisesti kansiossa **C:\Windows\SYSVOL\domain\Policies.** 
    -   Jos aiot käyttää keskitettyä käytäntösäilöä koko toimialueellesi, lisää Siellä PolicyDefinitions-sisältö.
6.  Jos sinulla on useita toimialueen ohjauskoneeseeneja, odota, että SYSVOL replikoi käytännöt. Tämä toimenpide toimii myös kaikissa hallintamallien tulevissa versioissa.

Tässä vaiheessa sinun pitäisi nähdä käytäntö Ota käyttöön automaattinen MDM-rekisteröinti käyttämällä **oletusarvoista Azure AD -tunnistetietoja.**