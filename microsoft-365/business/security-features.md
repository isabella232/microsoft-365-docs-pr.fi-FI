---
title: Microsoft 365 Businessin suojaus- ja yhteensopivuusominaisuudet
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
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Lue tietoja Microsoft 365 Businessin mukana tulevista suojausominaisuuksista, joiden avulla voit suojata tietokoneesi, puhelimesi ja tablettisi tiedot.
ms.openlocfilehash: 85f9b50225c3dbdb0c1b76c33d516aaa03bec773
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561256"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>Microsoft 365 Businessin suojaus- ja yhteensopivuusominaisuudet

Microsoft 365 Business tarjoaa yksinkertaistettuja suojausominaisuuksia, jotka auttavat suojaamaan tietokoneita, puhelimia ja tabletteja koskevia tietoja.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Microsoft 365 Business -hallintakeskuksen suojausominaisuudet

[![Selite, jossa ilmoitetaan, että hallintakeskus muuttuu. Lisätietoja löytyy osoitteesta aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Voit hallita monia Hallintakeskuksen Microsoft 365 Business -suojausominaisuuksia, jolloin voit ottaa nämä ominaisuudet käyttöön tai poistaa ne käytöstä yksinkertaistetulla tavalla. Hallintakeskuksessa voit tehdä seuraavat toimet:
  
- [Määritä sovellusten hallinta-asetukset Android- tai iOS-laitteille](app-protection-settings-for-android-and-ios.md) . 
    
    Näitä asetuksia ovat muun muassa tiedostojen poistaminen passiivisesta laitteesta tietyn ajan kuluttua, työtiedostojen salaaminen, vaaditaan, että käyttäjät asettavat PIN-koodin ja niin edelleen.
    
- [Määritä Windows 10 -laitteiden sovellusten suojausasetukset](protection-settings-for-windows-10-devices.md) . 
    
    Näitä asetuksia voidaan käyttää yrityksen tietoihin sekä yrityksen omistamista että henkilökohtaisesti omistamista laitteista.
    
- [Määritä Windows 10 -laitteiden laitesuojausasetukset](protection-settings-for-windows-10-pcs.md) . 
    
    Voit ottaa [BitLocker-salauksen](https://go.microsoft.com/fwlink/p/?linkid=871405) käyttöön tietojen suojaamiseksi siltä varalta, että laite katoaa tai varastetaan, ja ottaa [Windows Exploit Guardin](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) käyttöön, jotta se voi tarjota kehittyneen suojauksen kiristysohjelmia vastaan. 
    
- [Yritystietojen poistaminen laitteista](remove-company-data.md)
    
    Voit poistaa yrityksen tiedot etänä, jos laite katoaa, varastetaan tai työntekijä poistuu yrityksestäsi.
    
- [Palauta Windows 10 -laitteet tehdasasetuksiinsa](reset-devices-to-factory-settings.md) . 
    
    Voit nollata kaikki Windows 10 -laitteet, joissa on käytössä laitteen suojausasetukset.
    
## <a name="additional-security-features"></a>Muut suojaustoiminnot 

Microsoft 365 Businessin lisäominaisuudet auttavat suojaamaan yritystäsi kyberuhkilta ja suojaamaan arkaluonteisia tietoja.
  
- **[Office 365:n kehittynyt uhkien suojaus](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Advanced Threat Protection (ATP) auttaa suojaamaan yritystäsi kehittyneiltä tietojenkalastelu- ja kiristysohjelmahyökkäyksiltä, jotka on suunniteltu vaarantamaan työntekijöiden tai asiakkaiden tiedot. Ominaisuuksia ovat:
    
  - Kehittynyt liitetiedostojen skannaus ja ai-käyttöinen analyysi vaarallisten viestien havaitsemiseksi ja hylkäämiseksi.
    
  - Sähköpostin linkkien automaattiset tarkistukset, joissa arvioidaan, kuuluvatko ne tietojenkalastelujärjestelmään. Tämä estää sinua käyttämästä vaarallisia verkkosivustoja.

- **[Intunen täydet ominaisuudet Azure-portaalissa](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Azure-portaalin Intune-hallintakeskuksen avulla voit määrittää muita suojausominaisuuksia, kuten MacOS-laitteiden, iPhonen ja Android-laitteiden hallinnan sekä Windowsin kehittyneen laitehallinnan, jotka eivät ole käytettävissä Microsoftin kautta. 365 Business -hallintakeskus.
- **Sama [ehdollinen käyttöoikeus](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) kuin Azure AD P1 -palvelupaketilla**


    Ehdollinen käyttö voi auttaa suojaamaan organisaatiotasi kirjautumisriskiltä, käyttämään käyttöyrityksiä odottamattomasta verkosta tai maa-asetustolta, käyttämään riskialttiiden laitetyyppien käyttöyrityksiä ja niin edelleen. Ehdollisen käytön käytännöt otetaan käyttöön ensimmäisen todennuksen päätyttyä, ja se käyttää ensimmäisen todennustapahtuman signaaleja selvittääkseen, onko yritys, estetty vai onko useampi todiste (kuten toinen tunnistusmuoto) tarvitaan.

    Ehdollisen käytön ominaisuudet ovat seuraavat:

    - Käyttäjänimeen, ryhmään ja rooliin perustuva käyttö
    - [Sovellukseen perustuva](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) käyttö 
    - [Käyttö sijainnin perusteella](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  sallia pääsyn vain luotetuista IP-alueista tai tietyistä maista 
    - Vaadi mfa pääsyä varten
    - [Vanhan todennuksen](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication) käyttävien sovellusten käytön estäminen
    - Sovellusten tp-käytön vaatiminen [Intune-sovelluksen suojaus](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Mukautettu todennus, kuten MFA muiden valmistajien, esimerkiksi DUO:n, kanssa.
   
    Muut ominaisuudet:
    - [Hybridi-Azure](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) AD:n itsepalvelusalasanan palautus
    
## <a name="compliance-features"></a>Vaatimustenmukaisuuden ominaisuudet

Microsoft 365 Business -tilauksesi sisältää ominaisuuksia, joiden avulla voit ylläpitää vaatimustenmukaisuus- ja sääntelystandardeja.

- **[Yleiskatsaus tietojen menetyksen ehkäisykäytäntöihin](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    Voit määrittää DLP:n tunnistamaan automaattisesti arkaluonteiset tiedot, kuten luottokorttien numerot, henkilötunnukset ja niin edelleen, estääksesi niiden tahattoman jakamisen yrityksesi ulkopuolella.
    
- **[Exchange Online Archiving](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online Archiving -käyttöoikeuden avulla viestit voidaan arkistoida helposti jatkuvalla tietojen varmuuskopioinnilla. Se tallentaa kaikki käyttäjän sähköpostit, mukaan lukien poistetut kohteet, jos niitä tarvitaan myöhemmin etsimistä tai palauttamista varten. Lisäksi voit käyttää erilaisia säilytyskäytäntöjä sähköpostitietojen säilyttämiseen oikeustoimiin, eDiscoveryen tai vaatimustenmukaisuusvaatimusten täyttämiseen.
    
- **[Luottamuksellisuusmerkinnät](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Microsoft 365 Business sisältää kaikki [Azure Information Protection Plan 1](https://go.microsoft.com/fwlink/p/?linkid=871407):n ominaisuudet. Tämän suunnitelman avulla voit luoda **herkkyystarroja,** joiden avulla voit hallita sähköpostin ja asiakirjojen arkaluonteisten tietojen käyttöä ohjausobjekteilla, kuten Älä välitä- ja Älä kopioi -toimintoja. Voit myös luokitella arkaluonteiset tiedot "luottamuksellisiksi" ja määrittää, miten salaisia tietoja voidaan jakaa yrityksen ulkopuolella ja sisällä. Yritystason salausta on helppo käyttää sähköpostiin ja asiakirjoihin, jotta tietosi pysyvät yksityisinä. Voit myös asentaa Azure Information Protection -asiakasapuohjelman Office-sovelluksille. Lisätietoja on kohdassa [Azure Information Protectionin yhdistetty merkintäasiakas](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). Jos haluat käyttää herkkyystarroja, asenna **AzInfoProtection_UL.exe**.

Voit hallita näitä ominaisuuksia &amp; Tietoturvan yhteensopivuuskeskuksessa ja Intune-hallintakeskuksessa. Ajan mittaan yksinkertaistetut ohjausobjektit lisätään Microsoft 365 Business -hallintakeskukseen.
  
    
## <a name="faq"></a>Usein kysytyt kysymykset

 ### <a name="are-these-security-features-available-in-all-markets"></a>Ovatko nämä turvaominaisuudet saatavilla kaikilla markkina-alueilla?
  
Kyllä, nämä ominaisuudet ovat käytettävissä kaikilla markkinoilla, joilla Microsoft 365 Business myydään.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Miten löydän tietoturvan &amp; yhteensopivuuskeskuksen?
  
1. [Kirjaudu Microsoft 365 Businessiin](https://portal.microsoft.com/) järjestelmänvalvojan tunnistetiedoilla. 
    
2. Etsi vasemmasta siirtymisruudusta **Hallintakeskukset** ja laajenna se. 
    
    ![Valitse Microsoft 365 -hallintakeskuksen vasemmassa siirtymisruudussa Hallintakeskukset.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Siirry tietoturvan yhteensopivuuskeskukseen &amp; valitsemalla ** &amp; Suojauksen yhteensopivuus.**
