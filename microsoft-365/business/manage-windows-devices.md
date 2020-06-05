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
ms.openlocfilehash: 857651081fb10856d28dd419333ebef655388407
ms.sourcegitcommit: e6e704cbd9a50fc7db1e6a0cf5d3f8c6cbb94363
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/04/2020
ms.locfileid: "44564933"
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

## <a name="4-set-up-service-connection-point-scp"></a>4. Palveluyhteyspisteen (SCP) määrittäminen

Näitä vaiheita yksinkertaistetaan [hybridi azure AD -liitoksen määrittämisestä.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) Voit suorittaa azure AD Connectin ja Microsoft 365 Business Premiumin yleisen järjestelmänvalvojan ja Active Directory -järjestelmänvalvojan salasanat.

1.  Käynnistä Azure AD Connect ja valitse sitten **Määritä**.
2.  Valitse **Lisätehtävät-sivulla** **Määritä laiteasetukset**ja valitse sitten **Seuraava**.
3.  Valitse **Yleiskatsaus-sivulla** **Seuraava**.
4.  Kirjoita **Yhdistä Azure AD:hen** -sivulla Microsoft 365 Business Premiumin yleisen järjestelmänvalvojan tunnistetiedot.
5.  Valitse **Laiteasetukset-sivulla** **Määritä Azure AD -yhdistelmäliitos**ja valitse sitten **Seuraava**.
6.  Tee seuraavat vaiheet **SCP-sivulla** jokaiselle puuryhmälle, johon haluat Azure AD Connectin määrittävän SCP:n, ja valitse sitten **Seuraava**:
    - Valitse metsän nimen vieressä oleva valintaruutu. Puuryhmän pitäisi olla AD-toimialuenimesi.
    - Avaa **Todennuspalvelu-sarakkeessa** avattava luettelo ja valitse vastaava toimialuenimi (vain yksi vaihtoehto pitäisi olla).
    - Anna toimialueen järjestelmänvalvojan tunnistetiedot valitsemalla **Lisää.**  
7.  Valitse **Laitteen käyttöjärjestelmät -sivulla** vain Windows 10 tai uudempi toimialueeseen liitetyt laitteet.
8.  Valitse **Valmis konfiguroimaan** -sivulla **Määritä**.
9.  Valitse **Kokoonpano valmis** -sivulla **Lopeta**.


## <a name="5-create-a-gpo-for-intune-enrollment--admx-method"></a>5. Luo GPO Intune Ilmoittautuminen - ADMX menetelmä

Käyttää. ADMX-mallitiedosto.

1.  Kirjaudu AD-palvelimeen, etsi ja avaa **Server Manager**  >  **Tools**  >  **-ryhmäkäytäntöjen hallinta**.
2.  Valitse toimialuenimi **Toimialueet-kohdasta** ja valitse **Uusi**napsauttamalla hiiren kakkospainikkeella **Ryhmäkäytäntöobjektit** .
3.  Anna uudelle gpo:lle nimi, esimerkiksi "*Cloud_Enrollment*" ja valitse sitten **OK**.
4.  Napsauta uutta ryhmäkäytäntöobjektia hiiren kakkospainikkeella **ryhmäkäytäntöobjektien** alla ja valitse **Muokkaa**.
5.  Siirry **ryhmäkäytäntöjen hallintaeditorissa** **kohtaan Tietokonemäärityskäytännöt**  >  **Policies**  >  **Hallintamallit**  >  **Windowsin osien**  >  **MDM**.
6. Napsauta hiiren kakkospainikkeella **Ota automaattinen MDM-rekisteröinti käyttöön Azure AD -oletustunnistetietojen avulla** ja valitse sitten **Käytössä**  >  **OK**. Sulje editori-ikkuna.

> [!IMPORTANT]
> Jos **käytäntöä Ota automaattinen MDM-rekisteröinti käyttöön Azure AD -oletustunnistetietojen avulla**ei ole näkyvissä , katso [uusimmat hallintamallit](#get-the-latest-administrative-templates).

## <a name="6-deploy-the-group-policy"></a>6. Ryhmäkäytännön käyttöönotto

1.  Valitse Palvelimen hallinnan **Toimialueet** > ryhmäkäytäntöobjektit -kohdassa ryhmäkäytäntöobjekti yllä olevasta vaiheesta 3, esimerkiksi "Cloud_Enrollment".
2.  Valitse **gpo:n Laajuus-välilehti.**
3.  Napsauta GPO:n Vaikutusalue-välilehden **Linkit**-kohdan toimialueen linkkiä hiiren kakkospainikkeella.
4.  Ota gpo käyttöön valitsemalla **Pakotettu** ja sitten **OK** vahvistusnäytössä.

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

