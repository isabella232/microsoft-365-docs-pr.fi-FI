---
title: Tarkista havaittuja uhkia ja toimi
f1.keywords: NOCSH
ms.author: sharik
author: SKjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- Adm_O365
- Adm_TOC
ms.custom: AdminSurgePortfolio
search.appverid: MET150
description: Opi tarkistamaan ja hallitsemaan uhkia, jotka Microsoft Defenderin virustentorjunta tunnistanut Windows 10 laitteissasi.
ms.openlocfilehash: f2edd27c527cc2b9fd8c986191a0bad5c0844da68880f8d8d775491e3480babd
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53882089"
---
# <a name="review-detected-threats-and-take-action"></a>Tarkista havaittuja uhkia ja toimi

Kun haittaohjelma havaitaan, se Microsoft Defenderin virustentorjunta ja estää sen suorittamisen. Kun pilvitallennussuojaus on käytössä, uusia havaittuja uhkia lisätään virusten ja haittaohjelmien torjuntaohjelmaan, jotta myös muut laitteet ja käyttäjät ovat suojattuja.

Microsoft Defenderin virustentorjunta havaitsee ja suojautuu seuraavilla uhilla:

- Virukset, haittaohjelmat ja verkkopohjaiset uhat laitteissa
- Tietojen kalasteluyritykset
- Tietojen varastamisyritykset

IT-ammattilaisena/järjestelmänvalvojana voit tarkastella tietoja uhkien tunnistamisesta kaikissa Windows 10 laitteissa, jotka on rekisteröity [intunessa](/mem/intune/enrollment/device-enrollment) Microsoft 365 -hallintakeskus. Näet yhteenvetotiedot, kuten:

- Kuinka moni laite tarvitsee virustentorjuntaohjelman suojauksen
- Kuinka monta laitetta ei ole tietoturvakäytäntöjen kanssa
- Kuinka monta uhkia on tällä hetkellä aktiivisia, lieventäviä tai ratkaistuja

Voit tarkastella uhkien tunnistuksen ja laitteiden yksityiskohtaisia tietoja useilla eri vaihtoehdoilla:

