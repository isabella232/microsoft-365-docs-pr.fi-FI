---
title: Pc-tietokoneiden laitesuojausasetusten muokkaaminen Windows 10 luominen
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
description: Lue lisää Microsoft 365 for Businessin Windows 10 asetuksista.
ms.openlocfilehash: 4859681d5e71a61b8a5dd58114bce899f485967a
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925315"
---
# <a name="edit-or-create-device-protection-settings-for-windows-10-pcs"></a>Pc-tietokoneiden laitesuojausasetusten muokkaaminen Windows 10 luominen

Tämä artikkeli koskee Microsoft 365 Business Premium.

Kun olet määrittänyt oletussuojausasetukset Windows-sivulla, voit lisätä uusia asetuksia, jotka koskevat joko kaikkia käyttäjiä tai käyttäjäjoukkoa. Voit myös muokata itse luomiasi.

## <a name="create-protection-settings-for-windows-10-devices"></a>Suojausasetusten luominen Windows 10 laitteille

Katso video siitä, miten voit suojata Windows 10 laitteiden Microsoft 365 Business Premium:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. Valitse vasemmassa siirtymispalkin kohdassa  \> **Laitekäytännöt** \> **Lisää**.
3. Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle. 
4. Valitse **Käytäntötyyppi**, valitse **Windows 10 -laitteen määritys**.
5. Laajenna **Suojatut Windows 10 -laitteet** \> määritä haluamasi asetukset. Lisätietoja on kohdassa Käytettävissä [olevat asetukset.](#available-settings) 
    
    Voit aina palauttaa oletusasetuksen **Oletusasetusten palauttaminen** -linkin avulla. 
    
    ![Add policy pane with Windows 10 Device configuration selected](../media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja etsi käyttöoikeusryhmä, joka saa nämä asetukset \> **Valitse**.
7. Lopuksi tallenna käytäntö valitsemalla **Valmis** ja määritä se laitteisiin. 

## <a name="edit-windows-10-protection-settings"></a>Muokkaa Windows 10 -asetuksia
 
1. Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. Valitse vasemmassa siirtymispalkin kohdassa  \> **Laitekäytännöt** .
1. Valitse olemassa oleva Windows ja valitse sitten **Muokkaa**.
1. Valitse **Muokkaa** sen asetuksen vierestä, jota haluat muuttaa, ja valitse sitten **Tallenna**.

## <a name="available-settings"></a>Käytettävissä olevat asetukset

Kaikki asetukset ovat oletusarvoisesti **käytössä**. Seuraavat asetukset ovat käytettävissä.
  
Lisätietoja on kohdassa Miten [windows-tietokoneen suojausominaisuudet Microsoft 365 Premium Intune-asetuksiin.](map-protection-features-to-intune-settings.md) 


|Asetus  <br/> |Kuvaus  <br/> |
|:-----|:-----|
|Auta suojaamaan tietokoneitasi viruksilta ja muilta uhkilta käyttämällä Windows Defenderin virustenorjuntaa  <br/> |Edellyttää, että Windows Defenderin virustentorjunta on otettu käyttöön suojaamaan tietokoneita Internetiin yhdistämisen vaaralta.  <br/> |
|Auta suojaamaan tietokoneitasi verkkopohjaisilta uhkilta Microsoft Edgessä  <br/> |Ottaa käyttöön Edgen asetukset, jotka auttavat suojaamaan käyttäjiä vahingollisilta sivustoilta ja latauksilta.  <br/> |
|Käytä sääntöjä, jotka pienentävät laitteiden hyökkäyspinta-alaa  <br/> |Kun tämä asetus käytössä, hyökkäyspinta-alan pienentäminen estää toiminnot ja sovellukset, joita haittaohjelmat yleensä käyttävät laitteiden saastuttamiseen. Tämä asetus on käytettävissä vain, jos Windows Defenderin virustentorjunta on käytössä. Lisätietoja on artikkelissa [Hyökkäyspinta-alan pienentäminen](/windows/security/threat-protection/microsoft-defender-atp/exploit-protection).  <br/> |
|Suojaa kansiot kiristysohjelmilta ja muilta uhilta  <br/> |Tämä asetus hyödyntää hallittua kansioiden käyttöä, jolla yrityksen data suojataan epäilyttävien tai haitallisten sovellusten, kuten kiristysohjelmien, tekemiltä muutoksilta. Tällaisia sovelluksia estetään tekemästä muutoksia suojattuihin kansioihin. Tämä asetus on käytettävissä vain, jos Windows Defenderin virustentorjunta on käytössä. Lisätietoja [on kohdassa Kansioiden suojaaminen valvotuilla](/mem/configmgr/protect/deploy-use/create-deploy-exploit-guard-policy#bkmk_CFA) kansioiden käyttöolta.  <br/> |
|Estä potentiaalisesti haitallisen sisällön käyttäminen Internetissä  <br/> |Tämän asetuksen avulla voit estää lähtevät käyttäjäyhteydet huonomaineisille Internet-sijainnille, jotka saattavat isännöidä tietojenkalasteluhuijauksia, heikkouksia hyödyntäviä ohjelmia tai muuta haitallista sisältöä. Tämä asetus on käytettävissä vain, Windows Defenderin virustentorjunta asetukseksi on **määritetty Käytössä**. Lisätietoja on kohdassa [Verkon suojaaminen.](/windows/security/threat-protection/windows-defender-antivirus/configure-real-time-protection-windows-defender-antivirus)  <br/> |
|Suojaa tietokoneiden tiedostot ja kansiot luvattomalta käytöltä BitLockerilla  <br/> |BitLocker suojaa datan salaamalla tietokoneen kiintolevyt ja estämällä sen joutumisen vääriin käsiin, jos tietokone katoaa tai varastetaan. Lisätietoja on kohdassa [BitLockerin usein kysytyt kysymykset.](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions)  <br/> |
|Salli käyttäjille sovellusten lataaminen Microsoft Storesta  <br/> |Sallii käyttäjien ladata ja asentaa sovelluksia Microsoft Storesta. Sovellukset vaihtelevat peleistä tuottavuustyökaluihin, joten asetus on **käytössä**, mutta voit poistaa sen käytöstä lisäsuojausta varten.  <br/> |
|Salli käyttäjien käyttää Cortanaa  <br/> |Cortana-toiminto voi olla hyvin hyödyllinen. Cortana ottaa asetukset käyttöön tai poistaa ne käytöstä, antaa reittiohjeita ja varmistaa, että olet ajoissa tapaamisia varten, joten asetus **on** oletusarvoisesti käytössä.  <br/> |
|Salli käyttäjille Windows-vihjeiden ja -mainosten vastaanottaminen Microsoftilta  <br/> |Windows-vihjeet voivat olla käteviä ja auttaa perehdyttämään käyttäjiä, kun uusia ominaisuuksia julkaistaan.  <br/> |
|Pidä Windows 10 -laitteet ajan tasalla automaattisesti  <br/> |Varmistaa, että Windows 10 -laitteet vastaanottavat automaattisesti päivityksiä.  <br/> |
|Sammuta laitteen näyttö, kun se on ollut käyttämättömänä tämän verran  <br/> |Varmistaa, että yritystiedot on suojattu, jos käyttäjä ei tee mitään. Käyttäjä saattaa työskennellä julkisessa paikassa, kuten kahvilassa, ja poistua tai kääntää huomion pois hetkeksi, jolloin laite on alttiina satunnaisille katseille. Tällä asetuksella voit määrittää, miten kauan käyttäjä voi olla toimettomana, ennen kuin näyttö pimenee.  <br/> |