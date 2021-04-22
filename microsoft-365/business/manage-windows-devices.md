---
title: Toimialueeseen liitettyjen Windows 10 -laitteiden hallinnoiminen Microsoft 365 for Businessissa
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
description: Voit ottaa Microsoft 365:n käyttöön ja suojata paikalliset Active Directoryyn yhdistetyt Windows 10 -laitteet seuraavasti.
ms.openlocfilehash: c9f5a21d993200abcf9ecf1fa236879245e1c153
ms.sourcegitcommit: 4076b43a4b661de029f6307ddc1a989ab3108edb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2021
ms.locfileid: "51939498"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Ota toimialueeseen liitettyjen Windows 10 -laitteiden hallinta Microsoft 365 Business Premiumin avulla

Jos organisaatiossasi on käytössä Paikallinen Windows Server Active Directory, voit määrittää Microsoft 365 Business Premiumin suojaamaan Windows 10 -laitteitasi säilyttäen edelleen paikallisen todentamisen edellyttävän paikallisen todentamisen resurssien käyttöoikeuden.
Voit määrittää tämän suojauksen laitteella, jossa Azure **AD-yhdistelmäympäristö on liitetty.** Nämä laitteet liitetään sekä paikalliseen Active Directoryyn että Azure Active Directoryyn.

Tässä videossa kuvataan ohjeet sen käyttöön yleisimpään tilanteeseen, joka on myös kuvattu seuraavissa vaiheissa.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Varmista ennen aloittamista, että olet suorittanut seuraavat vaiheet:
- Synkronoi käyttäjät Azure AD:n kanssa Azure AD Connectin avulla.
- Viimeistele Azure AD Connectin organisaatioyksikön (OU) synkronointi.
- Varmista, että kaikilla synkronoiduilla toimialuekäyttäjillä on Microsoft 365 Business Premiumin käyttöoikeudet.

Katso [ohjeet toimialuekäyttäjien synkronoiminen Microsoftiin.](manage-domain-users.md)

## <a name="1-verify-mdm-authority-in-intune"></a>1. MDM-myöntäjän tarkistaminen Intunessa

Siirry [Endpoint Manageriin](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) ja valitse Microsoft Intune -sivulla Laitteen  rekisteröinti **.** Varmista sitten Yleiskatsaus-sivulla, että **MDM-myöntäjä** on **Intune.**

- Jos **MDM-myöntäjä** **on Ei** mitään , määritä **MDM-myöntäjäksi** **Intune.**
- Jos **MDM-myöntäjä** on Microsoft Office  **365,** siirry laitteet Ilmoittavat laitteet -välilehteen ja lisää Intune MDM -myöntäjä oikealla olevan Lisää mobiililaitteiden hallinta -myöntäjä -valintaikkunan avulla (Lisää MDM-myöntäjä -valintaikkuna on käytettävissä vain, jos  >   **MDM-myöntäjäksi** on määritetty Microsoft Office 365).   

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Varmista, että Azure AD on otettu käyttöön tietokoneisiin liittymistä varten

- Siirry hallintakeskukseen kohteessa ja valitse <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Azure Active Directory** (valitse Näytä kaikki, jos Azure Active Directory ei ole näkyvissä) **Hallintakeskukset-luettelossa.** 
- Siirry **Azure Active Directory -hallintakeskuksessa** **Azure Active Directoryyn,** valitse **Laitteet** ja valitse sitten **Laiteasetukset**.
- Varmista,**että käyttäjät voivat liittyä laitteisiin Azure AD:ssä** on otettu käyttöön 
    1. Ota kaikki käyttäjät käyttöön asettamalla arvoksi **Kaikki**.
    2. Jos haluat ottaa tietyt käyttäjät käyttöön, valitse **Valittu,** jotta tietty käyttäjäryhmä otetaan käyttöön.
        - Lisää haluamasi Azure AD:ssä synkronoidut toimialuekäyttäjät [käyttöoikeusryhmään.](../admin/create-groups/create-groups.md)
        - Ota **MDM-käyttäjäalue** käyttöön tässä käyttöoikeusryhmässä valitsemalla Valitse ryhmät.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Varmista, että Azure AD on otettu käyttöön MDM:ssä

