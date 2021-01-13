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
description: Tutustu Microsoft 365 Business Premiumin suojausominaisuuksiin, joiden avulla voit suojata tietosi tietokoneissa, puhelimissa ja taulutietokoneissa.
ms.openlocfilehash: b7fdd3d7fa25c23ee49ae82aa037588d8fba61a1
ms.sourcegitcommit: 83a40facd66e14343ad3ab72591cab9c41ce6ac0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/13/2021
ms.locfileid: "49840385"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Microsoft 365 Business Premiumin suojaus- ja yhteensopivuusominaisuudet

Microsoft 365 Business Premium tarjoaa yksinkertaistettuja suojausominaisuuksia, joiden avulla voit suojata tietosi tietokoneissa, puhelimissa ja taulutietokoneissa.
    
## <a name="microsoft-365-admin-center-security-features"></a>Microsoft 365 -hallintakeskuksen suojausominaisuudet

Voit hallita hallintakeskuksen monia Microsoft 365 Business Premium -suojausominaisuuksia, joiden avulla voit ottaa nämä ominaisuudet käyttöön ja poistaa ne käytöstä. Hallintakeskuksessa voit tehdä seuraavat toimet:
  
- [Määritä sovellusten hallinta-asetukset Android- tai iOS-laitteille.](app-protection-settings-for-android-and-ios.md) 
    
    Näitä asetuksia ovat esimerkiksi tiedostojen poistaminen passiivisista laitteesta tietyn ajan kuluttua, työtiedostojen salaaminen, PIN-koodin määrittäminen käyttäjille ja niin edelleen.
    
- [Määritä sovellusten suojausasetukset Windows 10 -laitteille.](protection-settings-for-windows-10-devices.md) 
    
    Näitä asetuksia voidaan soveltaa yrityksen tietoihin sekä yrityksen omistamista että omistamista laitteista.
    
