---
title: Microsoft 365 Business Premiumin turvallisuus-ja yhteensopivuus ominaisuudet
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
description: Tutustu Microsoft 365 Business Premiumin käyttö oikeus ominaisuuksiin, jotka auttavat suojaamaan tietoja tieto koneilla, puhelimilla ja tableteilla.
ms.openlocfilehash: 587d80c27f867a387c901d23f4ec05f3c5905bf6
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/03/2020
ms.locfileid: "48843484"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Microsoft 365 Business Premiumin turvallisuus-ja yhteensopivuus ominaisuudet

Microsoft 365 Business Premium tarjoaa yksinkertaistettuja suojaus ominaisuuksia, jotka suojaavat tietoja tieto koneilla, puhelimilla ja tableteilla.
    
## <a name="microsoft-365-admin-center-security-features"></a>Microsoft 365-hallinta keskuksen käyttö oikeus ominaisuudet

Voit hallita monia Microsoft 365 Business Premium-tieto turva ominaisuuksia hallinta keskuksessa, jonka avulla voit ottaa nämä ominaisuudet käyttöön tai poistaa ne käytöstä yksinkertaisella tavalla. Hallinta keskuksessa voit tehdä seuraavat toimet:
  
- [Sovellusten hallinta-asetusten määrittäminen Android-tai iOS-laitteille](app-protection-settings-for-android-and-ios.md) . 
    
    Nämä asetukset sisältävät tiedostojen poistamisen käyttämättömästä laitteesta tietyn vaiheen jälkeen, salattaessa työtiedostoja, vaatimalla käyttäjiä määrittämään PIN-tunnuksen ja niin edelleen.
    
- [Sovellusten suojaus asetusten määrittäminen Windows 10-laitteille](protection-settings-for-windows-10-devices.md) . 
    
    Näitä asetuksia voidaan käyttää yrityksen tietoihin sekä yrityksen omistamissa että itse omistamissa laitteissa.
    
- [Laitteen suojaus asetusten määrittäminen Windows 10-laitteille](protection-settings-for-windows-10-pcs.md) . 
    
    Voit ottaa [BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) -Sala uksen käyttöön, jos haluat suojata tietoja, jos laite katoaa tai varastetaan, ja ottaa käyttöön [Windows Exploit Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) -suoja uksen, joka antaa kehittyneen suojan kiristys laitteita vastaan. 
    
- [Yritystietojen poistaminen laitteista](remove-company-data.md)
    
    Voit pyyhkiä yrityksen tiedot etänä, jos laite katoaa, varastetaan tai työn tekijä lähtee yrityksestä.
    
- [Palauta Windows 10-laitteet tehdas asetuksiksi](reset-devices-to-factory-settings.md) . 
    
    Voit palauttaa kaikki Windows 10-laitteet, joissa on käytössä laitteen suojaus asetukset.
    
## <a name="additional-security-features"></a>Muut suojaustoiminnot 

Microsoft 365 Business Premiumin lisä ominaisuuksia on saatavilla, jotka auttavat suojaamaan yritystäsi tieto verkko uhilta ja turvaamaan luottamukselliset tiedot.
  
- **[Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)**
    
    Microsoft Defender for Office 365 auttaa suojaamaan yritystäsi edistyneemmät tietojenkalastelulta ja kiristys ohjelmilta, jotka on suunniteltu työn tekijöiden tai asiakas tietojen vaarantamaan. Ominaisuuksiin kuuluvat:
    
  - Hienostunut liitteiden tarkistus ja AI-käyttöinen analyysi vaarallisten viestien havaitsemiseksi ja hylkäämiseksi.
    
  - Sähkö postin linkkien automaattinen tarkistus, jos haluat arvioida, ovatko ne osa tietojenkalastelujärjestelmää. Tämä estää haitallisten sivustojen käytön.

