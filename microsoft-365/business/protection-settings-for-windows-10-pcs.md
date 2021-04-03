---
title: Windows 10 -tietokoneiden laitesuojausasetusten muokkaaminen tai luominen
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Lue lisää Microsoft 365 for Businessin asetuksista Windows 10 -laitteiden suojaaminen.
ms.openlocfilehash: acfb27b2e4592d4ed1e446a63c9495ae07d916de
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578223"
---
# <a name="edit-or-create-device-protection-settings-for-windows-10-pcs"></a>Windows 10 -tietokoneiden laitesuojausasetusten muokkaaminen tai luominen

Tämä artikkeli koskee Microsoft 365 Business Premiumia.

Kun olet määrittänyt Windowsin oletussuojausasetukset Asetukset-sivulla, voit lisätä uusia asetuksia, jotka koskevat joko kaikkia käyttäjiä tai käyttäjäjoukkoa. Voit myös muokata luomiasi.

## <a name="create-protection-settings-for-windows-10-devices"></a>Suojausasetusten luominen Windows 10 -laitteille

Katso video Windows 10 -laitteiden tietoturvasta Microsoft 365 Business Premiumin avulla:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. Valitse vasemmassa siirtymispalkin kohdassa  \> **Laitekäytännöt** \> **Lisää.**
3. Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle. 
4. Valitse **Käytäntötyyppi**, valitse **Windows 10 -laitteen määritys**.
5. Laajenna **Suojatut Windows 10 -laitteet** \> määritä haluamasi asetukset. Lisätietoja on kohdassa Käytettävissä [olevat asetukset.](#available-settings) 
    
    Voit aina palauttaa oletusasetuksen **Oletusasetusten palauttaminen** -linkin avulla. 
    
    ![Add policy pane with Windows 10 Device configuration selected](../media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja etsi käyttöoikeusryhmä, joka saa nämä asetukset \> **Valitse**.
7. Lopuksi tallenna käytäntö valitsemalla **Valmis** ja määritä se laitteisiin. 

## <a name="edit-windows-10-protection-settings"></a>Windows 10:n suojausasetusten muokkaaminen
 
1. Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. Valitse vasemmassa siirtymispalkin kohdassa  \> **Laitekäytännöt.**
1. Valitse olemassa oleva Windows-laitekäytäntö ja sitten **Muokkaa.**
1. Valitse **Muokkaa** sen asetuksen vieressä, jota haluat muuttaa, ja valitse **sitten Tallenna.**

## <a name="available-settings"></a>Käytettävissä olevat asetukset

Kaikki asetukset ovat oletusarvoisesti **käytössä**. Seuraavat asetukset ovat käytettävissä.
  
Lisätietoja on kohdassa Miten [Microsoft 365 Premiumin suojausominaisuudet liittyvät Intune-asetuksiin.](map-protection-features-to-intune-settings.md) 
  
|||
|:-----|:-----|
|Asetus  <br/> |Kuvaus  <br/> |
|Auta suojaamaan tietokoneitasi viruksilta ja muilta uhkilta käyttämällä Windows Defenderin virustenorjuntaa  <br/> |Edellyttää, että Windows Defenderin virustentorjunta on otettu käyttöön suojaamaan tietokoneita Internetiin yhdistämisen vaaralta.  <br/> |
|Auta suojaamaan tietokoneitasi verkkopohjaisilta uhkilta Microsoft Edgessä  <br/> |Ottaa käyttöön Edgen asetukset, jotka auttavat suojaamaan käyttäjiä vahingollisilta sivustoilta ja latauksilta.  <br/> |
|Käytä sääntöjä, jotka pienentävät laitteiden hyökkäyspinta-alaa  <br/> |Kun tämä asetus käytössä, hyökkäyspinta-alan pienentäminen estää toiminnot ja sovellukset, joita haittaohjelmat yleensä käyttävät laitteiden saastuttamiseen. Tämä asetus on käytettävissä vain, jos Windows Defenderin virustentorjunta on käytössä. Lisätietoja on artikkelissa [Hyökkäyspinta-alan pienentäminen](/windows/security/threat-protection/microsoft-defender-atp/exploit-protection).  <br/> |
|Suojaa kansiot kiristysohjelmilta ja muilta uhilta  <br/> |Tämä asetus hyödyntää hallittua kansioiden käyttöä, jolla yrityksen data suojataan epäilyttävien tai haitallisten sovellusten, kuten kiristysohjelmien, tekemiltä muutoksilta. Tällaisia sovelluksia estetään tekemästä muutoksia suojattuihin kansioihin. Tämä asetus on käytettävissä vain, jos Windows Defenderin virustentorjunta on käytössä. Lisätietoja [on kohdassa Kansioiden suojaaminen valvotuilla](/mem/configmgr/protect/deploy-use/create-deploy-exploit-guard-policy#bkmk_CFA) kansioilla.  <br/> |
|Estä potentiaalisesti haitallisen sisällön käyttäminen Internetissä  <br/> |Tämän asetuksen avulla voit estää lähtevät käyttäjäyhteydet huonomaineisille Internet-sijainnille, jotka saattavat isännöidä tietojenkalasteluhuijauksia, hyväksikäyttöä tai muuta haitallista sisältöä. Tämä asetus on käytettävissä vain, jos Windows Defenderin virustentorjunta on **käytössä.** Lisätietoja on ohjeaiheessa [Verkon suojaaminen.](/windows/security/threat-protection/windows-defender-antivirus/configure-real-time-protection-windows-defender-antivirus)  <br/> |
|Suojaa tietokoneiden tiedostot ja kansiot luvattomalta käytöltä BitLockerilla  <br/> |BitLocker suojaa datan salaamalla tietokoneen kiintolevyt ja estämällä sen joutumisen vääriin käsiin, jos tietokone katoaa tai varastetaan. Lisätietoja on [BitLockerin usein kysytyissä kysymyksissä.](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions)  <br/> |
|Salli käyttäjille sovellusten lataaminen Microsoft Storesta  <br/> |Sallii käyttäjien ladata ja asentaa sovelluksia Microsoft Storesta. Sovellukset vaihtelevat peleistä tuottavuustyökaluihin, joten asetus on **käytössä**, mutta voit poistaa sen käytöstä lisäsuojausta varten.  <br/> |
|Salli käyttäjien käyttää Cortanaa  <br/> |Cortana-toiminto voi olla hyvin hyödyllinen. Cortana voi ottaa asetukset käyttöön tai poistaa ne käytöstä, antaa reittiohjeita ja varmistaa, että olet ajoissa tapaamisia varten, joten asetus **on** oletusarvoisesti käytössä.  <br/> |
|Salli käyttäjille Windows-vihjeiden ja -mainosten vastaanottaminen Microsoftilta  <br/> |Windows-vihjeet voivat olla käteviä ja auttaa perehdyttämään käyttäjiä, kun uusia ominaisuuksia julkaistaan.  <br/> |
|Pidä Windows 10 -laitteet ajan tasalla automaattisesti  <br/> |Varmistaa, että Windows 10 -laitteet vastaanottavat automaattisesti päivityksiä.  <br/> |
|Sammuta laitteen näyttö, kun se on ollut käyttämättömänä tämän verran  <br/> |Varmistaa, että yritystiedot on suojattu, jos käyttäjä ei tee mitään. Käyttäjä saattaa työskennellä julkisessa paikassa, kuten kahvilassa, ja poistua tai kääntää huomion pois hetkeksi, jolloin laite on alttiina satunnaisille katseille. Tällä asetuksella voit määrittää, miten kauan käyttäjä voi olla toimettomana, ennen kuin näyttö pimenee.  <br/> |