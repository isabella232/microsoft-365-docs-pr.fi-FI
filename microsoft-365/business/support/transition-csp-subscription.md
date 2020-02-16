---
title: Microsoft 365 Businessin CSP-tilauksen siirtyminen 
description: Ota selvää, miten voit siirtää Microsoft 365 BusinessCSP -tilauksen esikatselusta ga-tilaukseen. 
author: jasongroce
f1.keywords:
- NOCSH
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Business, Microsoft 365, SMB, siirtymän CSP-tilaus
ms.date: 11/01/2017
ms.openlocfilehash: 7d8e04a0136f86d3c4bb51208081fd1dcbecf59d
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2020
ms.locfileid: "42057202"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Microsoft 365 Businessin CSP-tilauksen siirtyminen

Jos sinulla on Microsoft 365 Business Preview CSP -tilaus, selvitä tämän oppaan ohjeiden mukaan, miten voit siirtää aiemmin luodun esikatselutilauksen Microsoft 365 Business GA:ksi (yleinen saatavuus).

**Esikatselutilauksen siirtyminen ga-tilaukseen**

1. Kirjaudu <a href="https://partnercenter.microsoft.com" target="_blank">kumppanikeskukseen</a>.
2. Valitse koontinäytössä **Asiakkaat**ja etsi ja valitse yrityksen nimi.

    Yhtiön tilaukset listataan.

    ![Asiakkaan tilaukset kumppanikeskuksessa](../../media/pc_customer_subscriptions_1.png)
    
3. Valitse Yrityksen **Tilaukset-sivulla** Lisää **tilaus**.
4. Valitse **Uusi tilaus -sivulla** **Pienyritys** ja valitse sitten luettelosta **Microsoft 365 Business.**
5. Lisää käyttöoikeuksien määrä ja valitse sitten **Seuraava: Tarkista,** jos haluat tarkastella tilausta, ja valitse sitten **Lähetä**.

    ![Microsoft 365 Businessin uuden tilauksen tarkistaminen](../../media/pc_customer_reviewnewsubscription.png)

    **Käyttöoikeuspohjaisissa tilauksissa** näkyvät **Microsoft 365 Business Preview** ja Microsoft **365 Business**. Keskeytät preview-tilauksen seuraavaksi.

6. Valitse **Microsoft 365 Business Preview**.
7. Keskeytä Esikatselutilaus valitsemalla **Microsoft 365 Business Preview** -sivulla **Keskeytetty.**

    ![Microsoft 365 Business Preview -tilauksen keskeyttäminen](../../media/pc_customer_m365bpreview_suspend.png)

8. Vahvista valitsemalla **Lähetä.**

    Varmista **Tilaukset-sivulla,** että **Microsoft 365 Business Preview -tila** näkyy **Keskeytettynä**.

    ![Varmista, että Esikatselutilauksen tila on keskeytetty](../../media/pc_customer_m365bpreview_suspend_confirm.png)

