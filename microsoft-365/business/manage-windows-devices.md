---
title: Toimialueen käyttöön liitettyjen Windows 10 -laitteiden hallinta Microsoft 365 for Businessissa
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Lue, miten voit ottaa Microsoft 365:n käyttöön paikallisten Active Directoryyn liitettyjen Windows 10 -laitteiden suojaamisessa muutamassa vaiheessa.
ms.openlocfilehash: 2eaf5aa76cae1680b93af008af615ae872e4fb20
ms.sourcegitcommit: fab425ea4580d1924fb421e6db233d135f5b7d19
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/31/2020
ms.locfileid: "46533781"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Toimialueen käyttöön liitettyjen Windows 10 -laitteiden hallinta Microsoft 365 Business Premiumilla

Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Business Premiumin suojaamaan Windows 10 -laitteita säilyttäen samalla paikallisen todennuksen edellyttävien paikallisten resurssien käytön.
Voit määrittää tämän suojauksen mukautuksella **Hybrid Azure AD -liitettyjä laitteita**. Nämä laitteet on liitetty sekä paikalliseen Active Directoryyn että Azure Active Directoryyn.

Tässä videossa kuvataan, miten tämä määritetään yleisin skenaario, joka on myös kuvattu vaiheet, joita seurataan.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Ennen kuin aloitat, varmista, että olet suorittanut seuraavat toimet:
- Synkronoi käyttäjät Azure AD:hen Azure AD Connectin avulla.
- Suorita Azure AD Connect Organizational Unit (OU) -synkronointi loppuun.
- Varmista, että kaikilla synkronoiduilla toimialueen käyttäjillä on käyttöoikeudet Microsoft 365 Business Premiumiin.

Vaiheet ovat [ohjeaiheessa Toimialueen käyttäjien synkronoiminen Microsoftiin.](manage-domain-users.md)

## <a name="1-verify-mdm-authority-in-intune"></a>1. Tarkista MDM-viranomainen Intuessa

Siirry portal.azure.com ja sivun yläreunassa etsi Intune.
Valitse Microsoft Intune -sivulla **Laiterekisteröinti** ja varmista **Yleiskatsaus-sivulla,** että **MDM-myöntäjä** on **Intune**.

- Jos **MDM-viranomainen** **ei ole Ei mitään**, määritä **MDM-myöntäjäksi** **Intune**.
- Jos **MDM-myöntäjä** on **Microsoft Office 365**, siirry **Devices**  >  **Laitteet-rekisteröintilaitteisiin** ja lisää **Intune MDM** -myöntäjä lisää **MDM-myöntäjän lisääminen** -valintaikkunassa **(Lisää MDM-myöntäjä** -valintaikkuna on käytettävissä vain, jos **MDM-myöntäjäksi** on määritetty Microsoft Office 365).

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Varmista, että Azure AD on otettu käyttöön tietokoneiden liittämistä varten

- Siirry hallintakeskukseen kohdassa <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ja valitse **Hallintakeskukset-luettelosta Azure Active Directory** (valitse Näytä kaikki, jos Azure Active Directory ei ole näkyvissä). **Admin centers** 
- Siirry **Azure Active Directory -hallintakeskuksessa** **Azure Active Directoryyn** , valitse **Laitteet** ja sitten **Laiteasetukset**.
- Tarkista, että**käyttäjät voivat liittyä laitteisiin Azure AD:ssä** on käytössä 
    1. Jos haluat ottaa kaikki käyttäjät käyttöön, määritä **Kaikki**.
    2. Jos haluat ottaa tietyt käyttäjät käyttöön, ota tietty käyttäjäryhmä käyttöön määrittämällä **Valittu.**
        - Lisää Azure AD:ssä synkronoidut toimialueen käyttäjät [suojausryhmään](../admin/create-groups/create-groups.md).
        - Ota MDM-käyttäjäalue käyttöön kyseisessä suojausryhmässä valitsemalla **Valitse ryhmät.**

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Varmista, että Azure AD on otettu käyttöön MDM:ssä

