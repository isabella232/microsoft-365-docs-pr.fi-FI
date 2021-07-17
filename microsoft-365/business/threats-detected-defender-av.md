---
title: Uhkia, jotka Microsoft Defenderin virustentorjunta
f1.keywords: CSH
ms.author: sharik
author: SKjerland
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- Adm_O365
- Adm_TOC
ms.custom: AdminSurgePortfolio
search.appverid: MET150
description: Lue, Microsoft Defenderin virustentorjunta suojata Windows laitteitasi ohjelmistouhkilta, kuten viruksilta, haittaohjelmilta ja vakoiluohjelmilta.
ms.openlocfilehash: 7c5d000e2a8c30e17d1f890cef69fe88beed75bb
ms.sourcegitcommit: dcb97fbfdae52960ae62b6faa707a05358193ed5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/25/2021
ms.locfileid: "53465407"
---
# <a name="threats-detected-by-microsoft-defender-antivirus"></a>Uhkia, jotka Microsoft Defenderin virustentorjunta

Microsoft Defenderin virustentorjunta suojaa Windows laitteeltasi ohjelmistouhkilta, kuten viruksilta, haittaohjelmilta ja vakoiluohjelmilta.

- Virukset leviävät yleensä liittämällä koodinsa laitteen tai verkon muihin tiedostoihin ja voivat aiheuttaa sen, että tartunnan saaneet ohjelmat toimivat virheellisesti.
- Haittaohjelmat sisältävät vahingollisia tiedostoja, sovelluksia ja koodia, jotka voivat vahingoittaa ja häiritä laitteiden tavallista käyttöä. Haittaohjelmat voivat myös sallia luvattoman käytön, käyttää järjestelmäresursseja, varastaa salasanoja ja tilitietoja, lukita sinut ulos tietokoneeltasi ja pyytää kiristysta ja paljon muuta.
- Vakoiluohjelma kerää tietoja, kuten verkkoselaamista, ja lähettää tiedot etäpalvelimiin.
 
Uhan uhkien Microsoft Defenderin virustentorjunta on useita menetelmiä. Näitä menetelmiä ovat pilvipohjainen suojaus, reaaliaikainen suojaus ja erilliset suojauspäivitykset.

- Pilvipohjainen suojaus auttaa löytämään nopeasti uusia ja uusia uhkia ja estämään ne.
- Aina skannattaessa käytetään tiedostojen ja prosessien valvontaa ja muita tekniikoita (tunnetaan myös nimellä *reaaliaikainen suojaus).*
- Dedicated protection updates are based on machine learning, human and automated big-data analysis, and in-depth threat resistance research. 

Lisätietoja haittaohjelmista ja Microsoft Defenderin virustentorjunta on seuraavissa artikkeleissa: 

- [Muiden uhkien & haittaohjelmien ymmärtäminen](/windows/security/threat-protection/intelligence/understanding-malware)
- [Miten Microsoft tunnistaa haittaohjelmat ja mahdollisesti ei-toivotut sovellukset](/windows/security/threat-protection/intelligence/criteria)
- [Seuraavan sukupolven suojaus Windows 10](/windows/security/threat-protection/microsoft-defender-antivirus/microsoft-defender-antivirus-in-windows-10)

## <a name="what-happens-when-a-non-microsoft-antivirus-solution-is-used"></a>Mitä tapahtuu, kun käytössä on muu kuin Microsoftin virustentorjuntaratkaisu? 

Microsoft Defenderin virustentorjunta kuuluu käyttöjärjestelmään ja se on käytössä laitteissa, joissa on Windows 10. Jos kuitenkin käytät muita kuin Microsoftin virustentorjuntaratkaisuja etkä käytä [Microsoft Defender for Endpointia](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-advanced-threat-protection), Microsoft Defenderin virustentorjunta siirtyy automaattisesti ei-tilaan.  

Kun käyttäjät ja asiakkaat ovat Poissa käytöstä -tilassa, he Microsoft Defenderin virustentorjunta uhkien tunnistamiseen ajoitettujen tai tarvittaessa tehtävien tarkistusten avulla. mutta Microsoft Defenderin virustentorjunta enää:

- käyttää oletusarvoisena virustentorjuntasovelluksena.
- tarkista tiedostot aktiivisesti uhkia varten.
- korjata tai ratkaista uhkia.

Jos poistat ei-Microsoftin virustentorjuntaratkaisun asennuksen, Microsoft Defenderin virustentorjunta siirtyy automaattisesti aktiiviseen tilaan ja suojaa Windows uhkilta.

> [!TIP]
> - Jos käytät virustentorjuntaohjelmaa, Microsoft 365 käyttää Microsoft Defenderin virustentorjunta ensisijaisena virustentorjuntaratkaisuna. Integrointi voi parantaa suojausta. Katso [Paremmat yhdessä: Microsoft Defenderin virustentorjunta Office 365.](/windows/security/threat-protection/microsoft-defender-antivirus/office-365-microsoft-defender-antivirus)
> - Varmista, että Microsoft Defenderin virustentorjunta ajan tasalla, vaikka käytössäsi olisi jokin muu kuin Microsoftin virustentorjuntaratkaisu.