9. Vaihtoehtoisesti voit myös vahvistaa käyttöoikeussopimuksen. Voit tehdä tämän seuraavasti:
    1. Valitse Yrityksen **Tilaukset-sivulta** **Käyttäjät ja käyttöoikeudet.**
    2. Valitse **käyttäjä Käyttäjät ja käyttöoikeudet** -sivulla.
    3. Tarkista käyttäjän sivulla **Käyttöoikeuksien määrittäminen** -osio ja varmista, että siinä näkyy **Microsoft 365 Business**.

        ![Microsoft 365 Business -käyttöoikeuden vahvistaminen on määritetty käyttäjälle](../../media/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Vaikutus asiakkaisiin ja käyttäjiin siirtymisen aikana ja sen jälkeen

Ei ole vaikutusta asiakkaisiin ja käyttäjiin siirtymisen ja post transition.

## <a name="impact-to-customers-who-dont-transition"></a>Vaikutus asiakkaisiin, jotka eivät siirry

Seuraavassa taulukossa on yhteenveto vaikutuksesta asiakkaisiin, jotka eivät siirry Microsoft 365 Business Preview -tilauksesta Microsoft 365 Business -tilaukseen.

|       | T-0–T+30     | T+30–T+60 | T+60–T+120 | Yli T+120  |
|-------|-----------------|--------------|---------------|---------------|
| **Valtion** | Lisäaikana | Vanhentunut      | Poistettu käytöstä      | Deprovisioned |
| **Palvelun vaikutukset**                                                        |
| **Microsoft 365 Business -hallintaportaali** | Ei vaikutusta toiminnallisuuteen | Ei vaikutusta toiminnallisuuteen | Voi lisätä / poistaa käyttäjiä, ostaa tilauksia.</br> Käyttöoikeuksia ei voi määrittää tai peruuttaa. | Asiakkaan tilaus ja kaikki tiedot poistetaan. Järjestelmänvalvoja voi hallita muita maksullisia tilauksia. |
| **Office-sovellukset**                         | Ei loppukäyttäjän vaikutusta | Ei loppukäyttäjän vaikutusta | Office siirtyy rajoitetun toiminnan tilaan.</br> Käyttäjät voivat tarkastella vain tiedostoja. | Office siirtyy rajoitetun toiminnan tilaan.</br> Käyttäjät voivat tarkastella vain tiedostoja. |
| **Pilvipalvelut (SharePoint Online, Exchange Online, Skype, Teams ja paljon muuta)** | Ei loppukäyttäjän vaikutusta | Ei loppukäyttäjän vaikutusta | Loppukäyttäjillä ja järjestelmänvalvojilla ei ole pääsyä pilven tietoihin. | Asiakkaan tilaus ja kaikki tiedot poistetaan. |
| **EM+S-komponentit** | Ei järjestelmänvalvojan vaikutusta</br> Ei loppukäyttäjän vaikutusta | Ei järjestelmänvalvojan vaikutusta</br> Ei loppukäyttäjän vaikutusta | Ominaisuutta ei enää panna täytäntöön.</br> Lisätietoja on [ohjeaiheessa Mobiililaitteen vaikutukset tilauksen vanhenemisen yhteydessä](#mobile-device-impacts-upon-subscription-expiration) ja [Windows 10 PC:n vaikutukset tilauksen vanhenemisen yhteydessä.](#windows-10-pc-impacts-upon-subscription-expiration) | Ominaisuutta ei enää panna täytäntöön.</br> Lisätietoja on [ohjeaiheessa Mobiililaitteen vaikutukset tilauksen vanhenemisen yhteydessä](#mobile-device-impacts-upon-subscription-expiration) ja [Windows 10 PC:n vaikutukset tilauksen vanhenemisen yhteydessä.](#windows-10-pc-impacts-upon-subscription-expiration) |
| **Windows 10 -liiketoiminta** | Ei järjestelmänvalvojan vaikutusta</br> Ei loppukäyttäjän vaikutusta | Ei järjestelmänvalvojan vaikutusta</br> Ei loppukäyttäjän vaikutusta | Ominaisuutta ei enää panna täytäntöön.</br> Lisätietoja on [ohjeaiheessa Mobiililaitteen vaikutukset tilauksen vanhenemisen yhteydessä](#mobile-device-impacts-upon-subscription-expiration) ja [Windows 10 PC:n vaikutukset tilauksen vanhenemisen yhteydessä.](#windows-10-pc-impacts-upon-subscription-expiration) | Ominaisuutta ei enää panna täytäntöön.</br> Lisätietoja on [ohjeaiheessa Mobiililaitteen vaikutukset tilauksen vanhenemisen yhteydessä](#mobile-device-impacts-upon-subscription-expiration) ja [Windows 10 PC:n vaikutukset tilauksen vanhenemisen yhteydessä.](#windows-10-pc-impacts-upon-subscription-expiration) |
| **Azure AD -kirjautuminen Windows 10 -tietokoneeseen** | Ei järjestelmänvalvojan vaikutusta</br> Ei loppukäyttäjän vaikutusta | Ei järjestelmänvalvojan vaikutusta</br> Ei loppukäyttäjän vaikutusta | Ei järjestelmänvalvojan vaikutusta</br> Ei loppukäyttäjän vaikutusta | Kun vuokraajan on poistettu, käyttäjä voi kirjautua sisään vain paikallisilla tunnistetiedoilla. Kuvaa laite uudelleen, jos paikallisia tunnistetietoja ei ole. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Mobiililaitteen vaikutukset tilauksen päättymisen jälkeen

Seuraavassa taulukossa on yhteenveto mobiililaitteiden sovellusten hallintakäytäntöjen vaikutuksesta.

|                            | Täysin lisensoitu kokemus                      | T+60 päivää päättymisen jälkeen          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Työtiedostojen poistaminen passiivisesta laitteesta** | Työtiedostot poistetaan valittujen päivien jälkeen | Työtiedostot säilyvät käyttäjän henkilökohtaisissa laitteissa |
| **Pakota käyttäjät tallentamaan kaikki työtiedostot OneDrive for Businessiin** | Työtiedostot voidaan tallentaa vain OneDrive for Businessiin | Työtiedostoja voidaan tallentaa mihin tahansa |
| **Salaa työtiedostot** | Työtiedostot salataan | Työtiedostoja ei enää salata.</br> Suojauskäytännöt poistetaan ja sovellusten Office-tiedot poistetaan. |
| **Vaadi PIN-koodi tai sormenjälki, jotta voit käyttää Office-sovelluksia** | Sovellusten rajoitettu käyttö | Ei sovellustason käyttörajoitusta |
| **Nollaa PIN-koodi, kun kirjautuminen epäonnistuu** | Sovellusten rajoitettu käyttö | Ei sovellustason käyttörajoitusta |
| **Käyttäjien vaatiminen kirjautumaan uudelleen office-sovellusten käyttämättömänä jälkeen** | Sisäänkirjautuminen vaaditaan | Sisäänkirjautumista ei tarvita |
| **Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu** | Työtiedostoja ei voi käyttää jailbroken/juurtuneilla laitteilla | Työtiedostoja voi käyttää jailbroken / juurtuneet laitteet |
| **Salli käyttäjien kopioida sisältöä Office-sovelluksista henkilökohtaisiin sovelluksiin** | Kopioiminen/liittäminen rajoitettu Microsoft 365 Business -tilauksen osana käytettävissä oleviin sovelluksiin | Kopioi/liitä kaikkien sovellusten käytettävissä |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Windows 10 PC:n vaikutus tilauksen vanhenemisen yhteydessä

Seuraavassa taulukossa on yhteenveto Windows 10 -laitteen määrityskäytäntöjen vaikutuksesta.

|                            | Täysin lisensoitu kokemus                      | T+60 päivää päättymisen jälkeen          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Tietokoneiden suojaaminen uhilta Windows Defenderin avulla** | Ottaminen käyttöön ja poistaminen käytöstä ei kuulu käyttäjän hallintaan | Käyttäjä voi ottaa Windows Defenderin käyttöön tai poistaa sen käytöstä Windows 10 -tietokoneessa |
| **Auta suojaamaan tietokoneitasi verkkopohjaisilta uhkilta Microsoft Edgessä** | Tietokoneen suojaus Microsoft Edgessä | Käyttäjä kanisteri hapantua model after/ lähettää PC suojelus kotona Mikroskooppi Hioa |
| **Laitteen näytön poistaminen käytöstä käyttämättömänä** | Järjestelmänvalvoja määrittää näytön aikakatkaisun aikakatkaisukäytännön | Loppukäyttäjä voi määrittää näytön aikakatkaisun |
| **Salli käyttäjille sovellusten lataaminen Microsoft Storesta** | Järjestelmänvalvoja määrittää, voiko käyttäjä ladata sovelluksia Microsoft Storesta | Käyttäjä voi ladata sovelluksia Microsoft Storesta milloin tahansa |
| **Salli käyttäjien käyttää Cortanaa** | Järjestelmänvalvoja määrittää Cortanan käyttöoikeuksia koskevan käytännön | Cortanan käyttöön ottaminen ja poistaminen käytöstä käyttäjälaitteet |
| **Salli käyttäjien saada vinkkejä ja mainoksia Microsoftilta** | Järjestelmänvalvoja määrittää käytännön, joka koskevat käyttäjien vastaanottovinkkejä ja mainoksia Microsoftilta | Käyttäjä kanisteri hapantua model after/ lähettää tips ja ilmoitus polveutua Mikroskooppi |
| **Salli käyttäjille sisällön kopiointi Office-sovelluksista henkilökohtaisiin sovelluksiin** | Järjestelmänvalvoja määrittää käytännön, joka pitää Windows 10 -laitteet ajan tasalla | Käyttäjät voivat päättää, milloin Windows päivitetään |
