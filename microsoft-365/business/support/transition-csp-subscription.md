---
title: Microsoft 365 Business CSP-tila uksen siirtymä 
description: Selvitä, miten voit siirtyä Microsoft 365 Business CSP-tila ukseen esikatselusta GA-kohteeseen. 
author: jasongroce
f1.keywords:
- NOCSH
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Business, Microsoft 365, SMB, Transition CSP-tilaus
ms.date: 11/01/2017
ms.openlocfilehash: 4aadfa24bec8728c7e011ac6da48a8e30516e145
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2020
ms.locfileid: "41595041"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Microsoft 365 Business CSP-tila uksen siirtymä

Jos sinulla on Microsoft 365 Business Preview CSP-tilaus, seuraa tätä ohjetta ja selvitä, miten voit siirtyä nykyisen esikatselutilauksen Microsoft 365 Business GA (yleinen saatavuus).

**Esikatselun tila uksen siirtyminen GA-kohteeseen**

1. Kirjaudu sisään <a href="https://partnercenter.microsoft.com" target="_blank">kumppani keskukseen</a>.
2. Valitse koonti näytöstä **Asiakkaat**ja Etsi ja valitse sitten yrityksen nimi.

    Yrityksen tila ukset näkyvät luettelossa.

    ![Asiakkaan tila ukset kumppani keskuksessa](images/pc_customer_subscriptions_1.png)
    
3. Valitse yrityksen **tila ukset** -sivulla **Lisää tilaus**.
4. Valitse **uusi tilaus** -sivulla **Small Business** ja valitse sitten luettelosta **Microsoft 365 Business** .
5. Lisää käyttö oikeuksien määrä ja valitse sitten **Seuraava:** Tarkista tilaus ja valitse sitten **Lähetä**.

    ![Tarkista uusi Microsoft 365 Business-tilaus](images/pc_customer_reviewnewsubscription.png)

    **Lisenssille perustuvat tila ukset** näyttävät **Microsoft 365 Business Preview** -ja **Microsoft 365 Business**-käyttö oikeudet. Keskeytät esikatselun tila uksen seuraavaksi.

6. Valitse **Microsoft 365 Business Preview**.
7. Keskeytä esikatselun tilaus valitsemalla **Microsoft 365 Business Preview** -sivulla **keskeytetty** .

    ![Keskeytä Microsoft 365 Business Preview-tilaus](images/pc_customer_m365bpreview_suspend.png)

8. Vahvista valinta valitsemalla **Lähetä** .

    Vahvista **tila ukset** -sivulla, että **Microsoft 365-yrityksen esikatselutila** näkyy **keskeytettynä**.

    ![Vahvista tila uksen esikatselun tila on keskeytetty](images/pc_customer_m365bpreview_suspend_confirm.png)

