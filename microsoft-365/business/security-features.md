---
title: Microsoft 365 Business Premiumin suojaus- ja yhteensopivuusominaisuudet
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-security-compliance
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Lue tietoja Microsoft 365 Business Premiumin mukana tulevista suojausominaisuuksista, jotka auttavat suojaamaan tietojasi tietokoneissa, puhelimissa ja tableteissa.
ms.openlocfilehash: 839b5481e27591e1762a0d8eb5623f279d6d22dd
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/27/2020
ms.locfileid: "44402710"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Microsoft 365 Business Premiumin suojaus- ja yhteensopivuusominaisuudet

Microsoft 365 Business Premium issa on yksinkertaistettuja suojausominaisuuksia, jotka auttavat suojaamaan tietojasi tietokoneissa, puhelimissa ja tableteissa.
    
## <a name="microsoft-365-admin-center-security-features"></a>Microsoft 365 -hallintakeskuksen suojausominaisuudet

[![Selite, jossa ilmoitetaan, että hallintakeskus muuttuu. Lisätietoja löytyy osoitteesta aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Voit hallita useita Microsoft 365 Business Premium -suojausominaisuuksia hallintakeskuksessa, jolloin voit ottaa nämä ominaisuudet käyttöön tai poistaa ne käytöstä. Hallintakeskuksessa voit tehdä seuraavat toimet:
  
- [Sovellusten hallinta-asetusten määrittäminen Android- tai iOS-laitteille](app-protection-settings-for-android-and-ios.md) . 
    
    Näitä asetuksia ovat tiedostojen poistaminen passiivisesta laitteesta tietyn ajan kuluttua, työtiedostojen salaaminen, edellyttää, että käyttäjät asettavat PIN-koodin ja niin edelleen.
    
- [Määritä windows 10 -laitteiden sovellusten suojausasetukset](protection-settings-for-windows-10-devices.md) . 
    
    Näitä asetuksia voidaan käyttää yrityksen tietoihin sekä yrityksen omistamissa että henkilökohtaisesti omistamissa laitteissa.
    
- [Määritä Windows 10 -laitteiden laitesuojausasetukset](protection-settings-for-windows-10-pcs.md) . 
    
    Voit ottaa [BitLocker-salauksen](https://go.microsoft.com/fwlink/p/?linkid=871405) käyttöön tietojen suojaamiseksi siltä varalta, että laite katoaa tai varastetaan, ja antaa [Windows Exploit Guardille](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) kehittyneen suojauksen kiristysohjelmia vastaan. 
    
- [Yritystietojen poistaminen laitteista](remove-company-data.md)
    
    Voit etäpyyhkiä yrityksen tiedot, jos laite katoaa, varastetaan tai työntekijä poistuu yrityksestäsi.
    
- [Palauta Windows 10 -laitteiden tehdasasetukset](reset-devices-to-factory-settings.md) . 
    
    Voit palauttaa kaikki Windows 10 -laitteet, joissa on käytössä laitteen suojausasetukset.
    
## <a name="additional-security-features"></a>Muut suojaustoiminnot 

Microsoft 365 Business Premiumin lisäominaisuudet ovat käytettävissä, jotta voit suojata yrityksesi verkkouhkilta ja suojata arkaluonteisia tietoja.
  
- **[Office 365:n kehittynyt uhkien torjunta](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)**
    
    Advanced Threat Protection (ATP) auttaa suojaamaan yritystäsi kehittyneiltä tietojenkalastelu- ja kiristysohjehyökkäyksiltä, jotka on suunniteltu vaarantamaan työntekijöiden tai asiakkaiden tiedot. Ominaisuuksia ovat:
    
  - Hienostunut liitetiedostojen skannaus ja AI-käyttöinen analyysi vaarallisten viestien havaitsemiseksi ja hylkäämiseksi.
    
  - Sähköpostin linkkien automaattiset tarkistukset sen arvioimiseksi, ovatko ne osa tietojenkalastelujärjestelmää. Tämä estää sinua käyttämästä vaarallisia verkkosivustoja.

- **[Intunen täydet ominaisuudet Azure-portaalissa](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Azure-portaalin Intune-hallintakeskuksen avulla voit määrittää muita suojausominaisuuksia, kuten MacOS-laitteiden, iPhonen ja Android-laitteiden hallinnan sekä windowsin kehittyneen laitehallinnan, jotka eivät ole käytettävissä Microsoft 365 -hallintakeskuksen kautta.
- **Sama [ehdollinen käyttö](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) kuin Azure AD Premium P1 -palvelupaketti**


    Ehdollinen käyttö voi auttaa suojaamaan organisaatiotakirjautumisriskeiltä, käyttämään yrityksiä odottamattomasta verkosta tai maa-maasta, käyttämään riskialttiiden laitetyyppien käyttöyrityksiä ja niin edelleen. Ehdollisen käytön käytännöt otetaan käyttöön ensimmäisen todennuksen jälkeen, ja se määrittää ensimmäisen todennustapahtuman signaalien avulla, onko käyttöyritys hyväksyttävä, evättävä vai tarvitaanko enemmän todisteita (kuten toinen tunnistusmuoto).

    Ehdollisen käytön ominaisuudet ovat seuraavat:

    - Käyttäjänimiin, ryhmään ja rooliin perustuva käyttöoikeus
    - [Sovelluksen perusteella käytettävissä](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Pääsy sijainnin perusteella](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  salli pääsy vain luotettavilta IP-alueilta tai tietyistä maista 
    - Vaadi mfa-käyttö
    - [Vanhan todennuksen](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication) käyttävien sovellusten käytön estäminen
    - Vaadi sovellukset tp käyttää [Intune app protection](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Mukautettu todennus, kuten MFA kolmannen osapuolen palveluntarjoajien, esimerkiksi DUO:n, kanssa.
   
    Muita ominaisuuksia:
    - [Azure AD:n itsepalvelusalasanan palautus](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization)
    
## <a name="compliance-features"></a>Yhteensopivuuden ominaisuudet

Microsoft 365 Business Premium -tilauksesi sisältää ominaisuuksia, joiden avulla voit ylläpitää vaatimustenmukaisuus- ja sääntelystandardeja.

- **[Yleiskatsaus tietojen menetyksen estämiskäytäntöihin](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies)** (DLP). 
    
    Voit määrittää DLP:n tunnistamaan automaattisesti arkaluonteiset tiedot, kuten luottokorttien numerot, henkilötunnukset ja niin edelleen, jotta ne eivät jakaisi tahattomasti yrityksesi ulkopuolella.
    
- **[Exchange Online Archiving](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online Archiving -käyttöoikeus mahdollistaa viestien arkistoimisen helposti jatkuvalla tietojen varmuuskopioinnilla. Se tallentaa kaikki käyttäjän sähköpostit, mukaan lukien poistetut kohteet, siltä varalta, että niitä tarvitaan myöhemmin etsintää tai palauttamista varten. Lisäksi voit käyttää eri säilytyskäytäntöjä, kun haluat säilyttää sähköpostitiedot riita-asioiden pitoihin, eDiscoveryen tai vaatimustenmukaisuusvaatimusten täyttämiseen.
    
- **[Luottamuksellisuusmerkinnät](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Microsoft 365 Business Premium sisältää kaikki [Azure Information Protection Plan 1](https://go.microsoft.com/fwlink/p/?linkid=871407):n ominaisuudet. Tämän suunnitelman avulla voit luoda **herkkyysotsikoita,** joiden avulla voit hallita sähköpostin ja asiakirjojen arkaluonteisten tietojen käyttöä, esimerkiksi "Älä välitä" ja Älä kopioi . Voit myös luokitella arkaluonteiset tiedot luottamuksellisiksi ja määrittää, miten turvaluokiteltuja tietoja voidaan jakaa yrityksen ulkopuolella ja sisällä. Yritystason salausta on helppo käyttää sähköpostiin ja asiakirjoihin, jotta tietosi pysyvät yksityisinä. Voit myös asentaa Office-sovellusten Azure Information Protection -asiakasohjelman apuohjelman. Lisätietoja on kohdassa [Azure Information Protectionunified labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). Jos haluat käyttää herkkyystarroja, asenna **AzInfoProtection_UL.exe**.

Voit hallita näitä ominaisuuksia &amp; Tietoturvan yhteensopivuus -keskuksessa ja Intune-hallintakeskuksessa. Ajan myötä yksinkertaistetut ohjausobjektit lisätään Microsoft 365 -hallintakeskukseen.
  
    
## <a name="faq"></a>Usein kysytyt kysymykset

 ### <a name="are-these-security-features-available-in-all-markets"></a>Ovatko nämä turvaominaisuudet saatavilla kaikilla markkina-alueilla?
  
Kyllä, nämä ominaisuudet ovat käytettävissä kaikilla markkinoilla, joilla Microsoft 365 Business Premium myydään.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Miten löydän &amp; tietoturvan yhteensopivuuskeskuksen?
  
1. [Kirjaudu Microsoft 365 Business Premiumiin](https://portal.microsoft.com/) järjestelmänvalvojan tunnistetiedoilla. 
    
2. Etsi vasemmasta siirtymisruudusta **Hallintakeskukset** ja laajenna se. 
    
    ![Valitse Microsoft 365 -hallintakeskuksen vasemmasta siirtymisruudusta Hallintakeskukset.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Siirry Suojauksen yhteensopivuus -keskukseen valitsemalla **Suojauksen &amp; yhteensopivuus.** &amp;
