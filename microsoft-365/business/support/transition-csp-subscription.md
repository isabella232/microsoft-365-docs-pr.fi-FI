---
title: Microsoft 365 BusinessIn CSP-tilauksen siirtyminen
description: Lue, miten voit siirtää Microsoft 365 Business CSP -tilauksen esikatselusta yleiseen saatavuuteen (GA).
author: jasongroce
f1.keywords:
- NOCSH
ms.custom:
- seo-marvel-mar
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Business- ja Microsoft 365-, SMB- ja siirtymäcsp-tilaus
ms.date: 11/01/2017
ms.openlocfilehash: da56ce5bc70dfed5a3e86c739ef3c940b4ac1511
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43635060"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Microsoft 365 BusinessIn CSP-tilauksen siirtyminen

Jos sinulla on Microsoft 365 Business Preview CSP -tilaus, lue tästä oppaasta, miten voit siirtää nykyisen esikatselutilauksesi Microsoft 365 Business GA:han (yleinen saatavuus).

**Esikatselutilauksen siirtyminen GA:ksi**

1. Kirjaudu <a href="https://partnercenter.microsoft.com" target="_blank">kumppanikeskukseen</a>.
2. Valitse koontinäytössä **Asiakkaat**ja etsi ja valitse yrityksen nimi.

    Yhtiön tilaukset listataan.

    ![Asiakkaan tilaukset Kumppanikeskuksessa](../../media/pc_customer_subscriptions_1.png)
    
3. Valitse yrityksen **Tilaukset-sivulla** Lisää **tilaus**.
4. Valitse **Uusi tilaus -sivulla** **Small business (Pienyritys)** ja valitse sitten luettelosta **Microsoft 365 Business.**
5. Lisää käyttöoikeuksien määrä ja valitse sitten **Seuraava: Tarkista,** jos haluat tarkastella tilausta, ja valitse sitten **Lähetä**.

    ![Microsoft 365 Businessin uuden tilauksen tarkistaminen](../../media/pc_customer_reviewnewsubscription.png)

    **Käyttöoikeuspohjaisissa tilauksissa** näkyy **Microsoft 365 Business Preview** ja Microsoft **365 Business**. Keskeytät Preview-tilauksen seuraavaksi.

6. Valitse **Microsoft 365 Business Preview**.
7. Keskeytä **Preview-tilaus valitsemalla Microsoft 365 Business Preview** **(Keskeytä)** -sivulla Keskeytetty.

    ![Microsoft 365 Business Preview -tilauksen keskeyttäminen](../../media/pc_customer_m365bpreview_suspend.png)

8. Vahvista valitsemalla **Lähetä.**

    Vahvista **Tilaukset-sivulla,** että **Microsoft 365 Business Preview -tilassa** näkyy **Keskeytetty**.

    ![Vahvista, että tilauksen esikatselutila on keskeytetty](../../media/pc_customer_m365bpreview_suspend_confirm.png)

