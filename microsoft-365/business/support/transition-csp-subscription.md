---
title: Siirtyminen Microsoft 365 Business CSP-tilaus 
description: Ota selvää, miten voi siirtyä Microsoft 365 Business CSP tilauksen esikatselusta GA. 
author: jasongroce
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Business, Microsoft 365, SMB, siirtymä CSP-tilaus
ms.date: 11/01/2017
ms.openlocfilehash: 8109c0b00f06a15c12bbccf89e7f49dc3fa4b34a
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982483"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Siirtyminen Microsoft 365 Business CSP-tilaus

Jos sinulla on Microsoft 365 Business esikatselu CSP tilauksen noudattamalla tämän oppaan voit selvittää, miten voi siirtyä aiemmin esikatselu-tilauksen Microsoft 365 Business GA (Yleinen saatavuus).

**Siirtymisestä GA tilauksen esikatselu**

1. Kirjaudu sisään <a href="https://partnercenter.microsoft.com" target="_blank">Partner</a>Centeriin.
2. Dashboardista, **Asiakkaat**, valitse Etsi ja valitse yrityksen nimi.

    Yrityksen tilaukset näkyvät.

    ![Asiakkaan tilausten Partner Center](images/pc_customer_subscriptions_1.png)
    
3. Valitse yrityksen **tilaukset** -sivulla **Lisää tilaus**.
4. **Uusi tilaus** -sivulla Valitse **Small business** ja valitse sitten luettelosta **Microsoft 365 Business** .
5. Lisää käyttöoikeuksien määrä ja valitse sitten **Seuraava: Tarkista** tilaus ja valitse sitten **Lähetä**.

    ![Uusi tilaus Microsoft 365 Business tarkastelua](images/pc_customer_reviewnewsubscription.png)

    **Käyttöoikeuden perustuvat tilaukset** näkyvät **Microsoft 365 Business esikatselu** ja **365 Microsoft Business**. Sinun on seuraavaksi keskeyttää tilauksen esikatselu.

6. Valitse **Microsoft 365 Business esikatselu**.
7. Valitse **Microsoft 365 Business esikatselu** -sivulla **Suspended** keskeyttää tilauksen esikatselu.

    ![Keskeyttää tilauksen Microsoft 365 Business esikatselu](images/pc_customer_m365bpreview_suspend.png)

8. Valitse **Lähetä** vahvistus.

    Varmista, että **Microsoft 365 Business esikatselu** tila näkyy **Suspended** **tilaukset** -sivun.

    ![Vahvista tilauksen esikatselu tila on keskeytetty](images/pc_customer_m365bpreview_suspend_confirm.png)

