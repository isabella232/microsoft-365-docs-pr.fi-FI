---
title: Suojatut Windows 10 -laitteet
f1.keywords:
- CSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4WindowsConfig
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
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: Lue lisää oletuslaitekäytännön asetusten määrittämisestä, jonka Windows 10 laite saa kirjauduttaessa sisään työ- tai koulutiliin.
ms.openlocfilehash: 3f85549e722c9aa4196cf50fc02bee2e89506017
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925235"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="32103-103">Suojatut Windows 10 -laitteet</span><span class="sxs-lookup"><span data-stu-id="32103-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="32103-104">Tämä artikkeli koskee Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="32103-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="32103-105">Tässä määrittämäsi asetukset ovat osa Windows 10:n oletuslaitekäytäntöä.</span><span class="sxs-lookup"><span data-stu-id="32103-105">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="32103-106">Kaikki käyttäjät, jotka Windows 10 yhteyden laitteeseen, mukaan lukien mobiililaitteet ja tietokoneet, kirjautumalla sisään työtilinsä avulla, saavat nämä asetukset automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="32103-106">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="32103-107">On suositeltavaa, että hyväksyt oletuskäytännön asennuksen aikana ja lisäät myöhemmin käytäntöjä, jotka kohdistuvat tiettyyn käyttäjäryhmään.</span><span class="sxs-lookup"><span data-stu-id="32103-107">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="32103-108">Windows 10 -laitteiden suojausasetukset</span><span class="sxs-lookup"><span data-stu-id="32103-108">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="32103-p102">Kaikki asetukset ovat oletusarvoisesti **käytössä**. Seuraavat asetukset ovat käytettävissä:</span><span class="sxs-lookup"><span data-stu-id="32103-p102">By default all settings are **On**. The following settings are available:</span></span>
  


|<span data-ttu-id="32103-111">Asetus</span><span class="sxs-lookup"><span data-stu-id="32103-111">Setting</span></span>  <br/> |<span data-ttu-id="32103-112">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="32103-112">Description</span></span>  <br/> |
|:-----|:-----|
|<span data-ttu-id="32103-113">Auta suojaamaan tietokoneitasi viruksilta ja muilta uhkilta käyttämällä Windows Defenderin virustenorjuntaa</span><span class="sxs-lookup"><span data-stu-id="32103-113">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="32103-114">Edellyttää, että Windows Defenderin virustentorjunta on otettu käyttöön suojaamaan tietokoneita Internetiin yhdistämisen vaaralta.</span><span class="sxs-lookup"><span data-stu-id="32103-114">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="32103-115">Auta suojaamaan tietokoneitasi verkkopohjaisilta uhkilta Microsoft Edgessä</span><span class="sxs-lookup"><span data-stu-id="32103-115">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="32103-116">Ottaa käyttöön Edgen asetukset, jotka auttavat suojaamaan käyttäjiä vahingollisilta sivustoilta ja latauksilta.</span><span class="sxs-lookup"><span data-stu-id="32103-116">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="32103-117">Suojaa tietokoneiden tiedostot ja kansiot luvattomalta käytöltä BitLockerilla</span><span class="sxs-lookup"><span data-stu-id="32103-117">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="32103-118">BitLocker suojaa datan salaamalla tietokoneen kiintolevyt ja estämällä sen joutumisen vääriin käsiin, jos tietokone katoaa tai varastetaan.</span><span class="sxs-lookup"><span data-stu-id="32103-118">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen.</span></span> <span data-ttu-id="32103-119">Lisätietoja on kohdassa [BitLockerin usein kysytyt kysymykset.](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions)</span><span class="sxs-lookup"><span data-stu-id="32103-119">For more information, see [Bitlocker FAQ](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions).</span></span>  <br/> |
|<span data-ttu-id="32103-120">Sammuta laitteen näyttö, kun se on ollut käyttämättömänä tämän verran</span><span class="sxs-lookup"><span data-stu-id="32103-120">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="32103-p104">Varmistaa, että yritystiedot on suojattu, jos käyttäjä ei tee mitään. Käyttäjä saattaa työskennellä julkisessa paikassa, kuten kahvilassa, ja poistua tai kääntää huomion pois hetkeksi, jolloin laite on alttiina satunnaisille katseille. Tällä asetuksella voit määrittää, miten kauan käyttäjä voi olla toimettomana, ennen kuin näyttö pimenee.</span><span class="sxs-lookup"><span data-stu-id="32103-p104">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|