- [Määritä laitesuojausasetukset Windows 10 -laitteille.](protection-settings-for-windows-10-pcs.md) 
    
    BitLocker-salauksen avulla voit suojata tietoja, jos laite katoaa tai varastetaan, ja antaa [Windows Exploit Guardin](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) tarjota lisäsuojausta kiristysohjelmilta. [](https://go.microsoft.com/fwlink/p/?linkid=871405) 
    
- [Yritystietojen poistaminen laitteista](remove-company-data.md)
    
    Voit poistaa yrityksen tiedot etäyhteydellä, jos laite katoaa, varastetaan tai työntekijä lähtee yrityksestäsi.
    
- [Palauta Windows 10 -laitteet tehdasasetuksiin.](reset-devices-to-factory-settings.md) 
    
    Voit palauttaa kaikki Windows 10 -laitteet, joissa on käytössä laitteen suojausasetukset.
    
## <a name="additional-security-features"></a>Muut suojaustoiminnot 

Microsoft 365 Business Premiumin lisäominaisuudet ovat käytettävissä, jotta voit suojata yritystäsi kyberuhkilta ja suojata luottamuksellisia tietoja.
  
- **[Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)**
    
    Microsoft Defender for Office 365 auttaa suojaamaan liiketoimintaasi kehittyneiltä tietojen kalastelu- ja kiristysohjelmahyökkäyksiltä, jotka on suunniteltu työntekijöiden tai asiakkaiden tietojen vaarantumiseen. Ominaisuuksia ovat seuraavat:
    
  - Kehittynyt liitteiden skannaus ja AI-käyttöinen analyysi, joka tunnistaa ja hylkää vaarallisia viestejä.
    
  - Sähköpostiviestin linkkien automaattiset tarkistukset sen arvioimiseksi, ovatko ne osa tietojenkalastelumallia. Näin pysyt turvassa epäluotettamattomien sivustojen käytön kanssa.

- **[Intunen kaikki ominaisuudet Azure-portaalissa](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Kun käytät Intune-hallintakeskusta Azure-portaalissa, voit määrittää muita suojausominaisuuksia, kuten MacOS-laitteiden, iPhonen ja Android-laitteiden hallinnan, sekä Windowsin kehittyneen laitehallinnan, jotka eivät ole käytettävissä Microsoft 365 -hallintakeskuksessa.
- **Sama [ehdollinen käyttöoikeus](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) kuin Azure AD Premium P1 -palvelupaketti**


    Ehdollinen käyttö voi auttaa suojaamaan organisaatiotasi kirjautumisriskiltä, odottamattomalta verkko- tai aluetasolta, riskialttiilta laitetyypeilta ja niin edelleen. Ehdollisten käyttöoikeuksien käytännöt ovat käytössä, kun ensimmäinen todennus on suoritettu, ja se määrittää ensimmäisen todennustapahtuman signaalien avulla, onko yrityskäyttö hyväksytty, hylätty tai vaaditaanko useampia todennukseen (esimerkiksi toisen tunnistusmenetelmän) ehtoja.

    Ehdolliset käyttöoikeusominaisuudet ovat seuraavat:

    - Access käyttäjänimen, ryhmän ja roolin perusteella
    - Access [sovelluksen perusteella](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Access sijainnin perusteella;](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration)  salli käyttö vain luotetusta IP-alueista tai tietyistä maista 
    - MFA:n edellytäminen käytön ajaksi
    - Estä vanhaa todennusta versioiden [todennusta versioiden käytön estäminen](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Sovellusten edellyttäminen [Intune-sovellussuojauksen käyttöä varten](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Mukautettu todentaminen, kuten MFA kolmannen osapuolen palveluntarjoajien kanssa, esimerkiksi DUO.
   
    Muut ominaisuudet:
    - [Azure AD:n yhdistelmäympäristön](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) omatoiminen salasanan vaihtaminen
    
## <a name="compliance-features"></a>Yhteensopivuusominaisuudet

Microsoft 365 Business Premium -tilauksesi sisältää ominaisuuksia, joiden avulla voit ylläpitää yhteensopivuus- ja säädöstenmukaisuusstandardeja.

- **[Yleiskatsaus tietojen menetyksen estämisen käytännöistä](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies)** (DLP). 
    
    Voit määrittää DLP:n tunnistamaan luottamukselliset tiedot, kuten luottokorttinumerot ja sosiaaliturvatunnukset, automaattisesti, jotta ne eivät vahingossa jaa tietoja yrityksen ulkopuolelle.
    
- **[Exchange Online Archiving](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online Archiving -käyttöoikeuden avulla viestit voidaan arkistoida helposti jatkuvalla tietojen varmuuskopioinnilla. Se tallentaa kaikki käyttäjän sähköpostiviestit, poistetut kohteet mukaan lukien, jos niitä tarvitaan myöhemmin etsinnän tai palauttamisen varalta. Lisäksi voit käyttää erilaisia säilytyskäytäntöjä, kun haluat säilyttää sähköpostitiedot oikeusjutusta, eDiscoveryta tai vaatimustenmukaisuusvaatimuksia varten.
    
- **[Luottamuksellisuusmerkinnät](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Microsoft 365 Business Premium sisältää kaikki [Azure Information Protection Plan 1:n ominaisuudet.](https://go.microsoft.com/fwlink/p/?linkid=871407) Tämän suunnitelman avulla voit  luoda luottamuksellisuusotsikoita, joiden avulla voit hallita luottamuksellisten tietojen pääsyä sähköpostissa ja asiakirjoissa, kuten "Älä lähetä edelleen" ja "Älä kopioi". Voit myös luokitella luottamukselliset tiedot luottamuksellisiksi ja määrittää, miten luokiteltuja tietoja voidaan jakaa yrityksen ulkopuolella ja sisällä. Yritystason salausta on helppo käyttää sähköposteihin ja asiakirjoihin, jotta tiedot ovat yksityisiä. Voit myös asentaa Azure Information Protection -asiakasohjelman apuohjelman Office-sovelluksiin. Lisätietoja on azure [information protectionin yhtenäisessä osoitetarrojen asiakasohjelmassa.](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history) Asenna luottamuksellisuusmerkinnät **-AzInfoProtection_UL.exe.**

Voit hallita näitä ominaisuuksia tietoturvan yhteensopivuuskeskuksessa &amp; ja Intune-hallintakeskuksessa. Ajan kuluessa yksinkertaistetut ohjausobjektit lisätään Microsoft 365 -hallintakeskukseen.
  
    
## <a name="faq"></a>Usein kysytyt kysymykset

 ### <a name="are-these-security-features-available-in-all-markets"></a>Ovatko nämä suojausominaisuudet käytettävissä kaikilla markkina-alueilla?
  
Kyllä, nämä ominaisuudet ovat käytettävissä kaikilla markkina-alueilla, joilla Microsoft 365 Business Premium myydään.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Miten löydän Tietoturvan &amp; yhteensopivuuskeskuksen?
  
1. [Kirjaudu Sisään Microsoft 365 Business Premiumiin](https://portal.microsoft.com/) järjestelmänvalvojan tunnistetiedoilla. 
    
2. Etsi hallintakeskukset vasemmasta **siirtymisruudusta ja** laajenna se. 
    
    ![Valitse Microsoft 365 -hallintakeskuksen vasemmassa siirtymispalkin kohdassa Hallintakeskukset.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Siirry **&amp; tietoturvan** yhteensopivuuskeskukseen valitsemalla &amp; Tietoturvan yhteensopivuus.