- Siirry hallintakeskukseen at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  ja valitse **Endpoint Managemen** t (valitse **Näytä kaikki,** jos **Endpoint-hallinta** ei ole näkyvissä)
- Valitse **Microsoft Endpoint Manager -hallintakeskuksessa** Laitteet   >  Windows Windows Enrollment Automatic Enrollment  >  **(Laitteet, Windows-rekisteröinnin**  >  **automaattinen rekisteröinti).**
- Tarkista, että MDM-käyttäjäalue on käytössä.

    1. Jos haluat rekisteröidä kaikki  tietokoneet, määritä Kaikki-asentoon, jos haluat rekisteröidä automaattisesti kaikki käyttäjätietokoneet, jotka on liitetty Azure AD:han ja uusiin tietokoneisiin, kun käyttäjät lisäävät työtilin Windowsiin.
    2. Valitse **Jotkin,** jos haluat rekisteröidä tietyn käyttäjäryhmän tietokoneet.
        -  Lisää haluamasi Azure AD:ssä synkronoidut toimialuekäyttäjät [käyttöoikeusryhmään.](../admin/create-groups/create-groups.md)
        -  Ota **MDM-käyttäjäalue** käyttöön tässä käyttöoikeusryhmässä valitsemalla Valitse ryhmät.

## <a name="4-create-the-required-resources"></a>4. Tarvittavien resurssien luominen 

[Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) -yhdistelmäliitoksen määrittämiseen tarvittavien tehtävien suorittamista on helpottettu [Käyttämällä Initialize-SecMgmtHybirdDeviceEnrollment-cmdlet-komentoa,](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) joka löytyy [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell -moduulista. Kun käynnistät tämän cmdlet-komentoa, se luo ja määrittää vaaditun palveluyhteyspisteen ja ryhmäkäytännön.

Voit asentaa tämän moduulin käyttämällä PowerShellin esiintymää seuraavasti:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> On suositeltavaa asentaa tämä moduuli Windows Serveriin, jossa on Azure AD Connect.

Jos haluat luoda vaaditun palveluyhteyspisteen ja ryhmäkäytännön, käynnistä [Initialize-SecMgmtHybirdDeviceEnrollment-cmdlet-komento.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Tämän tehtävän suorittamiseen tarvitaan yleisen Microsoft 365 Business Premium -järjestelmänvalvojan tunnistetiedot. Kun olet valmis luomaan resurssit, avaa seuraava komento:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

Ensimmäinen komento muodostaa yhteyden Microsoftin pilvipalveluun ja määrittää pyydettäessä Microsoft 365 Business Premiumin yleisen järjestelmänvalvojan tunnistetiedot.

## <a name="5-link-the-group-policy"></a>5. Linkitä ryhmäkäytäntö

1. Napsauta ryhmäkäytäntöjen hallintakonsolissa hiiren kakkospainikkeella sijaintia, johon haluat linkittää käytännön, ja valitse pikavalikosta Linkitä aiemmin luotu *ryhmäkäytäntöobjekti....*
2. Valitse yllä olevassa vaiheessa luotu käytäntö ja valitse sitten **OK**.

## <a name="get-the-latest-administrative-templates"></a>Hanki uusimmat hallintamallit

Jos et näe käytäntöä Enable **automatic MDM enrollment using default Azure AD credentials**( Ota käyttöön automaattinen MDM-rekisteröinti Azure AD:n oletustunnuksilla), tämä voi olla mahdollista, koska ADMX ei ole asennettuna Windows 10:lle, versiolle 1803 tai uudempaan. Voit korjata ongelman seuraavasti (Huomautus: uusin MDM.admx on yhteensopiva aiempien versioiden kanssa):

1.  Lataa: [Windows 10:n hallintamallit (.admx) lokakuuta 2020 -päivitys (20H2).](https://www.microsoft.com/download/102157)
2.  Asenna paketti toimialueen ohjauskoneeseen.
3.  Siirry kansioon hallintamallien version mukaan: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2).**
4.  Nimeä yllä **olevassa** polussa oleva Käytäntömääritykset-kansio uudelleen **policydefinitions-kansioon.**
5.  Kopioi **PolicyDefinitions-kansio** SYSVOL-jakamaan, oletusarvoisesti **sijaintiin C:\Windows\SYSVOL\domain\Policies.** 
    -   Jos aiot käyttää keskitettyä käytäntösäilöä koko toimialueellesi, lisää Siellä PolicyDefinitions -sisältö.
6.  Jos sinulla on useita toimialueen ohjauskomia, odota, että SYSVOL replikoi käytännöt. Tämä toimenpide toimii myös kaikissa tulevissa hallintamallien versioissa.

Tässä vaiheessa sinun pitäisi nähdä käytäntö Enable automatic MDM enrollment using default Azure AD credentials available (Ota käyttöön automaattinen **MDM-rekisteröinti käyttäen oletusarvoista Azure AD -tunnistetietoja).**

## <a name="related-content"></a>Aiheeseen liittyvä sisältö

[Toimialuekäyttäjien synkronoiminen Microsoft 365:lle](manage-domain-users.md) (artikkeli) Ryhmän luominen [hallintakeskuksessa](../admin/create-groups/create-groups.md) (artikkeli) Opetusohjelma: Azure Active Directory -yhdistelmäliitoksen määrittäminen [hallittuja](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) toimialueita varten (artikkeli)