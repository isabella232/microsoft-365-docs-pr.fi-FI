---
title: Microsoft 365 Business CSP -tilauksen siirtyminen
description: Katso, miten voit siirtyä Microsoft 365 Business CSP -tilauksesta esikatselusta yleiseen käytettävyseen (GA).
author: jasongroce
f1.keywords:
- NOCSH
ms.custom:
- seo-marvel-mar
- AdminSurgePortfolio
ms.author: jasongroce
ms.topic: article
manager: jasonh
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business
keywords: Microsoft 365 Business-, Microsoft 365-, SMB- ja siirtymä-CSP-tilaus
ms.date: 11/01/2017
ms.openlocfilehash: c35cb3b78c4fe2cebc8308b34ceef3decd346b3db298ce5fb56abc8cf205e69d
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53867120"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Microsoft 365 Business CSP -tilauksen siirtyminen

Jos käytössäsi on Microsoft 365 Business Preview -palvelun CSP-tilaus, katso tästä oppaasta, miten voit muuttaa nykyisen esikatselutilauksesi Microsoft 365 Business GA:een (yleinen saatavuus).

**Esikatselutilauksen siirtyminen GA-tilaukseen**

1. Kirjaudu <a href="https://partnercenter.microsoft.com" target="_blank">kumppanikeskukseen.</a>
2. Valitse koontinäytössä **Asiakkaat** ja etsi ja valitse yrityksen nimi.

    Yrityksen tilaukset näkyvät luettelossa.

    ![Asiakkaan tilaukset kumppanikeskuksessa](../../media/pc_customer_subscriptions_1.png)
    
3. Valitse yrityksen **Tilaukset-sivulla** Lisää **tilaus**.
4. Valitse Uusi **tilaus** -sivulla **Pienyritys** ja valitse Microsoft 365 **Business** luettelosta.
5. Lisää käyttöoikeuksien määrä ja tarkista tilaus **valitsemalla Seuraava:** Tarkista ja valitse sitten **Lähetä**.

    ![Microsoft 365 Businessin uuden tilauksen tarkistaminen](../../media/pc_customer_reviewnewsubscription.png)

    **Käyttöoikeuspohjaiset tilaukset näyttävät** Microsoft 365 **Business Preview-** ja **Microsoft 365 Business -tilaukset.** Voit keskeyttää Preview-tilauksen seuraavan kerran.

6. Valitse **Microsoft 365 Business Preview**.
7. Valitse **Microsoft 365 Business Preview -sivulla** **Keskeytetty,** jos haluat keskeyttää Preview-tilauksen.

    ![Microsoft 365 Business Preview -tilauksen keskeyttäminen](../../media/pc_customer_m365bpreview_suspend.png)

8. Vahvista **valitsemalla** Lähetä.

    Varmista **Tilaukset-sivulla,** että **Microsoft 365 Business Preview 'n tila** on **Keskeytetty**.

    ![Varmista, että Preview-tilauksen tila on keskeytetty](../../media/pc_customer_m365bpreview_suspend_confirm.png)

