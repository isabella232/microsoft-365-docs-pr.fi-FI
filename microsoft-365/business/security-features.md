---
title: Microsoft 365 Business Premium ja yhteensopivuusominaisuuksien avulla
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Tutustu tietoturvaominaisuuksiin, jotka Microsoft 365 Business Premium suojata tietosi tietokoneissa, puhelimissa ja tableteissa.
ms.openlocfilehash: 50b74ed18d641e8de38db3284c3ef3abf319825f4f7dbe02b6575f6c0fbc6f85
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53887565"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Microsoft 365 Business Premium ja yhteensopivuusominaisuuksien avulla

Microsoft 365 Business Premium tarjoaa yksinkertaistettuja suojausominaisuuksia, joiden avulla voit suojata tietosi tietokoneissa, puhelimissa ja taulutietokoneissa.
    
## <a name="microsoft-365-admin-center-security-features"></a>Microsoft 365 -hallintakeskus suojausominaisuudet

Voit hallita monia hallintakeskuksen Microsoft 365 Business Premium suojausominaisuuksia, joiden avulla voit ottaa nämä ominaisuudet käyttöön tai poistaa ne käytöstä yksinkertaisella tavalla. Hallintakeskuksessa voit tehdä seuraavat toimet:
  
- [Määritä sovellusten hallinta-asetukset Android- tai iOS-laitteille.](app-protection-settings-for-android-and-ios.md) 
    
    Näitä asetuksia ovat esimerkiksi tiedostojen poistaminen käytöstä poistetulta laitteelta tietyn ajan kuluttua, työtiedostojen salaaminen, PIN-koodin määrittäminen käyttäjille ja niin edelleen.
    
- [Määritä sovellusten suojausasetukset Windows 10 laitteille.](protection-settings-for-windows-10-devices.md) 
    
    Näitä asetuksia voidaan käyttää yritystietoihin sekä yrityksen omistamista että omistamista laitteista.
    
- [Määritä laitteiden suojausasetukset Windows 10 laitteille.](protection-settings-for-windows-10-pcs.md) 
    
    Voit ottaa [BitLocker-salauksen](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions) käyttöön tietojen suojaamiseksi, jos laite katoaa tai varastetaan, ja sallia [Windows Exploit Guardin](/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) tarjota lisäsuojausta kiristysohjelmilta. 
    
- [Yritystietojen poistaminen laitteista](remove-company-data.md)
    
    Voit poistaa yrityksen tiedot etänä, jos laite katoaa, varastetaan tai työntekijä lähtee yrityksestäsi.
    
- [Palauta Windows 10 tehdasasetukset](reset-devices-to-factory-settings.md) . 
    
    Voit palauttaa kaikki Windows 10 laitteet, joissa on laitteen suojausasetukset käytössä.
    
## <a name="additional-security-features"></a>Muut suojaustoiminnot 

Voit suojata Microsoft 365 Business Premium kyberuhkilta ja suojata luottamuksellisia tietoja Microsoft 365 Business Premium ominaisuuksia.
  
- **[Microsoft Defender for Office 365](../security/office-365-security/defender-for-office-365.md)**
    
    Microsoft Defender for Office 365 auttaa suojaamaan liiketoimintaasi kehittyneiltä tietojen kalastelu- ja kiristysohjelmahyökkäyksiltä, jotka on suunniteltu työntekijöiden tai asiakkaiden tietojen vaarantumiseen. Ominaisuuksia ovat:
    
  - Kehittynyt liitteiden tarkistus ja AI-käyttöinen analyysi, jonka avulla voit tunnistaa ja hylätä vaarallisia viestejä.
    
  - Automaattinen sähköpostilinkkien tarkistus sen arvioimiseksi, kuuluuko ne tietojenkalasteluun. Näin pysyt turvassa, jos et voi käyttää vaarallisia sivustoja.

- **[Intunen kaikki ominaisuudet Azure-portaalissa](/mem/intune/fundamentals/what-is-intune)**
    
    Kun käytät Intune-hallintakeskusta Azure-portaalissa, voit määrittää muita suojausominaisuuksia, kuten MacOS-laitteiden hallinnan, iPhone- ja Android-laitteiden hallinnan sekä Windows:n kehittyneet laitehallintaominaisuudet, jotka eivät ole käytettävissä Microsoft 365 -hallintakeskus.