9. Vaihtoehtoisesti voit myös vahvistaa käyttöoikeussopimuksen. Voit tehdä tämän seuraavasti:
    1. Valitse yrityksen **Tilaukset-sivulta** **Käyttäjät ja käyttöoikeudet.**
    2. Valitse **käyttäjä Käyttäjät ja käyttöoikeudet** -sivulla.
    3. Tarkista käyttäjän sivulla **Käyttöoikeuksien määrittäminen** -osa ja vahvista, että siinä näkyy **Microsoft 365 Business**.

        ![Vahvista, että Microsoft 365 Business -käyttöoikeus on määritetty käyttäjälle](../../media/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Vaikutus asiakkaisiin ja käyttäjiin siirtymisen aikana ja sen jälkeen

Asiakkaat ja käyttäjät eivät vaikuta haitalliseen siirtymisen ja siirtymisen aikana.

## <a name="impact-to-customers-who-dont-transition"></a>Vaikutus asiakkaisiin, jotka eivät siirry

Seuraavassa taulukossa on yhteenveto vaikutuksista asiakkaisiin, jotka eivät siirry Microsoft 365 Business Preview -tilauksesta Microsoft 365 Business -tilaukseen.

|       | T-0-T+30     | T+30 – T+60 | T+60 – T+120 | Yli T+120  |
|-------|-----------------|--------------|---------------|---------------|
| **Valtion** | Lisäaikana | Vanhentunut      | Poistettu käytöstä      | Deprovisioned (Deprovisioned) |
| **Palvelun vaikutukset**                                                        |
| **Microsoft 365 Business -hallintaportaali** | Ei vaikutusta toiminnallisuuteen | Ei vaikutusta toiminnallisuuteen | Voi lisätä / poistaa käyttäjiä, ostaa tilauksia.</br> Käyttöoikeuksia ei voi määrittää tai peruuttaa. | Asiakkaan tilaus ja kaikki tiedot poistetaan. Järjestelmänvalvoja voi hallita muita maksullisia tilauksia. |
| **Office-sovellukset**                         | Ei loppukäyttäjän vaikutusta | Ei loppukäyttäjän vaikutusta | Office siirtyy rajoitetun toiminnan tilaan.</br> Käyttäjät voivat tarkastella vain tiedostoja. | Office siirtyy rajoitetun toiminnan tilaan.</br> Käyttäjät voivat tarkastella vain tiedostoja. |
| **Pilvipalvelut (SharePoint Online, Exchange Online, Skype, Teams ja paljon muuta)** | Ei loppukäyttäjän vaikutusta | Ei loppukäyttäjän vaikutusta | Loppukäyttäjät ja järjestelmänvalvojat eivät voi käyttää pilvitietoja. | Asiakkaan tilaus ja kaikki tiedot poistetaan. |
| **EM+S-komponentit** | Ei admin vaikutus</br> Ei loppukäyttäjän vaikutusta | Ei admin vaikutus</br> Ei loppukäyttäjän vaikutusta | Kapasiteettia ei enää panna täytäntöön.</br> Lisätietoja on [ohjeaiheessa Mobiililaitteen vaikutukset tilauksen vanhenemisen yhteydessä](#mobile-device-impacts-upon-subscription-expiration) ja [Windows 10 -tietokoneen vaikutukset tilauksen vanhentumisen yhteydessä.](#windows-10-pc-impacts-upon-subscription-expiration) | Kapasiteettia ei enää panna täytäntöön.</br> Lisätietoja on [ohjeaiheessa Mobiililaitteen vaikutukset tilauksen vanhenemisen yhteydessä](#mobile-device-impacts-upon-subscription-expiration) ja [Windows 10 -tietokoneen vaikutukset tilauksen vanhentumisen yhteydessä.](#windows-10-pc-impacts-upon-subscription-expiration) |
| **Windows 10 -liiketoiminta** | Ei admin vaikutus</br> Ei loppukäyttäjän vaikutusta | Ei admin vaikutus</br> Ei loppukäyttäjän vaikutusta | Kapasiteettia ei enää panna täytäntöön.</br> Lisätietoja on [ohjeaiheessa Mobiililaitteen vaikutukset tilauksen vanhenemisen yhteydessä](#mobile-device-impacts-upon-subscription-expiration) ja [Windows 10 -tietokoneen vaikutukset tilauksen vanhentumisen yhteydessä.](#windows-10-pc-impacts-upon-subscription-expiration) | Kapasiteettia ei enää panna täytäntöön.</br> Lisätietoja on [ohjeaiheessa Mobiililaitteen vaikutukset tilauksen vanhenemisen yhteydessä](#mobile-device-impacts-upon-subscription-expiration) ja [Windows 10 -tietokoneen vaikutukset tilauksen vanhentumisen yhteydessä.](#windows-10-pc-impacts-upon-subscription-expiration) |
| **Azure AD -kirjautuminen Windows 10 -tietokoneeseen** | Ei admin vaikutus</br> Ei loppukäyttäjän vaikutusta | Ei admin vaikutus</br> Ei loppukäyttäjän vaikutusta | Ei admin vaikutus</br> Ei loppukäyttäjän vaikutusta | Kun vuokraaja on poistettu, käyttäjä voi kirjautua sisään vain paikallisilla tunnistetiedoilla. Kuvaanlaite uudelleen, jos paikallisia tunnistetietoja ei ole. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Mobiililaitteen vaikutukset tilauksen erääntyessä

Seuraavassa taulukossa on yhteenveto mobiililaitteiden sovellusten hallintakäytäntöjen vaikutuksista.

|                            | Täysin lisensoitu kokemus                      | T + 60 päivää päättymisen jälkeen          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Työtiedostojen poistaminen passiivisesta laitteesta** | Työtiedostot poistetaan valittujen päivien jälkeen | Työtiedostot säilyvät käyttäjän henkilökohtaisissa laitteissa |
| **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** | Työtiedostot voidaan tallentaa vain OneDrive for Businessiin | Työtiedostot voidaan tallentaa mihin tahansa |
| **Salaa työtiedostot** | Työtiedostot salataan | Työtiedostoja ei enää salata.</br> Suojauskäytännöt poistetaan ja sovellusten Office-tiedot poistetaan. |
| **Vaadi PIN-koodi tai sormenjälki Office-sovellusten käyttämiseen** | Rajoitettu pääsy sovelluksiin | Ei sovellustason käyttöoikeusrajoituksia |
| **Pin-koodin nollaaminen, kun kirjautuminen epäonnistuu** | Rajoitettu pääsy sovelluksiin | Ei sovellustason käyttöoikeusrajoituksia |
| **Käyttäjien vaatiminen kirjautumaan uudelleen sisään, kun Office-sovellukset ovat olleet käyttämättömänä** | Kirjautuminen vaaditaan | Sisäänkirjautumista ei tarvita |
| **Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu** | Työtiedostoja ei voi käyttää jailbroken/rooted-laitteissa | Työtiedostoja voi käyttää jailbroken/rooted-laitteissa |
| **Salli käyttäjien kopioida sisältöä Office-sovelluksista Personal-sovelluksiin** | Kopioi tai liitä vain Microsoft 365 -tilauksen osana saatavilla oleviin sovelluksiin | Kopioi /liitä kaikkien sovellusten käytettävissä |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Windows 10 -tietokoneen vaikutukset tilauksen vanhentumisen yhteydessä

Seuraavassa taulukossa on yhteenveto Windows 10 -laitteen määrityskäytäntöihin kohdistuvista vaikutuksista.

|                            | Täysin lisensoitu kokemus                      | T + 60 päivää päättymisen jälkeen          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Suojaa tietokoneita uhkilta Windows Defenderin avulla** | Päälle/pois päältä ei ole käyttäjän hallinnassa | Käyttäjä kanisteri hapantua model after/ lähettää Akkuna Puoltaa model after Akkuna 10 PC |
| **Auta suojaamaan tietokoneitasi verkkopohjaisilta uhkilta Microsoft Edgessä** | Tietokoneen suojaus Microsoft Edgessä | Käyttäjä kanisteri hapantua model after/ lähettää PC suojelus kotona Mikroskooppi Hioa |
| **Laitteen näytön poistaminen käytöstä käyttämättömänä** | Järjestelmänvalvoja määrittää näytön aikakatkaisuvälin käytännön | Käyttäjän voi määrittää näytön aikakatkaisun |
| **Salli käyttäjille sovellusten lataaminen Microsoft Storesta** | Järjestelmänvalvoja määrittää, voiko käyttäjä ladata sovelluksia Microsoft Storesta | Käyttäjä voi ladata sovelluksia Microsoft Storesta milloin tahansa |
| **Salli käyttäjien käyttää Cortanaa** | Järjestelmänvalvoja määrittää käytännön, joka perustuu Cortanan käyttöön | Cortanan ottaminen käyttöön ja poistaminen käytöstä |
| **Salli käyttäjien vastaanottaa vinkkejä ja mainoksia Microsoftilta** | Admin määrittää käytännön käyttäjien vastaanottaa vinkkejä ja mainoksia Microsoftilta | Käyttäjä kanisteri hapantua model after/ lähettää tips ja ilmoitus polveutua Mikroskooppi |
| **Salli käyttäjille sisällön kopiointi Office-sovelluksista henkilökohtaisiin sovelluksiin** | Järjestelmänvalvoja määrittää käytännön, joka pitää Windows 10 -laitteet ajan tasalla | Käyttäjät voivat päättää, milloin Windows päivitetään |