9. Vaihtoehtoisesti voit myös vahvistaa käyttöoikeussopimuksen. Voit tehdä tämän seuraavasti:
    1. Valitse **Käyttäjät ja käyttöoikeudet** yrityksen Tilaukset-sivulta. 
    2. Valitse **käyttäjä Käyttäjät ja käyttöoikeudet** -sivulla.
    3. Valitse käyttäjän sivulla Määritä käyttöoikeudet  -osa ja varmista, että siinä näkyy Microsoft 365 **Business.**

        ![Vahvista Microsoft 365 että käyttäjälle on määritetty Business-käyttöoikeus](../../media/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Vaikutus asiakkaisiin ja käyttäjiin siirtymisen aikana ja sen jälkeen

Siirtymän ja siirtymisen aikana ei ole vaikutusta asiakkaisiin ja käyttäjiin.

## <a name="impact-to-customers-who-dont-transition"></a>Vaikutus asiakkaisiin, jotka eivät siirry

Seuraavassa taulukossa on yhteenveto vaikutuksista asiakkaisiin, jotka eivät siirry Microsoft 365 Business Preview -tilauksesta Microsoft 365 Business -tilaukseen.

|       | T-0 –T+30     | T+30 – T+60 | T+60 – T+120 | T+120:n jälkeen  |
|-------|-----------------|--------------|---------------|---------------|
| **Osavaltio** | Lisäajan aikana | Vanhentunut      | Ei käytössä      | Purettu |
| **Palvelun vaikutukset**                                                        |
| **Microsoft 365 -hallintakeskus** | Ei vaikutusta toimintoihin | Ei vaikutusta toimintoihin | Voi lisätä tai poistaa käyttäjiä, ostaa tilauksia.</br> Käyttöoikeuksia ei voi määrittää tai kumota. | Asiakkaan tilaus ja kaikki tiedot poistetaan. Järjestelmänvalvoja voi hallita muita maksullisia tilauksia. |
| **Office-sovellukset**                         | Ei loppukäyttäjien vaikutusta | Ei loppukäyttäjien vaikutusta | Office siirtyy rajoitetun toiminnan tilaan.</br> Käyttäjät voivat vain tarkastella tiedostoja. | Office siirtyy rajoitetun toiminnan tilaan.</br> Käyttäjät voivat vain tarkastella tiedostoja. |
| **Pilvipalvelut (SharePoint Online, Exchange Online, Skype, Teams ja paljon muuta)** | Ei loppukäyttäjien vaikutusta | Ei loppukäyttäjien vaikutusta | Loppukäyttäjillä ja järjestelmänvalvojilla ei ole pääsyä pilvipalvelun tietoihin. | Asiakkaan tilaus ja kaikki tiedot poistetaan. |
| **EM+S-osat** | Ei järjestelmänvalvojan vaikutusta</br> Ei loppukäyttäjien vaikutusta | Ei järjestelmänvalvojan vaikutusta</br> Ei loppukäyttäjien vaikutusta | Ominaisuus ei ole enää pakotettu.</br> Lisätietoja [on kohdassa Mobiililaite vaikuttaa tilauksen](#mobile-device-impacts-upon-subscription-expiration) Windows 10 ja tietokone vaikuttaa [tilauksen](#windows-10-pc-impacts-upon-subscription-expiration) vanhenemiseen. | Ominaisuus ei ole enää pakotettu.</br> Lisätietoja [on kohdassa Mobiililaite vaikuttaa tilauksen](#mobile-device-impacts-upon-subscription-expiration) Windows 10 ja tietokone vaikuttaa [tilauksen](#windows-10-pc-impacts-upon-subscription-expiration) vanhenemiseen. |
| **Windows 10 Business** | Ei järjestelmänvalvojan vaikutusta</br> Ei loppukäyttäjien vaikutusta | Ei järjestelmänvalvojan vaikutusta</br> Ei loppukäyttäjien vaikutusta | Ominaisuus ei ole enää pakotettu.</br> Lisätietoja [on kohdassa Mobiililaite vaikuttaa tilauksen](#mobile-device-impacts-upon-subscription-expiration) Windows 10 ja tietokone vaikuttaa [tilauksen](#windows-10-pc-impacts-upon-subscription-expiration) vanhenemiseen. | Ominaisuus ei ole enää pakotettu.</br> Lisätietoja [on kohdassa Mobiililaite vaikuttaa tilauksen](#mobile-device-impacts-upon-subscription-expiration) Windows 10 ja tietokone vaikuttaa [tilauksen](#windows-10-pc-impacts-upon-subscription-expiration) vanhenemiseen. |
| **Azure AD -kirjautuminen Windows 10 PC:hen** | Ei järjestelmänvalvojan vaikutusta</br> Ei loppukäyttäjien vaikutusta | Ei järjestelmänvalvojan vaikutusta</br> Ei loppukäyttäjien vaikutusta | Ei järjestelmänvalvojan vaikutusta</br> Ei loppukäyttäjien vaikutusta | Kun vuokraaja on poistettu, käyttäjä voi kirjautua sisään vain paikallisilla tunnistetiedoilla. Kuvaa laite uudelleen, jos paikallisia tunnistetietoja ei ole. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Mobiililaite vaikuttaa tilauksen vanhenemiseen

Seuraavassa taulukossa on yhteenveto mobiililaitteiden sovellusten hallintakäytännöistä.

|                            | Käyttöoikeutettu käyttökokemus                      | T+60 päivää vanhenemisen jälkeen          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Työtiedostojen poistaminen passiivisista laitteesta** | Työtiedostot poistetaan valittujen päivien jälkeen | Työtiedostot säilyvät käyttäjän henkilökohtaisissa laitteissa |
| **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** | Työtiedostoja voi tallentaa vain OneDrive for Business | Työtiedostot voidaan tallentaa mihin tahansa |
| **Salaa työtiedostot** | Työtiedostot on salattu | Työtiedostoja ei enää salata.</br> Suojauskäytännöt poistetaan, Office tietoja poistetaan sovelluksista. |
| **Vaadi PIN-koodia tai sormenjälkeä sovellusten Office varten** | Rajoitettu sovellusten käyttö | Ei sovellustason käyttöoikeusrajoitusta |
| **Palauta PIN-koodi, kun kirjautuminen epäonnistuu** | Rajoitettu sovellusten käyttö | Ei sovellustason käyttöoikeusrajoitusta |
| **Vaadi käyttäjiä kirjautumaan uudelleen, kun Office on ollut käyttämättömänä** | Kirjautuminen vaaditaan | Kirjautumista ei tarvita |
| **Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu** | Työtiedostoja ei voi käyttää laitteissa, joissa on murrettu suojaus | Työtiedostoja voi käyttää laitteissa, joissa on murrettu suojaus |
| **Salli käyttäjien kopioida sisältöä Office sovelluksista henkilökohtaisiin sovelluksiin** | Kopiointi ja liittäminen rajoitettu sovelluksiin, jotka ovat Microsoft 365 osana tilausta | Kopioiminen ja liittäminen kaikkien sovellusten käytettävissä |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Windows 10 TIETOKONE vaikuttaa tilauksen vanhenemiseen

Seuraavassa taulukossa on yhteenveto siitä, miten tämä vaikuttaa Windows 10 määrityskäytäntöihin.

|                            | Käyttöoikeutettu käyttökokemus                      | T+60 päivää vanhenemisen jälkeen          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Auta suojaamaan tietokoneita uhkilta Windows Defender** | Turn on /off is outside of user control | Käyttäjä voi ottaa käyttöön tai poistaa Windows Defender tietokoneen Windows 10 käytöstä |
| **Auta suojaamaan tietokoneitasi verkkopohjaisilta uhkilta Microsoft Edgessä** | Tietokoneen suojaus Microsoft Edge | Käyttäjä voi ottaa tietokoneen suojauksen käyttöön tai poistaa sen käytöstä Microsoft Edge |
| **Poista laitteen näyttö käytöstä, kun se on käyttämättömänä** | Järjestelmänvalvoja määrittää näytön aikakatkaisuvälikäytännön | Loppukäyttäjä voi määrittää näytön aikakatkaisun |
| **Salli käyttäjille sovellusten lataaminen Microsoft Storesta** | Järjestelmänvalvoja määrittää, voiko käyttäjä ladata sovelluksia Microsoft Store | Käyttäjä voi ladata sovelluksia Microsoft Store milloin tahansa |
| **Salli käyttäjien käyttää Cortanaa** | Järjestelmänvalvoja määrittää käytännön, joka määrittää käyttäjien Cortana | Käyttäjän laitteet, joiden avulla käyttäjä voi ottaa Cortana |
| **Vihjeiden ja mainosten vastaanottamisen salliminen Microsoftilta** | Järjestelmänvalvoja määrittää käytännön, joka määrittää, miten käyttäjä saa Microsoftilta vihjeitä ja mainoksia | Käyttäjä voi ottaa käyttöön tai poistaa käytöstä Microsoftin vihjeitä ja mainoksia |
| **Salli käyttäjille sisällön kopiointi Office-sovelluksista henkilökohtaisiin sovelluksiin** | Järjestelmänvalvoja määrittää käytännön, joka pitää Windows 10 ajan tasalla | Käyttäjät voivat päättää, milloin Windows |
