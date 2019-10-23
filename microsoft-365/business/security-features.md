---
title: Microsoft 365 Business Securityn ja yhteensopivuuden ominaisuudet
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
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Lue lisä tietoja Microsoft 365 Businessin mukana tulevien suojaus ominaisuuksien ominaisuuksista.
ms.openlocfilehash: 0d1c35192bf82ac61e59356cda4d9fb29cb3d995
ms.sourcegitcommit: 4d5e4cb3fa3ab45ad15f103c720c77277b22fc23
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/22/2019
ms.locfileid: "37636768"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>Microsoft 365 Business Securityn ja yhteensopivuuden ominaisuudet

Microsoft 365 Business tarjoaa yksinkertaistettuja tieto turva ominaisuuksia, jotka suojaavat tietojasi tieto koneilla, puhelimilla ja tableteilla.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Microsoft 365 Business Admin Centerin suojaus ominaisuudet

[![Etiketti, jonka avulla voit tietää, että hallinta keskus on muuttumassa ja löydät lisä tietoja osoitteessa aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Voit hallita useita Microsoft 365 Business Security-ominaisuuksia hallinta keskuksessa, jolloin voit ottaa nämä ominaisuudet käyttöön tai poistaa ne käytöstä yksinkertaistetulla tavalla. Hallinta keskuksessa voit tehdä seuraavaa:
  
  
- [Määritä sovellusten hallinta-asetukset Android-tai iOS-laitteille](app-protection-settings-for-android-and-ios.md) . 
    
    Nämä asetukset sisältävät tiedostojen poistamisen passiivisen laitteen jälkeen tietyn ajan, salaamalla työtiedostot, jotka edellyttävät, että käyttäjät asettaa PIN, jne.
    
- [Aseta sovellusten suojaus asetukset Windows 10-laitteille](protection-settings-for-windows-10-devices.md) . 
    
    Näitä asetuksia voidaan soveltaa yrityksen tietoihin sekä yrityksen omistamiin että henkilökohtaisesti omistamiin laitteisiin.
    
- [Aseta laitteen suojaus asetukset Windows 10-laitteille](protection-settings-for-windows-10-pcs.md) . 
    
    Voit ottaa [BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) -Sala uksen käyttöön suojatakseen tietoja siinä tapa uksessa, että laite katoaa tai varastetaan, ja mahdollistaa [Windowsin hyväksikäyttö](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) suojan tarjoamaan kehittynyttä suojausta kiristys ohjelmilta. 
    
- [Yritystietojen poistaminen laitteista](remove-company-data.md)
    
    Voit pyyhkiä yrityksen tiedot etänä, jos laite katoaa, varastetaan tai työn tekijä poistuu yrityksestasi.
    
- [Palauta Windows 10-laitteet tehdas asetuksiin](reset-devices-to-factory-settings.md) . 
    
    Voit nollata kaikki Windows 10-laitteet, joissa on käytössä laitteen suojaus asetukset.
    
## <a name="additional-security-features"></a>Muut suojaustoiminnot 

Microsoft 365 Businessin lisä ominaisuudet auttavat suojaamaan yritystäsi kyberuhkilta ja suojelemaan arkaluonteisia tietoja.
  
- **[Office 365 Advanced uhkien torjunta](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Kehittynyt uhkien torjunta (ATP) auttaa suojautuminen kehittyneiltä tietojenkalasteluilta ja kiristys ohjelma hyökkäyksiltä, joiden tarkoituksena on vaarantaa työn tekijöiden tai asiakkaiden tiedot. Ominaisuuksia ovat:
    
  - Hienostunut kiinnitys skannaus ja tekoäly analyysi vaarallisten viestien havaitsemiseksi ja hylkäämistä varten.
    
  - Automaattinen Sähkö posti linkkien tarkistus, jotta voidaan arvioida, ovatko ne osa tietojenkalastelujärjestelmää. Näin voit turvallisesti käyttää vaarallisia verkko sivustoja.

- **[Intune-järjestelmän täydet ominaisuudet Azure-portaalissa](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Käyttämällä Intune hallinta keskukseen Azure-portaalissa voit määrittää lisä suojaus ominaisuuksia, kuten MacOS-laitteiden, iPhonen ja Android-laitteiden hallinta sekä Windowsin laajennettu laite hallinta, jotka eivät ole saatavilla Microsoftin 365 liike toiminnan hallinta keskus.
- **Sama [ehdollinen pääsy](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/overview) kuin Azure AD P1-suunnitelma**

    Ehdollinen käyttö oikeus voi suojata organisaatiotasi kirjautumisriskiltä, käyttää odottamattomia verkko-tai aluekohtaisia yrityksiä, muodostaa riskialttiita laite tyyppejä ja niin vielä. Ehdolliset käyttö oikeus käytännöt otetaan käyttöön sen jälkeen, kun ensimmäinen todennus on suoritettu, ja se käyttää ensimmäisen todennus tapahtuman signaaleja määrittääkseen, onko käytön yrittämisestä hyväksyttävä, kieltää tai f enemmän todisteita (kuten toinen tunnistus muoto) Tarvitaan.

    Ehdolliset käyttö oikeudet sisältyvät:

    - Käyttö oikeus käyttäjä nimen, ryhmän ja roolin perusteella
    - [Sovellukseen perustuva](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) käyttö 
    - [Käyttö sijainnin perusteella](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  Salli pääsy vain luotettavista IP-alueista tai tietyistä maista 
    - Edellytä MFA-käyttö oikeutta
    - Estä pääsy sovelluksiin, jotka käyttävät [vanhaa todennusta](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Vaadi apps TP käyttää [Intune App Protection](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Mukautettu todennus, kuten MFA kolmannen osapuolen palveluntarjoajien kanssa, esimerkiksi DUO.
   
    Muita ominaisuuksia:
    - [Itsepalvelun Sala sanan nollaus](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) Hybrid Azure AD
    
## <a name="compliance-features"></a>Yhteensopivuuden ominaisuudet

Microsoft 365 Business-tilauksesi sisältää ominaisuuksia, joiden avulla voit ylläpitää yhteensopivuus-ja sääntely standardeja.

- **[Yleiskatsaus tietojen menetyksen estämis käytännöistä](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    Voit määrittää DLP-ohjelman tunnistamaan automaattisesti arkaluontoiset tiedot, kuten luotto korttien numerot ja sosiaaliturvatunnukset, jotta estät niiden vahingossa tapahtuvan jakamisen yrityksesi ulkopuolelle.
    
- **[Exchange Online Archiving](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online-arkistointi lisenssi mahdollistaa viestien helpon arkistoimisen jatkuvalla tietojen varmuus kopioinnilla. Se tallentaa kaikki käyttäjän sähkö postit, mukaan lukien poistetut kohteet, jos niitä tarvitaan myöhemmin löytämiseen tai palauttamiseen. Lisäksi voit käyttää eri säilytys käytäntöjä Sähkö posti tietojen säilyttämiseksi riita-asioiden, eDiscoveryn tai yhteensopivuus vaatimusten täyttämiseksi.
    
- **[Luottamuksellisuusmerkinnät](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Microsoft 365 Business sisältää kaikki [Azure-tieto suoja suunnitelman 1](https://go.microsoft.com/fwlink/p/?linkid=871407)ominaisuudet. Tämän suunnitelman avulla voit luoda **herkkyys tarroja**, joiden avulla voit valvoa arkaluontoisten tietojen käyttö oikeutta sähkö postissa ja asia kirjoissa, joissa on ohjaus objekteja, kuten "Älä välitä" ja "Älä kopioi". Voit myös luokitella arkaluonteiset tiedot luottamuksellisiksi ja määrittää, miten luottamuksellisia tietoja voidaan jakaa yrityksen ulkopuolella ja sisällä. Yritys tason salausta on helppo soveltaa sähkö postiin ja asia kirjoihin, jotta tietosi pysyvät yksityisissä. Voit myös asentaa Office-sovellusten Azure Information Protection-apuohjelman. Lisä tietoja on artikkelissa [Azure-tietojen suojaus Unified merkintä Client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). Jos kyseessä on herkkyys tarra, asenna **AzInfoProtection_UL. exe**.

Voit hallita näitä ominaisuuksia Security &amp; Compliance Centerissä ja Intune-hallinta keskuksessa. Ajan mittaan yksinkertaistetut ohjaimet lisätään Microsoft 365 Business-hallinta keskukseen.
  
    
## <a name="faq"></a>Usein kysytyt kysymykset

 ### <a name="are-these-security-features-available-in-all-markets"></a>Ovatko nämä turva ominaisuudet saatavilla kaikilla markkinoilla?
  
Kyllä, nämä ominaisuudet ovat käytettävissä kaikilla markkinoilla, joilla Microsoft 365 Business myydään.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Miten löydän tieto turvan &amp; yhteensopivuus keskuksen?
  
1. [Kirjaudu sisään Microsoft 365 Business](https://portal.microsoft.com/) -käyttö järjestelmän järjestelmänvalvojan tunniste tiedoilla. 
    
2. Etsi vasemmasta NAV-ohjelman **hallinta keskuksista** ja laajenna se. 
    
    ![Valitse vasemmasta NAV-ohjelman Microsoft 365-hallinta keskuksesta hallinta keskukset.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Siirry tieto &amp; turvan yhteensopivuus keskukseen valitsemalla ** &amp; suojaus yhteensopivuus** .
