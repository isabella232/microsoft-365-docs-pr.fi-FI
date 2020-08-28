---
title: Windows 10-tieto koneiden laite suojaus asetusten muokkaaminen tai luominen
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Tutustu Microsoft 365 for Businessin käytettävissä oleviin asetuksiin, joilla voit suojata Windows 10-laitteet.
ms.openlocfilehash: bd992113403c7134fb32bc6cced5bf216843241b
ms.sourcegitcommit: abf63669daf12993ad3353e4b578f41c8910b20f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/27/2020
ms.locfileid: "47289151"
---
# <a name="edit-or-create-device-protection-settings-for-windows-10-pcs"></a>Windows 10-tieto koneiden laite suojaus asetusten muokkaaminen tai luominen

Tämä artikkeli koskee Microsoft 365 Business Premiumia.

Kun olet määrittänyt Määritä Windowsin oletusarvoiset suojaus asetukset asetus sivulle, voit lisätä uusia käyttäjiä, jotka koskevat joko kaikki käyttäjät tai käyttäjä joukkoa. Voit myös muokata itse luomiasi.

## <a name="create-protection-settings-for-windows-10-devices"></a>Windows 10-laitteiden suojaus asetusten luominen

Katso video Windows 10-laitteiden suojaamisesta Microsoft 365 Business Premiumin avulla:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. Siirry hallinta keskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. Valitse vasemmanpuoleisesta siirtymis ruudusta **laitteet** \> **käytännöt** \> **Lisää**.
3. Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle. 
4. Valitse **Käytäntötyyppi**, valitse **Windows 10 -laitteen määritys**.
5. Laajenna **Suojatut Windows 10 -laitteet** \> määritä haluamasi asetukset. Lisä tietoja on kohdassa [käytettävissä olevat asetukset](#available-settings). 
    
    Voit aina palauttaa oletusasetuksen **Oletusasetusten palauttaminen** -linkin avulla. 
    
    ![Add policy pane with Windows 10 Device configuration selected](../media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja etsi käyttöoikeusryhmä, joka saa nämä asetukset \> **Valitse**.
7. Lopuksi tallenna käytäntö valitsemalla **Valmis** ja määritä se laitteisiin. 

## <a name="edit-windows-10-protection-settings"></a>Windows 10-suojaus asetusten muokkaaminen
 
1. Siirry hallinta keskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. Valitse vasemmanpuoleisesta siirtymis ruudusta **laitteet** - \> **käytännöt** .
1. Valitse aiemmin luotu Windows-laite käytännöt ja **Muokkaa**niitä.
1. Valitse **Muokkaa** sen asetus kohdan vierestä, jota haluat muuttaa, ja valitse sitten **Tallenna**.

## <a name="available-settings"></a>Käytettävissä olevat asetukset

Kaikki asetukset ovat oletusarvoisesti **käytössä**. Seuraavat asetukset ovat käytettävissä.
  
Lisä tietoja on kohdassa [miten Microsoft 365 Premium Map-sovelluksen suojaus ominaisuudet ovat Intune-asetuksiin](map-protection-features-to-intune-settings.md). 
  
|||
|:-----|:-----|
|Asetus  <br/> |Kuvaus  <br/> |
|Auta suojaamaan tietokoneitasi viruksilta ja muilta uhkilta käyttämällä Windows Defenderin virustenorjuntaa  <br/> |Edellyttää, että Windows Defenderin virustentorjunta on otettu käyttöön suojaamaan tietokoneita Internetiin yhdistämisen vaaralta.  <br/> |
|Auta suojaamaan tietokoneitasi verkkopohjaisilta uhkilta Microsoft Edgessä  <br/> |Ottaa käyttöön Edgen asetukset, jotka auttavat suojaamaan käyttäjiä vahingollisilta sivustoilta ja latauksilta.  <br/> |
|Käytä sääntöjä, jotka pienentävät laitteiden hyökkäyspinta-alaa  <br/> |Kun tämä asetus käytössä, hyökkäyspinta-alan pienentäminen estää toiminnot ja sovellukset, joita haittaohjelmat yleensä käyttävät laitteiden saastuttamiseen. Tämä asetus on käytettävissä vain, jos Windows Defenderin virustentorjunta on käytössä. Lisätietoja on artikkelissa [Hyökkäyspinta-alan pienentäminen](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/exploit-protection).  <br/> |
|Suojaa kansiot kiristysohjelmilta ja muilta uhilta  <br/> |Tämä asetus hyödyntää hallittua kansioiden käyttöä, jolla yrityksen data suojataan epäilyttävien tai haitallisten sovellusten, kuten kiristysohjelmien, tekemiltä muutoksilta. Tällaisia sovelluksia estetään tekemästä muutoksia suojattuihin kansioihin. Tämä asetus on käytettävissä vain, jos Windows Defenderin virustentorjunta on käytössä. Lisä tietoja [on artikkelissa kansioiden suojaaminen hallitsevalta kansiolla on käytettävissä](https://docs.microsoft.com/mem/configmgr/protect/deploy-use/create-deploy-exploit-guard-policy#bkmk_CFA) .  <br/> |
|Estä potentiaalisesti haitallisen sisällön käyttäminen Internetissä  <br/> |Tämän asetuksen avulla voit estää lähtevien käyttäjien yhteydet heikkomaineiseen Internet-sijainteihin, jotka voivat isännöidä tietojenkalasteluhuijauksia, heikkoutta tai muuta haitallista sisältöä. Tämä asetus on käytettävissä vain, jos Windows Defender anti virus-asetuksena on **käytössä**. Lisä tietoja on Ohje aiheessa [verkon suojaaminen](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/configure-real-time-protection-windows-defender-antivirus).  <br/> |
|Suojaa tietokoneiden tiedostot ja kansiot luvattomalta käytöltä BitLockerilla  <br/> |BitLocker suojaa datan salaamalla tietokoneen kiintolevyt ja estämällä sen joutumisen vääriin käsiin, jos tietokone katoaa tai varastetaan. Lisä tietoja on kohdassa [BitLocker-usein kysytyt kysymykset](https://go.microsoft.com/fwlink/?linkid=871000).  <br/> |
|Salli käyttäjille sovellusten lataaminen Microsoft Storesta  <br/> |Sallii käyttäjien ladata ja asentaa sovelluksia Microsoft Storesta. Sovellukset vaihtelevat peleistä tuottavuustyökaluihin, joten asetus on **käytössä**, mutta voit poistaa sen käytöstä lisäsuojausta varten.  <br/> |
|Salli käyttäjien käyttää Cortanaa  <br/> |Cortana-toiminto voi olla hyvin hyödyllinen. Cortana voi ottaa asetuksia käyttöön tai poistaa sen käytöstä, antaa ohjeita ja varmistaa, että tapaamiset ovat ajan tasalla, joten pidämme tämän asetuksen oletusarvoisesti **käytössä** .  <br/> |
|Salli käyttäjille Windows-vihjeiden ja -mainosten vastaanottaminen Microsoftilta  <br/> |Windows-vihjeet voivat olla käteviä ja auttaa perehdyttämään käyttäjiä, kun uusia ominaisuuksia julkaistaan.  <br/> |
|Pidä Windows 10 -laitteet ajan tasalla automaattisesti  <br/> |Varmistaa, että Windows 10 -laitteet vastaanottavat automaattisesti päivityksiä.  <br/> |
|Sammuta laitteen näyttö, kun se on ollut käyttämättömänä tämän verran  <br/> |Varmistaa, että yritystiedot on suojattu, jos käyttäjä ei tee mitään. Käyttäjä saattaa työskennellä julkisessa paikassa, kuten kahvilassa, ja poistua tai kääntää huomion pois hetkeksi, jolloin laite on alttiina satunnaisille katseille. Tällä asetuksella voit määrittää, miten kauan käyttäjä voi olla toimettomana, ennen kuin näyttö pimenee.  <br/> |