## <a name="what-to-expect-when-threats-are-detected"></a>Mitä on odotettavissa, kun uhkia havaitaan

Kun uhkia havaitaan Microsoft Defenderin virustentorjunta, tapahtuu seuraavat asiat:

- Käyttäjät saavat [ilmoituksia Windows.](https://support.microsoft.com/windows/8942c744-6198-fe56-4639-34320cf9444e) 
- Tunnistuksen vaihtoehdot Windowsin suojaus **suojaushistoriasivulla.** [](/windows/security/threat-protection/windows-defender-security-center/windows-defender-security-center)  
- Jos olet varmistanut [Windows 10-laitteet](secure-win-10-pcs.md) ja rekisteröinyt ne [Intunessa](/mem/intune/enrollment/windows-enrollment-methods)ja organisaatiossasi on enintään 800 laitetta, näet uhkien tunnistuksen  ja oivallukset <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">Microsoft 365 -hallintakeskus:ssä</a> Uhat ja  virustentorjunta -sivulla, jota voit käyttää Microsoft Defenderin virustentorjunta-kortista aloitussivulla (tai siirtymisruudussa valitsemalla Terveysuhkien &   >  **virustentorjunta**).

    Jos organisaatiossasi on yli 800 Intuneen rekisteröityä laitetta, sinua pyydetään katselemaan [uhkien](/mem/endpoint-manager-overview) tunnistuksen ja tietojen Microsoft Endpoint Manager Uhkia ja virustentorjuntaa -sivun **sijaan.**
 
    > [!NOTE]
    > Uusi **Microsoft Defenderin virustentorjunta** sekä Uhkien ja **virustentorjuntaohjelmien** sivu tulee käyttöön vaiheittain, joten et ehkä voi käyttää niitä heti.

Useimmissa tapauksissa käyttäjien ei tarvitse tehdä mitään lisätoimia. Kun laitteessa havaitaan haitallisen tiedoston tai ohjelman, se Microsoft Defenderin virustentorjunta sen ja estää sen suorittamisen. Lisäksi virustentorjunta- ja haittaohjelmien torjuntaohjelmaan lisätään uusia havaittuja uhkia, jotta myös muut laitteet ja käyttäjät ovat suojattuja.  

Jos käyttäjän on tehtävä toimenpiteitä, kuten hyväksyessään haitallisen tiedoston poistamisen, käyttäjä näkee sen saadessään ilmoituksen. Lisätietoja toiminnoista, joita Microsoft Defenderin virustentorjunta käyttäjän puolesta tai joita käyttäjät saattavat joutua tekemään, on [suojaushistoriassa.](https://support.microsoft.com/office/f1e5fd95-09b4-46d1-b8c7-1059a1e09708) Lisätietoja uhkien tunnistuksen hallitsemisesta IT-ammattilaisena/järjestelmänvalvojana on kohdassa [Havaittujen uhkien tarkistaminen ja toimenpiteisiin toimiminen.](review-threats-take-action.md)

Lisätietoja erilaisista uhista on <a href="https://www.microsoft.com/wdsi/threats" target="_blank">Microsoftin suojaustiedustelu-sivustossa,</a>jossa voit suorittaa seuraavat toimet: 

- Tarkastele ajankohtaista tietoa parhaista uhista.
- Tarkastele tietyn alueen uusimpia uhkia.
- Hae uhkien tietokatkosta lisätietoja tietystä uhasta.

## <a name="related-content"></a>Aiheeseen liittyvä sisältö

[Suojattujen Windows 10](secure-windows-10-devices.md) (artikkeli)\
[Arvioi Microsoft Defenderin virustentorjunta](/windows/security/threat-protection/microsoft-defender-antivirus/evaluate-microsoft-defender-antivirus) (artikkeli)\
[Reaaliaikaisen ja pilvipohjaisen virustentorjuntaohjelman](/mem/intune/user-help/turn-on-defender-windows#turn-on-real-time-and-cloud-delivered-protection) (article)\ käyttöönottaaminen
[Ohjeet Microsoft Defenderin virustentorjunta käyttöön Windowsin suojaus](/windows/security/threat-protection/microsoft-defender-antivirus/microsoft-defender-security-center-antivirus) (artikkeli)\
[Ryhmäkäytännön Microsoft Defenderin virustentorjunta käyttöönottaaminen](/mem/intune/user-help/turn-on-defender-windows#turn-on-windows-defender) (artikkeli)\
[Virustentorjuntamääritysten päivittäminen](/mem/intune/user-help/turn-on-defender-windows#update-your-antivirus-definitions) (artikkeli)\
[Haittaohjelmien ja muiden kuin haittaohjelmien lähettäminen Microsoftille analyysia varten](/microsoft-365/security/office-365-security/submitting-malware-and-non-malware-to-microsoft-for-analysis) (artikkeli)
