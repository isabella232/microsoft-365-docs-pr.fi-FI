---
title: Sovellusten suojausasetusten muokkaaminen tai Windows 10 määrittäminen
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Opi luomaan tai muokkaamaan sovellusten hallintakäytäntöjä ja suojaamaan työtiedostoja käyttäjien henkilökohtaisissa Windows 10 laitteissa.
ms.openlocfilehash: 6d38d1765e0a331516b2261870112d530ab4ee50f24c6defba95964ea4d9dcfa
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53852640"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a>Sovellusten suojausasetusten määrittäminen tai muokkaaminen Windows 10 laitteissa

Tämä artikkeli koskee Microsoft 365 Business Premium.

## <a name="edit-an-app-management-policy-for-windows-10"></a>Muokkaa sovelluksen hallintakäytäntöä Windows 10

1. Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. Valitse vasemmassa siirtymispalkin kohdassa  \> **Laitekäytännöt** .
1. Valitse aiemmin luotu Windows ja valitse sitten **Muokkaa**.
1. Valitse **Muokkaa** sen asetuksen vierestä, jota haluat muuttaa, ja valitse sitten **Tallenna**.

## <a name="create-an-app-management-policy-for-windows-10"></a>Windows 10:n sovellustenhallintakäytännön luominen

Jos käyttäjillä on henkilökohtaisia Windows 10 -laitteita, joissa he tekevät työtehtäviä, voit suojata tiedot myös kyseisissä laitteissa.
  
1. Siirry hallintakeskukseen osoitteessa <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. Valitse vasemmassa siirtymispalkin kohdassa  \> **Laitekäytännöt** \> **Lisää**.
3. Kirjoita **Lisää käytäntö** -ruutuun yksilöivä nimi tälle käytännölle. 
4. Valitse **Käytännön tyyppi** -kohdassa **Windows 10:n sovellusten hallinta**.
5. Valitse **Laitetyyppi**-kohdassa joko **Henkilökohtainen** tai **Yrityksen omistama**.
6. **Salaa työtiedostot** otetaan automaattisesti käyttöön. 
7. Määritä **Estä käyttäjiä kopioimasta yritystietoja henkilökohtaisiin tiedostoihin ja pakota heidät tallentamaan työtiedostot OneDrive for Businessiin** **käyttöön**, jos et halua käyttäjien tallentavan työtiedostoja tietokoneeseensa. 
9. Laajenna **Tietojen palauttaminen Windows laitteissa**. Suosittelemme, että otat sen **käyttöön**.
    Ennen kuin voit etsiä Tietojenpalautusagentti-varmenteen, sinun on ensin luotava se. Ohjeet ovat kohdassa [EFS (Encrypting File System) Data Recovery Agent (DRA)](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate)-varmenteen luominen ja tarkistaminen.
    
    Työtiedostot on oletusarvoisesti salattu salaisella avaimella, joka on tallennettu laitteeseen ja liitetty käyttäjän profiiliin. Vain käyttäjä itse voi avata tiedoston ja purkaa sen salauksen. Jos laite häviää tai jos käyttäjä poistetaan, tiedosto voi jäädä salattuun tilaan. Järjestelmänvalvoja voi purkaa tiedoston salauksen Tietojenpalautusagentti-varmenteen (Data Recovery Agent, DRA) avulla.
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Laajenna **Suojaa lisää verkko- ja** pilvisijainteja, jos haluat lisätä muita toimialueita tai SharePoint verkkosijainteja ja varmistaa, että kaikkien luettelossa lueteltujen sovellusten tiedostot on suojattu. Jos sinun on annettava jompaankumpaan kenttään useita kohteita, lisää kohteiden väliin puolipiste (;).
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Päätä seuraavaksi, **ketkä saavat nämä asetukset**. Jos et halua käyttää oletusarvoista **Kaikki käyttäjät** -käyttöoikeusryhmää, valitse **Muuta** ja valitse käyttöoikeusryhmät, jotka saavat nämä asetukset \> **Valitse**.
12. Lopuksi tallenna käytäntö valitsemalla **Lisää** ja määritä se laitteisiin.