- **[Intunen kaikki ominaisuudet Azure-portaalissa](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Kun käytät Intune-hallinta keskusta Azure-portaalissa, voit määrittää muita tieto turva ominaisuuksia, kuten Mac OS-laitteiden, iPhonen ja Android-laitteiden hallinnan sekä Windowsin kehittyneet laitteiden hallinta toiminnot, jotka eivät ole käytettävissä Microsoft 365-hallinta keskuksen kautta.
- **Sama [Ehdollinen käyttäminen](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) kuin Azure AD Premium P1-palvelu paketin**


    Ehdollinen käyttäminen voi auttaa suojaamaan organisaatiotasi kirjautumisriskeiltä, käyttämään odottamattomia verkkoja tai maa-asetuksia, käyttämään riskialttiiden laite tyyppien yrityksiä ja niin edelleen. Ehdollisen käytön käytännöt on pakotettu, kun ensimmäinen todennus on valmis, ja se käyttää ensimmäisen todennus tapahtuman signaaleja määrittääkseen, onko yritys käyttö oikeus hyväksyttävä, estetty vai tarvitaanko muita todisteita (kuten toinen tunniste).

    Ehdollisen käytön ominaisuuksiin sisältyvät seuraavat:

    - Käyttäjä nimen, ryhmän ja roolin perusteella
    - [Sovellukseen perustuva](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) yhteys 
    - [Käyttäminen sijainnin perusteella](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  Salli vain luotettujen IP-alueiden tai tiettyjen maiden käyttäminen 
    - Edellytä MFA-käyttöä Accessissa
    - [Vanhaa todennusta](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication) käyttävien sovellusten käytön estäminen
    - Edellytä, että sovellus TP käyttää [Intune-sovelluksen suojausta](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Mukautettu todennus, kuten MFA kolmannen osapuolen palveluntarjoajien kanssa, esimerkiksi DUO.
   
    Muita ominaisuuksia:
    - [Omatoiminen Sala sanan palautus](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) Hybrid Azure AD:hen
    
## <a name="compliance-features"></a>Yhteensopivuus ominaisuudet

Microsoft 365 Business Premium-tilaukseesi sisältyy ominaisuuksia, jotka auttavat ylläpitämään vaatimustenmukaisuutta ja lain säädäntöä koskevia standardeja.

- **[Yleistä tietojen menetyksen esto käytännöistä](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies)** (DLP). 
    
    Voit määrittää DLP:N tunnistamaan automaattisesti luottamukselliset tiedot, kuten luotto kortti numerot ja sosiaaliturvatunnukset, jotta estetään niiden tahaton jakaminen yrityksen ulkopuolelta.
    
- **[Exchange Online Archiving](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online-arkistointi käyttö oikeus mahdollistaa viestien helpon arkistoinnin jatkuvan tietojen varmuus kopioinnin avulla. Se tallentaa kaikki käyttäjän sähkö postit, mukaan lukien poistetut kohteet, siinä tapa uksessa, että niitä tarvitaan myöhemmin löydöstä tai palauttamisesta. Lisäksi voit käyttää erilaisia säilytys käytäntöjä Sähkö posti tietojen säilyttämiseen oikeus toimiin, eDiscoveryyn tai yhteensopivuus vaatimusten täyttämiseen.
    
- **[Luottamuksellisuusmerkinnät](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Microsoft 365 Business Premium sisältää kaikki [Azuren tieto turva palvelu paketin 1](https://go.microsoft.com/fwlink/p/?linkid=871407)ominaisuudet. Tässä ohjelmassa voit luoda **Luottamuksellisuusotsikoita** , joiden avulla voit hallita sähkö postin ja asia kirjojen luottamuksellisten tietojen käyttö oikeuksia, esimerkiksi "Älä lähetä edelleen"-ja "Älä kopioi"-toimintoja. Voit myös luokitella luottamuksellisia tietoja luottamuksellisiksi ja määrittää, miten luokitellut tiedot voidaan jakaa yrityksen sisä-ja ulkopuolella. Yritys tason salausta on helppo käyttää sähkö postissa ja asia kirjoissa, jotta tietosi pysyvät yksityisinä. Voit asentaa myös Azure Information Protectionin Client-apuohjelman Office-sovelluksiin. Lisä tietoja on kohdassa [Azure Information Protectionin Unified-merkintä asiakas](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). Jos kyseessä on herkkyys tarra, asenna **AzInfoProtection_UL.exe**.

Voit hallita näitä ominaisuuksia tieto turvan &amp; yhteensopivuus keskuksessa ja Intune-hallinta keskuksessa. Ajan mittaan ne lisätään Microsoft 365-hallinta keskukseen.
  
    
## <a name="faq"></a>Usein kysytyt kysymykset

 ### <a name="are-these-security-features-available-in-all-markets"></a>Ovatko nämä turva ominaisuudet saatavilla kaikilla markkinoilla?
  
Kyllä, nämä ominaisuudet ovat käytettävissä kaikilla markkinoilla, joilla Microsoft 365 Business Premium on myynnissä.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Miten löydän tieto turvan &amp; yhteensopivuus keskuksen?
  
1. [Kirjaudu sisään Microsoft 365 Business Premiumiin](https://portal.microsoft.com/) järjestelmänvalvojan tunniste tiedoilla. 
    
2. Etsi vasemmasta siirtymis ruudusta **hallinta keskukset** ja laajenna se. 
    
    ![Valitse vasemmanpuoleisessa NAV-ohjelmassa Microsoft 365-hallinta keskuksessa hallinta keskukset.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Valitse **tieto &amp; turva yhteensopivuus,** jos haluat siirtyä tieto turvan &amp; yhteensopivuus keskukseen.
