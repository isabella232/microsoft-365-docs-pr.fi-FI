---
title: Sovellusten suojaus asetusten muokkaaminen tai määrittäminen Windows 10-laitteille
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Lue, miten voit luoda tai muokata sovellusten hallinta käytäntöjä ja suojata työtiedostoja käyttäjien henkilökohtaisissa Windows 10-laitteissa.
ms.openlocfilehash: f85a59649e43c141b62091337b842a490d411833
ms.sourcegitcommit: abf63669daf12993ad3353e4b578f41c8910b20f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/27/2020
ms.locfileid: "47289195"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a>Windows 10-laitteiden sovellusten suojaus asetusten määrittäminen tai muokkaaminen

Tämä artikkeli koskee Microsoft 365 Business Premiumia.

## <a name="edit-an-app-management-policy-for-windows-10"></a>Sovelluksen hallinta käytännön muokkaaminen Windows 10-sovelluksessa

1. Siirry hallinta keskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. Valitse vasemmanpuoleisesta siirtymis ruudusta **laitteet** - \> **käytännöt** .
1. Valitse aiemmin luotu Windows-sovellus käytännössä ja **Muokkaa**sitä.
1. Valitse **Muokkaa** sen asetus kohdan vierestä, jota haluat muuttaa, ja valitse sitten **Tallenna**.

## <a name="create-an-app-management-policy-for-windows-10"></a>Windows 10:n sovellustenhallintakäytännön luominen

Jos käyttäjillä on henkilökohtaisia Windows 10 -laitteita, joissa he tekevät työtehtäviä, voit suojata tiedot myös kyseisissä laitteissa.
  
1. Siirry hallinta keskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. Valitse vasemmanpuoleisesta siirtymis ruudusta **laitteet** \> **käytännöt** \> **Lisää**.
3. Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle. 
4. Valitse **Käytännön tyyppi** -kohdassa **Windows 10:n sovellusten hallinta**.
5. Valitse **laite tyyppi**-kohdassa joko **henkilökohtainen** tai **yrityksen omistama**.
6. **Salaa työtiedostot** otetaan automaattisesti käyttöön. 
7. Määritä **Estä käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin ja pakota heidät tallentamaan työtiedostot OneDrive for Businessiin** **käyttöön**, jos et halua käyttäjien tallentavan työtiedostoja tietokoneeseensa. 
9. Laajenna **tietojen palauttaminen Windows-laitteissa**. Suosittelemme **, että otat sen käyttöön**.
    Ennen kuin voit etsiä Tietojenpalautusagentti-varmenteen, sinun on ensin luotava se. Lisä tietoja on artikkelissa EFS [(Encrypting File System)-tietojen palautus agentin (DRA) varmenteen luominen ja tarkistaminen](https://go.microsoft.com/fwlink/p/?linkid=853700).
    
    Työtiedostot on oletusarvoisesti salattu salaisella avaimella, joka on tallennettu laitteeseen ja liitetty käyttäjän profiiliin. Vain käyttäjä itse voi avata tiedoston ja purkaa sen salauksen. Jos laite häviää tai jos käyttäjä poistetaan, tiedosto voi jäädä salattuun tilaan. Järjestelmänvalvoja voi purkaa tiedoston Sala uksen käyttämällä tietojen palautus agentti (DRA)-varmennetta.
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Laajenna **suojaa muita verkko-ja pilvi sijainteja** , jos haluat lisätä muita toimi alueita tai SharePoint Online-sijainteja varmistaaksesi, että kaikkien luettelossa olevien sovellusten tiedostot ovat suojattuja. Jos sinun on annettava jompaankumpaan kenttään useita kohteita, lisää kohteiden väliin puolipiste (;).
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja valitse käyttöoikeusryhmät, jotka saavat nämä asetukset \> **Valitse**.
12. Lopuksi tallenna käytäntö valitsemalla **Lisää** ja määritä se laitteisiin. 
