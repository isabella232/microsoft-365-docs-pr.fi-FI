---
title: Microsoft 365 Business tietoturvan ja määritystenmukaisuuden suhteen ominaisuudet
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
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Lisätietoja suojausominaisuuksia, jotka Microsoft 365 Business mukana.
ms.openlocfilehash: bd61ad3bf1b34635a7b80f1c9ccf63fa98d31915
ms.sourcegitcommit: 274af83139ad7da3aa33366c3323d533d95c7db4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/17/2019
ms.locfileid: "35017518"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>Microsoft 365 Business tietoturvan ja määritystenmukaisuuden suhteen ominaisuudet

365 Microsoft Business tarjoaa yksinkertaistettu suojausominaisuudet suojaa tietosi, tietokoneet, puhelimet ja tabletit.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Microsoft 365 Business admin center suojausominaisuudet

![Nauha, joka osoittaa https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Voit hallita monia hallintakeskukseen, jonka avulla voit ottaa nämä ominaisuudet käyttöön yksinkertaistettu helposti Microsoft 365 Business suojausominaisuuksia. Admin Centerissä voit tehdä seuraavaa:
  
  
- [Määrittää sovelluksen asetukset Android- tai iOS laite](app-protection-settings-for-android-and-ios.md) . 
    
    Näihin asetuksiin kuuluvat tiedostojen poistaminen käytöstä laitteen tietyksi jaksoksi, työn tiedostojen salaamiseen, edellyttävät, että käyttäjät määrittää PIN-koodi, jne.
    
- [Määrittää sovelluksen suojausasetuksia Windows 10-laitteille](protection-settings-for-windows-10-devices.md) . 
    
    Nämä asetukset voidaan ottaa käyttöön yrityksen tiedot sekä yrityksen omistamien tai henkilökohtaisesti omistaa laitteet.
    
- [Määrittää laitteen asetukset Windows 10-laitteille](protection-settings-for-windows-10-pcs.md) . 
    
    Voit ottaa [BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) -salaus auttaa suojaamaan tietoja siltä varalta, että laite katoaa tai varastetaan ja ottaa käyttöön [Windows hyödyntää Guard](https://go.microsoft.com/fwlink/p/?linkid=871404) voit suojata ransomware. 
    
- [Yritystietojen poistaminen laitteista](remove-company-data.md)
    
    Yrityksen tietoja etäyhteyden kautta voit pyyhkiä, jos laite katoaa, varastetaan, tai jos työntekijä lähtee yrityksen.
    
- [Niiden tehdasasetusten palauttaminen Windows 10 laitteet](reset-devices-to-factory-settings.md) . 
    
    Voit palauttaa Windows 10 laitteet, joissa on käytetty laite suojausasetukset.
    
## <a name="additional-security-features"></a>Muut suojaustoiminnot 

Kehittyneitä ominaisuuksia Microsoft Business-365 ovat käytettävissä auttaa sinua suojaamaan yritystäsi cyber uhilta ja luottamuksellisten tietojen turvaamiseksi.
  
- **[Office 365 kehittyneen uhkien suojaa](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Advanced Threat Protection (ATP) suojaa yrityksesi kehittyneitä tietokalastelu- ja vaarantaa työntekijän tai asiakkaan tiedot suunniteltu ransomware hyökkäyksiä vastaan. Seuraavat ominaisuudet:
    
  - Liite kehittyneitä skannaus ja AI powered analyysi tunnistaa ja hylkää vaarallisten viestit.
    
  - Automaattinen tarkistaa linkkejä sähköpostitse arvioida, jos ne ovat osa tietojen kalastelun. Näin voit turvallisesti käyttämästä epäluotettavista WWW-sivustoista.

- **[Azure portaalin Intune täynnä ominaisuuksia](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Käytettäessä Azure portaalin admin Centerin avulla voit määrittää muita suojausominaisuuksia, kuten MacOS laitteet, iPhone ja Android laitteiden Lisäasetukset Windows Laitehallinta ja hoidon Intune eivät ole saatavana Microsoft 365 business hallintakeskukseen.
- **Saman [Ehdollisen käyttöoikeuden](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/overview) Azure AD P1-suunnitelma**

    Ehdollisen käyttöoikeuden voi auttaa suojaamaan organisaatiosi riskistä sisään, yrittää käyttää kieltä tai odottamattomia verkon, access yrittää lomakkeen riskialtis laitetyyppejä, ja niin edelleen. Ehdollisen käyttöoikeuden käytännöt ovat voimassa sen jälkeen, kun ensimmäinen todennus on valmis ja se käyttää Ensimmäinen todennus-signaalit Jos yritetty käyttö olisi hyväksyttävä, estää tai f todiste enemmän (esimerkiksi toisen lomakkeen tunnus) on tarvitaan.

    Ehdollisen käyttöoikeuden ominaisuuksista ovat:

    - Käyttäjä-, ryhmä- ja rooliin perustuvat käyttöoikeudet
    - Access [app perusteella](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Access sijainnin perusteella](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  Salli vain Luotetut IP-alueet tai tiettyjen maiden käyttö 
    - Access edellyttää MFA
    - Sovellukset, jotka [vanhan mallin mukainen todennus](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication) estää pääsyn
    - Apps tp käytöstä [Intune app suojaus](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Kolmannen osapuolen toimittajat, esimerkiksi DUO MFA kuten mukautettu todentaminen.
   
    Muita ominaisuuksia:
    - [Omatoiminen salasanan](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) hybridi Azure AD
    
## <a name="compliance-features"></a>Noudattamista ominaisuudet

Microsoft 365 liiketoiminnan tilaus sisältää ominaisuuksia, jotka auttavat säilyttää yhteensopivuuden ja standardien.

- **[Yleiskatsaus tietojen menetyksen ehkäisemiseen tähtäävissä](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    Voit määrittää DLP havaitsemaan arkaluontoisia tietoja, kuten luottokorttinumeroita, henkilötunnuksia jne estää tahattomat niiden jakamista yrityksen ulkopuolelle.
    
- **[Exchange Online Archiving](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Käyttöoikeuden Exchange Online arkistoida avulla viestit helposti jatkuvan tietojen varmuuskopiointi ja arkistointi. Se tallentaa kaikki käyttäjän sähköpostit, mukaan lukien poistetut kohteet siltä varalta, että niitä tarvitaan myöhemmin etsiminen ja palauttaminen. Lisäksi voit käyttää eri säilytyskäytännöt säilyttää tiedot oikeudenkäynnistä Pidot, eDiscovery, sähköposti tai yhteensopivuusvaatimusten täyttämiseksi.
    
- **[Azure-tietojen suojaaminen](https://go.microsoft.com/fwlink/p/?linkid=871406)**
    
    Tietojen suojaus auttaa luottamukselliset tiedot, sähköposti ja asiakirjat kontrolloida ohjausobjekteja, ”Älä välitä” ja ”kopioi”. Voit myös luokitella arkaluonteisia tietoja, kuten ”Luottamuksellinen” ja määrittää turvaluokitellun tiedon jakamista ulkopuolella ja yrityksen sisällä. Enterprise-luokan salaus on helppo sähköposti ja tietosi yksityisinä asiakirjoja. 365 Microsoft Business sisältää kaikki ominaisuudet [Azure tietojen suojauksen suunnitteleminen](https://go.microsoft.com/fwlink/p/?linkid=871407)1. Voit myös asentaa Azure tietojen suojaus asiakkaan apuohjelma Office-sovelluksille. Lisätietoja [Azure tietojen suojaaminen client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide)-järjestelmänvalvojan oppaassa.

Voit hallita näitä ominaisuuksia suojaus- &amp; Compliance Centeriin ja Intune hallintakeskukseen. Ajan mittaan yksinkertaistettu ohjausobjektit lisätään Microsoft 365 Business hallintakeskukseen.
  
    
## <a name="faq"></a>Usein kysytyt kysymykset

 ### <a name="are-these-security-features-available-in-all-markets"></a>Ovatko nämä suojausominaisuudet käytettävissä kaikilla markkina-alueilla?
  
Kyllä, nämä ominaisuudet ovat käytettävissä kaikilla markkina-alueilla, jossa myydään Microsoft 365 Business.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Miten löydän vakuuden &amp; Compliance Centeriin?
  
1. [Microsoft 365 Business kirjautua](https://portal.microsoft.com/) järjestelmänvalvojan tunnuksilla. 
    
2. Siirtyminen vasemmalle Etsi **Admin keskittää** ja laajentaa sitä. 
    
    ![Valitse Microsoft 365 admin Centerissä siirtyminen vasemmalle Admin centers.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Valitse **suojauksen &amp; yhteensopivuuden** Go to Security &amp; compliance Centeriin.