9. Vaihtoehtoisesti voi myös tarkistaa Käyttöoikeussopimuksen ehtoja. Voit tehdä tämän seuraavasti:
    1. Valitse yrityksen **tilaukset** -sivun **käyttäjät ja käyttöoikeudet** .
    2. Valitse **käyttäjät ja käyttöoikeudet** -sivulle käyttäjä.
    3. Sivun käyttäjän **käyttöoikeuksien määrittäminen** -osassa ja se näkyy **Microsoft 365 Business**.

        ![Vahvista käyttäjä on liitetty Microsoft 365 Business käyttöoikeuden](images/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Asiakkaille ja käyttäjille aikana ja sen jälkeen siirtymisen vaikutukset

Siirtymän ja kirjaa siirron aikana on vaikutusta asiakkaille ja käyttäjille.

## <a name="impact-to-customers-who-dont-transition"></a>Asiakkaat, jotka eivät Muulla ohjelmistolla luodun vaikutus

Seuraavassa taulukossa on yhteenveto vaikutus asiakkaille, joilla ei ole Siirtyminen Microsoft 365 Business esikatselu tilauksen Microsoft 365 Business-tilaukseen.

|       | T + 30 T-0     | T + 30 T + 60 | T + 60 T + 120 | Lisäksi T + 120  |
|-------|-----------------|--------------|---------------|---------------|
| **Osavaltio** | Jatkoaika- | Vanhentunut      | Ei käytössä      | Deprovisioned |
| **Palvelun vaikutuksia**                                                        |
| **Microsoft 365 Business-hallintaportaaliin.** | Toimintoja ei ole vaikutusta | Toimintoja ei ole vaikutusta | Voit Lisää tai poista käyttäjiä, ostaa tilaukset.</br> Ei voi määrittää/revoke käyttöoikeuksia. | Asiakkaan tilauksen ja kaikki tiedot poistetaan. Järjestelmänvalvoja voi hallita muita maksuttomia. |
| **Office-sovellukset**                         | Käyttäjä ei ole vaikutusta | Käyttäjä ei ole vaikutusta | Office siirtyy rajoitetun toiminnan tilaan.</br> Käyttäjät voivat tarkastella vain tiedostoja. | Office siirtyy rajoitetun toiminnan tilaan.</br> Käyttäjät voivat tarkastella vain tiedostoja. |
| **Cloud services (SharePoint Online, Exchange Online, Skype, työryhmät ja muut)** | Käyttäjä ei ole vaikutusta | Käyttäjä ei ole vaikutusta | Käyttäjät ja järjestelmänvalvojat on pilven ei voi käyttää tietoja. | Asiakkaan tilauksen ja kaikki tiedot poistetaan. |
| **M + S osat** | Admin ei ole vaikutusta</br> Käyttäjä ei ole vaikutusta | Admin ei ole vaikutusta</br> Käyttäjä ei ole vaikutusta | Ominaisuus soveltaminen voidaan panna täytäntöön.</br> Saat lisätietoja [matkaviestimen vaikuttaa enää tilaus](#mobile-device-impacts-upon-subscription-expiration) ja [tilauksen vanhentumisen yhteydessä Windows 10 PC iskut](#windows-10-pc-impacts-upon-subscription-expiration) . | Ominaisuus soveltaminen voidaan panna täytäntöön.</br> Saat lisätietoja [matkaviestimen vaikuttaa enää tilaus](#mobile-device-impacts-upon-subscription-expiration) ja [tilauksen vanhentumisen yhteydessä Windows 10 PC iskut](#windows-10-pc-impacts-upon-subscription-expiration) . |
| **Windows 10-Business** | Admin ei ole vaikutusta</br> Käyttäjä ei ole vaikutusta | Admin ei ole vaikutusta</br> Käyttäjä ei ole vaikutusta | Ominaisuus soveltaminen voidaan panna täytäntöön.</br> Saat lisätietoja [matkaviestimen vaikuttaa enää tilaus](#mobile-device-impacts-upon-subscription-expiration) ja [tilauksen vanhentumisen yhteydessä Windows 10 PC iskut](#windows-10-pc-impacts-upon-subscription-expiration) . | Ominaisuus soveltaminen voidaan panna täytäntöön.</br> Saat lisätietoja [matkaviestimen vaikuttaa enää tilaus](#mobile-device-impacts-upon-subscription-expiration) ja [tilauksen vanhentumisen yhteydessä Windows 10 PC iskut](#windows-10-pc-impacts-upon-subscription-expiration) . |
| **Azure AD kirjautuminen Windows 10-PC** | Admin ei ole vaikutusta</br> Käyttäjä ei ole vaikutusta | Admin ei ole vaikutusta</br> Käyttäjä ei ole vaikutusta | Admin ei ole vaikutusta</br> Käyttäjä ei ole vaikutusta | Kun vuokralaisen on poistettu, käyttäjä voi kirjautua sisään paikalliset tunnistetiedot. Kuvan laite uudelleen, jos paikallinen tunnistetietoja. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Kannettava laite vaikuttaa tilauksen vanhentumisen jälkeen

Followint-taulukossa on yhteenveto app hallintakäytäntöjä kannettavien laitteiden vaikutus.

|                            | Täysin lisensoitu kokemus                      | T + 60 päivää kirjaa vanheneminen          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Passiivinen laite Työtiedostojen poistaminen** | Työn tiedostot poistetaan, kun valitut päivät | Työn tiedostot säilyvät käyttäjän henkilökohtaisten laitteiden |
| **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** | Työtä tiedostoja voi tallentaa vain yrityksen OneDrive | Työn tiedostot voidaan tallentaa mihin tahansa |
| **Salaa työtiedostot** | Työn tiedostot salataan. | Työtiedostojen ei enää ole salattu.</br> Käytännöt poistetaan ja tiedot Office-sovellukset on poistettu. |
| **Pyydä PIN-tunnus tai fingerprint käyttämään Office-sovellukset** | Rajoitettu pääsy apps | Ei ole app tason käyttöoikeuksien rajoittaminen |
| **Vaihda PIN-koodi, kun kirjautuminen epäonnistuu.** | Rajoitettu pääsy apps | Ei ole app tason käyttöoikeuksien rajoittaminen |
| **Vaadi käyttäjiä kirjautumaan uudelleen sen jälkeen, kun Office-sovellukset on ollut käyttämättömänä** | -Kirjautuminen vaaditaan | Ei-Kirjautuminen vaaditaan käyttämään apps |
| **Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu** | Työ-tiedostoja ei voi käyttää jailbroken tai vartteita laitteet | Työ-tiedostoja voidaan käyttää jailbroken tai vartteita laitteet |
| **Salli käyttäjille sisällön kopioiminen omat sovellukset Office-sovellukset** | Kopioi/Liitä rajoitettu apps käytettävissä osana Microsoft 365 Business-tilaus | Kopioi/Liitä kaikki apps käytettävissä |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Windows 10 PC iskut tilauksen vanhentumisen jälkeen

Seuraavassa taulukossa on esitetty Windows 10 laitteen kokoonpanon politiikan vaikutuksia.

|                            | Täysin lisensoitu kokemus                      | T + 60 päivää kirjaa vanheneminen          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Suojaa PCs uhat Windows Defenderin käyttäminen** | Ota käyttöön tai poistaa sen käytöstä on ulkopuolella käyttäjän ohjausobjekti | Ottaa tai poistaa sen käytöstä Windows Defender Windows 10 PC: n käyttäjä |
| **Auta suojaamaan tietokoneita verkkopohjaisilta uhilta Microsoft Edgessä** | Microsoft Edge PC suojelua | Käyttäjä voi ottaa käytössä/ei käytössä Microsoft Edge PC suojelua |
| **Sammuta laite-näyttö Kun kone on vapaa** | Järjestelmänvalvoja määrittää näytön aikakatkaisu väli-käytäntö | Käyttäjä voi määrittää näytön aikakatkaisu |
| **Salli käyttäjille sovellusten lataaminen Microsoft Storesta** | Jos käyttäjä voi ladata apps Microsoft Store määrittää Admin | Käyttäjä voi ladata apps Microsoft Store anytime |
| **Salli käyttäjien käyttää Cortanaa** | Järjestelmänvalvoja määrittää käytännön Cortana käyttöoikeudet | Voit ottaa käyttöön ja poistaa käytöstä Cortana käyttäjän laitteiden |
| **Käyttäjät voivat saada vinkkejä ja ilmoituksia Microsoftilta** | Admin käyttäjä määrittää käytännön vinkkejä ja mainoksia saada Microsoftilta | Käyttäjä saattaa sammua ja vinkkejä ja ilmoituksia Microsoftilta |
| **Salli käyttäjille sisällön kopiointi Office-sovelluksista henkilökohtaisiin sovelluksiin** | Järjestelmänvalvoja määrittää käytännön, joka pitää ajan tasalla Windows 10-laitteet | Käyttäjät voivat päättää, milloin Windows päivittää |