- Siirry hallintakeskukseen ja <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> valitse **päätepisteen hallinta**t (valitse Näytä **kaikki,** jos **Päätepisteen hallinta** ei ole näkyvissä)
- Siirry **Microsoft Endpoint Manager -hallintakeskuksessa** **kohtaan Laitteet**  >  **Windows**  >  **Windowsin rekisteröityminen**  >  **automaattisesti**.
- Varmista, että MDM-käyttäjän vaikutusalue on käytössä.

    1. Jos haluat rekisteröidä kaikki tietokoneet, määritä **Kaikki** rekisteröimään automaattisesti kaikki käyttäjätietokoneet, jotka on liitetty Azure AD:hen ja uusiin tietokoneisiin, kun käyttäjät lisäävät työtilin Windowsiin.
    2. Määritä **Joidenkin-asetukseksi,** jos haluat rekisteröidä tietyn käyttäjäryhmän tietokoneet.
        -  Lisää Azure AD:ssä synkronoidut toimialueen käyttäjät [suojausryhmään](../admin/create-groups/create-groups.md).
        -  Ota MDM-käyttäjäalue käyttöön kyseisessä suojausryhmässä valitsemalla **Valitse ryhmät.**

## <a name="4-create-the-required-resources"></a>4. Tarvittavien resurssien luominen 

Tarvittavien tehtävien suorittamista [Azure AD -yhdistelmän määrittämiseksi](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) on yksinkertaistettu [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) [PowerShell-moduulissa olevan Initialize-SecMgmtHybirdDeviceEnrollment-cmdlet-otoksen](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) avulla. Kun käynnistät tämän cmdlet-liitännän, se luo ja määrittää tarvittavan palveluyhteyspisteen ja ryhmäkäytännön.

Voit asentaa tämän moduulin vetoamalla PowerShellin esiintymään seuraaviin nätin:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> On suositeltavaa asentaa tämä moduuli Windows Serveriin, jossa on Azure AD Connect.

Voit luoda tarvittavan palveluyhteyspisteen ja ryhmäkäytännön käynnistämalla [Initialize-SecMgmtHybirdDeviceEnrollment-cmdlet-liitännän.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Tarvitset Microsoft 365 Business Premiumin yleiset järjestelmänvalvojan tunnistetiedot tätä tehtävää suoritettaessa. Kun olet valmis luomaan resurssit, käynnistä seuraavat toimet:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

Ensimmäinen komento muodostaa yhteyden Microsoftin pilveen, ja kun sinua kehotetaan, määritä Microsoft 365 Business Premiumin yleiset järjestelmänvalvojan tunnistetiedot.

## <a name="5-link-the-group-policy"></a>5. Linkitä ryhmäkäytäntö

1. Napsauta ryhmäkäytäntöjen hallintakonsolissa (GPMC) hiiren kakkospainikkeella sijaintia, johon haluat linkittää käytännön, ja valitse pikavalikosta *Linkitä aiemmin luotu ryhmäkäytäntöobjekti...*
2. Valitse yllä olevassa vaiheessa luotu käytäntö ja valitse sitten **OK**.

## <a name="get-the-latest-administrative-templates"></a>Hanki uusimmat hallintamallit

Jos käytäntö **Ota automaattinen MDM-rekisteröinti käyttöön Azure AD -oletustunnistetietojen avulla**ei ole näkyvissä , syy siihen, että ADMX:ää ei ole asennettu Windows 10:lle, versiolle 1803, versiolle 1809 tai versiolle 1903. Voit korjata ongelman seuraavasti (Huomautus: uusin MDM.admx on taaksepäin yhteensopiva):

1.  Download: [Windows 10:n toukokuun 2019 päivitys (1903) hallintamallit (.admx).](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all)
2.  Asenna paketti ensisijaiseen toimialueen ohjauskoneeseen (PDC).
3.  Siirry kansion version mukaan: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.
4.  Nimeä **käytäntömääritykset** -kansio uudelleen edellä mainitussa **PolicyDefinitions-polun polussa.**
5.  Kopioi **PolicyDefinitions-kansio** **kansioon C:\Windows\SYSVOL\domain\Policies**. 
    -   Jos aiot käyttää koko toimialueen keskitettyä käytäntösäilöä, lisää siihen PolicyDefinitions-sisältö.
6.  Käynnistä ensisijainen toimialueen ohjauskone uudelleen, jotta käytäntö on käytettävissä. Tämä menettely toimii kaikissa tulevissa versioissa samoin.

Tässä vaiheessa sinun pitäisi pystyä näkemään käytäntö **Ota automaattinen MDM-rekisteröinti käyttöön käyttämällä Azure AD:n oletustunnistetietoja.**