- **Sama [ehdollinen käyttöoikeus](/azure/active-directory/conditional-access/overview) kuin Azure AD Premium P1 -suunnitelmassa**


    Ehdollinen käyttöoikeus voi auttaa suojaamaan organisaatiota kirjautumisriskiltä, käyttämään odottamattomalta verkko- tai alueelta, käyttämään yrityksiä riskialttiilta laitetyypeilta ja niin edelleen. Ehdollisten käyttöoikeuksien käytännöt ovat käytössä, kun ensimmäinen todennus on valmis, ja se määrittää ensimmäisen todennustapahtuman signaaleilla, onko yritetty käyttöoikeus hyväksyttävä, estettävä tai vaaditaanko useampia todennistustodennusta (kuten toinen tunnistusmuoto).

    Ehdollisen käyttöoikeuden ominaisuudet ovat seuraavat:

    - Access käyttäjänimen, ryhmän ja roolin perusteella
    - Access [sovelluksen perusteella](/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Access sijainnin perusteella](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  salli käyttö vain luotettavilta IP-alueilta tai tietyistä maista 
    - MFA:n edellytäminen käytön ajaksi
    - Estä vanhaa todennusta versioiden [todennusta versioiden käytön estäminen](/azure/active-directory/conditional-access/block-legacy-authentication)
    - Sovellusten edellyttäminen [Intune-sovelluksen suojauksen käyttöön](/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Mukautettu todentaminen, kuten MFA kolmannen osapuolen palveluntarjoajissa, esimerkiksi DUO.
   
    Muut ominaisuudet:
    - Azure AD [-yhdistelmäympäristön](/azure/active-directory/authentication/concept-sspr-customization) omatoiminen salasanan vaihto
    
## <a name="compliance-features"></a>Yhteensopivuusominaisuudet

Tilauksesi Microsoft 365 Business Premium ominaisuuksia, joiden avulla voit ylläpitää vaatimustenmukaisuus- ja sääntelystandardeja.

- **[Lisätietoja tietojen menetyksen estämisestä](../compliance/dlp-learn-about-dlp.md))** (DLP). 
    
    Voit määrittää DLP:n tunnistamaan luottamukselliset tiedot, kuten luottokorttinumerot, henkilötunnukset ja niin edelleen, jotta niiden tahaton jakaminen yrityksen ulkopuolelle voidaan estää.
    
- **[Exchange Online Archiving](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online Archiving-käyttöoikeuden avulla viestit voidaan arkistoida helposti jatkuvalla tietojen varmuuskopioinnilla. Se tallentaa kaikki käyttäjän sähköpostiviestit poistetut kohteet mukaan lukien, jos niitä tarvitaan myöhemmin etsinnän tai palauttamisen vuoksi. Lisäksi voit käyttää erilaisia säilytyskäytäntöjä, jos haluat säilyttää sähköpostitiedot oikeus oikeusjutusta, eDiscoveryta tai yhteensopivuusvaatimuksia varten.
    
- **[Luottamuksellisuusmerkinnät](../compliance/sensitivity-labels.md)**

   Microsoft 365 Business Premium sisältää kaikki [Azure Information Protection Plan 1:n ominaisuudet.](https://go.microsoft.com/fwlink/p/?linkid=871407) Tämän suunnitelman avulla voit  luoda luottamuksellisuusotsikoita, joiden avulla voit hallita luottamuksellisten tietojen pääsyä sähköposteihin ja asiakirjoihin, kuten "Älä lähetä edelleen" ja "Älä kopioi". Voit myös luokitella luottamukselliset tiedot luottamuksellisiksi ja määrittää, miten luokiteltuja tietoja voidaan jakaa yrityksen ulkopuolelle ja yrityksen sisällä. Yritystason salausta on helppo käyttää sähköpostiviesteihin ja asiakirjoihin, jotta tiedot ovat yksityisiä. Voit asentaa myös Azure Information Protection -asiakasohjelman apuohjelman Office sovelluksille. Lisätietoja on kohdassa [Azure Information Protectionin yhdistetyn osoitetarra-asiakasohjelman tiedot.](/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history) Asenna luottamuksellisuusmerkinnät-AzInfoProtection_UL.exe. ****

Voit hallita näitä ominaisuuksia tietoturvakeskuksessa &amp; ja Intune-hallintakeskuksessa. Ajan kuluessa yksinkertaiset ohjausobjektit lisätään Microsoft 365 -hallintakeskus.
  
    
## <a name="faq"></a>Usein kysytyt kysymykset

 ### <a name="are-these-security-features-available-in-all-markets"></a>Ovatko nämä suojausominaisuudet käytettävissä kaikilla markkina-alueilla?
  
Kyllä, nämä ominaisuudet ovat käytettävissä kaikilla markkina-alueilla, Microsoft 365 Business Premium myydään.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Miten löydän Tietoturvan &amp; yhteensopivuuskeskuksen?
  
1. [Kirjaudu sisään Microsoft 365 Business Premium](https://portal.microsoft.com/) järjestelmänvalvojan tunnistetiedoilla. 
    
2. Etsi hallintakeskukset vasemmasta **siirtymisruudusta** ja laajenna se. 
    
    ![Valitse hallintakeskukset Microsoft 365 -hallintakeskus siirtymispalkin vasemmasta siirtymispalkin valikosta.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Siirry **&amp; Tietoturvan yhteensopivuuskeskukseen** &amp; valitsemalla Tietoturvan yhteensopivuus.