- Aktiiviset **laitteet** -sivu <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">Microsoft 365 -hallintakeskus.</a> Katso [tämän artikkelin kohta Uhkien tunnistuksen hallinta Aktiiviset](#manage-threat-detections-on-the-active-devices-page) laitteet -sivulla.
- Aktiiviset **uhat** -sivu <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">Microsoft 365 -hallintakeskus.</a> Katso [tämän artikkelin kohta Uhkien tunnistuksen hallinta Aktiiviset](#manage-threat-detections-on-the-active-threats-page) uhat -sivulla.
- **Virustentorjunta-sivu** <a href="https://go.microsoft.com/fwlink/p/?linkid=2150463" target="_blank">Microsoft Endpoint Manager.</a> Katso [tämän artikkelin kohta Microsoft Endpoint Manager](#manage-threat-detections-in-microsoft-endpoint-manager) tunnistuksen hallinta.

Lisätietoja on ohjeaiheessa [Microsoft Defenderin virustentorjunta.](threats-detected-defender-av.md)

## <a name="manage-threat-detections-on-the-active-devices-page"></a>Uhkien tunnistuksen hallinta **Aktiiviset laitteet -sivulla**

Seuraava menettely koskee asiakkaita, joilla on Microsoft 365 Business Premium.

1. Siirry Microsoft 365 -hallintakeskus ja kirjaudu <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> sisään.

2. Valitse siirtymissivulla Laitteet  >  **Aktiiviset laitteet**. Näet luettelon aktiivisista laitteista ja yksityiskohdista, kuten suojauksen tilan, virustentorjuntaohjelman (AV) suojauksen tilan ja havaittujen aktiivisten uhkien määrän.

3. Valitse laite, jos haluat nähdä lisätietoja laitteesta ja käytettävissä olevista toiminnoista. Pikaikkunassa on suosituksia ja käytettävissä olevia toimintoja, kuten **Päivityskäytäntö**, Päivitä **virustentorjunta**, **Suorita** pikatarkistus **,** Suorita täysi tarkistus ja paljon muuta.

## <a name="manage-threat-detections-on-the-active-threats-page"></a>Uhkien tunnistuksen hallinta **Aktiiviset uhat -sivulla**

Seuraava menettely koskee asiakkaita, joilla on Microsoft 365 Business Premium. [Windows 10 laitteet on suojattava](./secure-win-10-pcs.md) [ja ne on rekisteröittävä Intunessa.](/mem/intune/enrollment/windows-enrollment-methods)

> [!NOTE]
> Uusi **Microsoft Defenderin virustentorjunta-kortti** **ja** Aktiiviset uhat -sivu tulee käyttöön vaiheittain, joten et ehkä voi käyttää niitä heti.

1. Siirry Microsoft 365 -hallintakeskus ja kirjaudu <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> sisään.

2. Valitse **Microsoft Defenderin virustentorjunta** Näytä **aktiiviset uhat**. (Voit myös valita siirtymisruudussa **Kunto**  >  **Virustentorjuntaohjelman &.)**

3. Valitse **Aktiiviset uhat** -sivulla havaittu uhka, niin saat siitä lisätietoja. Pikaikkuna avautuu, ja siinä on tietoja tästä uhasta, mukaan lukien mihin laitteisiin tämä vaikuttaa.

4. Valitse pikaikkunassa laite, jossa voit tarkastella käytettävissä olevia toimintoja, kuten **Päivityskäytäntö**, Päivitä **virustentorjunta**, Suorita **pikatarkistus** ja paljon muuta.

## <a name="actions-you-can-take"></a>Toimet, joita voit tehdä

Kun tarkastelet tietoja erityisistä uhista tai laitteista, näet suosituksia ja yhden tai useampia toimintoja, joita voit tehdä. Seuraavassa taulukossa on kuvattu toimintoja, joita saatat nähdä.<br><br>

| Toiminto | Kuvaus |
|--|--|
| Suojauksen määrittäminen | Uhkien torjuntakäytännöt on määritettävä. Siirry käytännön määrityssivulle valitsemalla linkki.<br><br>Tarvitsetko apua? Lisätietoja [on kohdassa Laitteen suojauksen hallinta Microsoft Intune.](/mem/intune/protect/endpoint-security-policy) |
| Päivityskäytäntö | Virustentorjunta- ja reaaliaikainen suojauskäytäntö on päivitettävä tai määritettävä. Siirry käytännön määrityssivulle valitsemalla linkki.<br><br>Tarvitsetko apua? Lisätietoja [on kohdassa Laitteen suojauksen hallinta Microsoft Intune.](/mem/intune/protect/endpoint-security-policy) |
| Suorita pikaskannaus | Käynnistää nopean virustentorjuntaohjelman laitteella ja keskittyy tavallisiin sijainppeihin, joissa saattaa olla rekisteröityjä haittaohjelmia, kuten rekisteriavaimia ja tunnettuja Windows käynnistyskansioita. |
| Suorita täysi tarkistus | Käynnistää laitteessa täyden virustentorjuntaohjelman, jossa keskitytään yleisiin sijainteja, joihin haittaohjelmat on rekisteröity, ja joka tiedosto ja kansio mukaan lukien laitteessa. Tulokset lähetetään [Microsoft Endpoint Manager.](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager) |
| Virustentorjuntaohjelman päivittäminen | Edellyttää laitetta virusten ja [haittaohjelmien](https://go.microsoft.com/fwlink/?linkid=2149926) torjuntaohjelmien suojauspäivitysten saamiseen. |
| Käynnistä laite uudelleen | Pakottaa Windows 10 käynnistämään uudelleen viiden minuutin kuluessa.<br><br>**TÄRKEÄÄ:** Laitteen omistaja tai käyttäjä ei saa automaattisesti ilmoitusta uudelleenkäynnistystoimenpiteestä, ja hän voi menettää tallentamattomia töitä. |

## <a name="manage-threat-detections-in-microsoft-endpoint-manager"></a>Uhkien tunnistuksen hallinta Microsoft Endpoint Manager

Voit hallita Microsoft Endpoint Manager tunnistuksen avulla. Windows 10-laitteet on [rekisteröittävä Intunessa](/mem/intune/enrollment/windows-enrollment-methods) (osa Microsoft Endpoint Manager).

1. Siirry Microsoft Endpoint Manager hallintakeskukseen ja <a href="https://go.microsoft.com/fwlink/p/?linkid=2150463" target="_blank">https://endpoint.microsoft.com</a> kirjaudu sisään.

2. Valitse siirtymisruudussa **Päätepisteen suojaus**.

3. Valitse **Hallinta**-kohdassa **Virustentorjunta**. Näet useita välilehtiä, kuten Yhteenveto **,** **huonosti Windows 10** päätepisteet ja Windows 10 **haittaohjelmia.**

4. Tarkista käytettävissä olevien välilehtien tiedot ja tee tarvittavat toimet.

Oletetaan esimerkiksi, että laitteet näkyvät tunnistetun Windows 10 **välilehdessä.** Kun valitset laitteen, käytettävissäsi on tiettyjä toimintoja, kuten Käynnistä uudelleen **,** **Pikatarkistus** **,** Täysi skannaus **,** Synkronoi tai Päivitä **allekirjoitukset**. Valitse toiminto laitteelle.

Seuraavassa taulukossa kuvataan toiminnot, joita saatat nähdä Microsoft Endpoint Manager.<br><br>

| Toiminto | Kuvaus |
|--|--|
| Käynnistä uudelleen | Pakottaa Windows 10 käynnistämään uudelleen viiden minuutin kuluessa.<br><br>**TÄRKEÄÄ:** Laitteen omistaja tai käyttäjä ei saa automaattisesti ilmoitusta uudelleenkäynnistystoimenpiteestä, ja hän voi menettää tallentamattomia töitä. |
| Pikaskannaus | Käynnistää nopean virustentorjuntaohjelman laitteella ja keskittyy tavallisiin sijainppeihin, joissa saattaa olla rekisteröityjä haittaohjelmia, kuten rekisteriavaimia ja tunnettuja Windows käynnistyskansioita. Tulokset lähetetään [Microsoft Endpoint Manager.](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager) |
| Täysi skannaus | Käynnistää laitteessa täyden virustentorjuntaohjelman, jossa keskitytään yleisiin sijainteja, joihin haittaohjelmat on rekisteröity, ja joka tiedosto ja kansio mukaan lukien laitteessa. Tulokset lähetetään [Microsoft Endpoint Manager.](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager) |
| Synkronoi | Edellyttää, että laite on sisään sisään intunella (osa Microsoft Endpoint Manager). Kun laite on sisään sisään, laite vastaanottaa laitteeseen määritetyt odottavat toiminnot tai käytännöt. |
| Allekirjoitusten päivittäminen | Edellyttää laitetta virusten ja [haittaohjelmien](https://go.microsoft.com/fwlink/?linkid=2149926) torjuntaohjelmien suojauspäivitysten saamiseen. |

> [!TIP]
> Lisätietoja on kohdassa Laitteiden [etätoiminnot.](/mem/intune/protect/endpoint-security-manage-devices#remote-actions-for-devices)

## <a name="how-to-submit-a-file-for-malware-analysis"></a>Tiedoston lähettäminen haittaohjelmien analysointia varten

Jos sinulla on tiedosto, jonka uskot ohitseen tai luokitellut väärin haittaohjelmiksi, voit lähettää tiedoston Microsoftille haittaohjelmien analysointia varten. Käyttäjät ja IT-järjestelmänvalvojat voivat lähettää tiedoston analyysia varten. Käy [https://www.microsoft.com/wdsi/filesubmission](https://www.microsoft.com/wdsi/filesubmission) osoitteessa .