9. Vaihtoehtoisesti voit myös tarkistaa käyttö oikeus sopimuksen. Voit tehdä tämän seuraavasti:
    1. Valitse **käyttäjät ja lisenssit** yrityksen **tila ukset** -sivulta.
    2. Valitse käyttäjä **käyttäjät ja lisenssit** -sivulla.
    3. Valitse käyttäjän sivulla **Määritä lisenssit** -osa ja vahvista, että se näyttää **Microsoft 365-liike toiminnan**.

        ![Vahvista, että Microsoft 365 Business License-käyttö oikeus on määritetty käyttäjälle](images/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Vaikutus asiakkaisiin ja käyttäjiin siirtymisen aikana ja sen jälkeen

Ei ole vaikutusta asiakkaisiin ja käyttäjiin siirtymisen ja post-siirtymisen aikana.

## <a name="impact-to-customers-who-dont-transition"></a>Vaikutus asiakkaisiin, jotka eivät ole siirtymässä

Seuraavassa taulukossa on yhteenveto vaikutuksista asiakkaisiin, jotka eivät siirry Microsoft 365 Business Preview-tila uksesta Microsoft 365 Business-tila ukseen.

|       | T-0 – T + 30     | T + 30-T + 60 | T + 60-T + 120 | Beyond T + 120  |
|-------|-----------------|--------------|---------------|---------------|
| **Valtion** | Jatko ajalla | Vanhentunut      | Poistettu käytöstä      | Deprovisioned |
| **Palvelun vaikutukset**                                                        |
| **Microsoft 365 Business-hallinta portaali** | Ei vaikutusta toiminnallisuuteen | Ei vaikutusta toiminnallisuuteen | Voit lisätä tai poistaa käyttäjiä, ostaa tila uksia.</br> Käyttö oikeuksia ei voi määrittää tai kumota. | Asiakkaan tilaus ja kaikki tiedot poistetaan. Järjestelmänvalvoja voi hallita muita maksullisia tila uksia. |
| **Office-sovellukset**                         | Loppu käyttäjän vaikutusta ei ole | Loppu käyttäjän vaikutusta ei ole | Office siirtyy rajoitetun toiminnan tilaan.</br> Käyttäjät voivat tarkastella vain tiedostoja. | Office siirtyy rajoitetun toiminnan tilaan.</br> Käyttäjät voivat tarkastella vain tiedostoja. |
| **Pilvi palvelut (SharePoint Online, Exchange Online, Skype, teams ja muut)** | Loppu käyttäjän vaikutusta ei ole | Loppu käyttäjän vaikutusta ei ole | Loppu käyttäjillä ja ylläpitäjät eivät pääse käyttämään tietoja pilvi palvelussa. | Asiakkaan tilaus ja kaikki tiedot poistetaan. |
| **EM + S-komponentit** | Ei järjestelmänvalvojan vaikutusta</br> Loppu käyttäjän vaikutusta ei ole | Ei järjestelmänvalvojan vaikutusta</br> Loppu käyttäjän vaikutusta ei ole | Ominaisuutta ei enää valvota.</br> Katso lisä tietoja [mobiililaitteen vaikutuksesta tila uksen vanhenemisen yhteydessä](#mobile-device-impacts-upon-subscription-expiration) ja [Windows 10-tieto koneen vaikutuksesta tila uksen vanhenemisen yhteydessä](#windows-10-pc-impacts-upon-subscription-expiration) . | Ominaisuutta ei enää valvota.</br> Katso lisä tietoja [mobiililaitteen vaikutuksesta tila uksen vanhenemisen yhteydessä](#mobile-device-impacts-upon-subscription-expiration) ja [Windows 10-tieto koneen vaikutuksesta tila uksen vanhenemisen yhteydessä](#windows-10-pc-impacts-upon-subscription-expiration) . |
| **Windows 10 Business** | Ei järjestelmänvalvojan vaikutusta</br> Loppu käyttäjän vaikutusta ei ole | Ei järjestelmänvalvojan vaikutusta</br> Loppu käyttäjän vaikutusta ei ole | Ominaisuutta ei enää valvota.</br> Katso lisä tietoja [mobiililaitteen vaikutuksesta tila uksen vanhenemisen yhteydessä](#mobile-device-impacts-upon-subscription-expiration) ja [Windows 10-tieto koneen vaikutuksesta tila uksen vanhenemisen yhteydessä](#windows-10-pc-impacts-upon-subscription-expiration) . | Ominaisuutta ei enää valvota.</br> Katso lisä tietoja [mobiililaitteen vaikutuksesta tila uksen vanhenemisen yhteydessä](#mobile-device-impacts-upon-subscription-expiration) ja [Windows 10-tieto koneen vaikutuksesta tila uksen vanhenemisen yhteydessä](#windows-10-pc-impacts-upon-subscription-expiration) . |
| **Azure AD Kirjaudu Windows 10-tieto koneeseen** | Ei järjestelmänvalvojan vaikutusta</br> Loppu käyttäjän vaikutusta ei ole | Ei järjestelmänvalvojan vaikutusta</br> Loppu käyttäjän vaikutusta ei ole | Ei järjestelmänvalvojan vaikutusta</br> Loppu käyttäjän vaikutusta ei ole | Kun vuokraaja on poistettu, käyttäjä voi kirja utua sisään vain paikallisilla tunniste tiedoilla. Kuvaa laite uudelleen, jos paikallisia tunniste tietoja ei ole. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Mobiililaite vaikuttaa tila uksen vanhenemisen yhteydessä

Seuraavassa taulukossa on yhteenveto sovellusten hallinta käytäntöjen vaikutuksesta mobiililaitteissa.

|                            | Täysin lisensoitu kokemus                      | T + 60 päivää julkaisun vanheneminen          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Työtiedostojen poistaminen passiivisessa laitteessa** | Työtiedostot poistetaan valittujen päivien jälkeen | Työtiedostot pysyvät käyttäjän henkilökohtaisissa laitteissa |
| **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** | Työtiedostot voidaan tallentaa vain OneDrive for Businessille | Työtiedostot voidaan tallentaa minne tahansa |
| **Salaa työtiedostot** | Työtiedostot on salattu | Työtiedostoja ei enää salata.</br> Suojaus käytännöt poistetaan, ja sovellusten Office-tiedot poistetaan. |
| **Vaadi PIN-koodi tai sormen jälki Office-sovellusten käytön** | Rajoitettu pääsy sovelluksiin | Ei sovellus tason käyttö rajoituksia |
| **Nollaa PIN kun kirjautuminen epäonnistuu** | Rajoitettu pääsy sovelluksiin | Ei sovellus tason käyttö rajoituksia |
| **Vaadi käyttäjiä Kirjautu maan uudelleen sisään, kun Office-sovellukset ovat olleet käyttämättömänä** | Kirjautuminen pakollinen | Kirjautumista ei vaadita |
| **Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu** | Työtiedostoja ei voi käyttää jailbroken/juurtuneet laitteet | Työtiedostot voidaan käyttää jailbroken/juurtunut laitteisiin |
| **Salli käyttäjien kopioida sisältöä Office-sovelluksista omiin sovelluksiin** | Kopioi/Liitä rajoitettu sovelluksiin, jotka ovat saatavilla osana Microsoft 365 Business-tilausta | Kopioi/Liitä kaikkien sovellusten käytettävissä |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Windows 10-tieto kone vaikuttaa tila uksen vanhenemisen yhteydessä

Seuraavassa taulukossa on yhteenveto Windows 10-laitteen kokoonpano käytäntöihin vaikuttavaan vaikutukseen.

|                            | Täysin lisensoitu kokemus                      | T + 60 päivää julkaisun vanheneminen          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Suojaa tieto koneita uhkilta Windows Defenderin avulla** | Päälle/pois päältä on käyttäjän ohja uksen ulkopuolella | Käyttäjä voi kytkeä päälle/pois Windows Defender Windows 10 PC |
| **Auta suojaamaan tietokoneitasi verkkopohjaisilta uhkilta Microsoft Edgessä** | Tieto koneen suojaus Microsoft Edgessä | Käyttäjä voi kytkeä päälle/pois PC suojaus Microsoft Edge |
| **Sammuta laitteen näyttö, kun se on käyttämättömänä** | Järjestelmänvalvoja määrittää näytön aika katkaisu välin käytännön | Loppu käyttäjä voi määrittää näytön aika katkaisun |
| **Salli käyttäjille sovellusten lataaminen Microsoft Storesta** | Järjestelmänvalvoja määrittää, voiko käyttäjä ladata sovelluksia Microsoft Storesta | Käyttäjä voi ladata sovelluksia Microsoft Storesta milloin tahansa |
| **Salli käyttäjien käyttää Cortanaa** | Järjestelmänvalvoja määrittää Cortanan käyttö oikeus käytännön | Cortana-toiminnon päälle/pois päältä |
| **Salli käyttäjien vastaanottaa vihjeitä ja mainoksia Microsoftilta** | Järjestelmänvalvoja määrittää käytännön käyttäjälle vastaanota vihjeitä ja mainoksia Microsoftilta | Käyttäjä voi ottaa käyttöön/poistaa käytöstä vihjeitä ja mainoksia Microsoftilta |
| **Salli käyttäjille sisällön kopiointi Office-sovelluksista henkilökohtaisiin sovelluksiin** | Järjestelmänvalvoja määrittelee käytännön, joka pitää Windows 10-laitteet ajan tasalla | Käyttäjät voivat päättää, milloin Windows päivitetään |
