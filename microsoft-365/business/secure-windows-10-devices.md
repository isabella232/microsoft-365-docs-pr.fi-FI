---
title: Suojatut Windows 10 -laitteet
f1.keywords:
- CSH
ms.author: sirkkuw
author: sirkkuw
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: 'Lue lisä tietoja oletus arvoista ja muista asetuksista Windows 10-laitteiden turvaamiseksi. '
ms.openlocfilehash: 9560bb4e299dba8f92d435a64670261b0e7e0290
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593441"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="b2752-103">Suojatut Windows 10 -laitteet</span><span class="sxs-lookup"><span data-stu-id="b2752-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="b2752-104">Tässä määrittämäsi asetukset ovat osa Windows 10:n oletuslaitekäytäntöä.</span><span class="sxs-lookup"><span data-stu-id="b2752-104">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="b2752-105">Kaikki käyttäjät, jotka yhdistävät Windows 10-laitteen, mukaan lukien mobiililaitteet ja tieto koneet, kirjautumiseen sisään työtililleen saavat automaattisesti nämä asetukset.</span><span class="sxs-lookup"><span data-stu-id="b2752-105">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="b2752-106">On suositeltavaa, että hyväksyt oletuskäytännön asennuksen aikana ja lisäät myöhemmin käytäntöjä, jotka kohdistuvat tiettyyn käyttäjäryhmään.</span><span class="sxs-lookup"><span data-stu-id="b2752-106">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="b2752-107">Windows 10 -laitteiden suojausasetukset</span><span class="sxs-lookup"><span data-stu-id="b2752-107">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="b2752-p102">Kaikki asetukset ovat oletusarvoisesti **käytössä**. Seuraavat asetukset ovat käytettävissä:</span><span class="sxs-lookup"><span data-stu-id="b2752-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="b2752-110">Asetus</span><span class="sxs-lookup"><span data-stu-id="b2752-110">Setting</span></span>  <br/> |<span data-ttu-id="b2752-111">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="b2752-111">Description</span></span>  <br/> |
|<span data-ttu-id="b2752-112">Auta suojaamaan tietokoneitasi viruksilta ja muilta uhkilta käyttämällä Windows Defenderin virustenorjuntaa</span><span class="sxs-lookup"><span data-stu-id="b2752-112">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="b2752-113">Edellyttää, että Windows Defenderin virustentorjunta on otettu käyttöön suojaamaan tietokoneita Internetiin yhdistämisen vaaralta.</span><span class="sxs-lookup"><span data-stu-id="b2752-113">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="b2752-114">Auta suojaamaan tietokoneitasi verkkopohjaisilta uhkilta Microsoft Edgessä</span><span class="sxs-lookup"><span data-stu-id="b2752-114">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="b2752-115">Ottaa käyttöön Edgen asetukset, jotka auttavat suojaamaan käyttäjiä vahingollisilta sivustoilta ja latauksilta.</span><span class="sxs-lookup"><span data-stu-id="b2752-115">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="b2752-116">Sammuta laitteen näyttö, kun se on ollut käyttämättömänä tämän verran</span><span class="sxs-lookup"><span data-stu-id="b2752-116">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="b2752-p103">Varmistaa, että yritystiedot on suojattu, jos käyttäjä ei tee mitään. Käyttäjä saattaa työskennellä julkisessa paikassa, kuten kahvilassa, ja poistua tai kääntää huomion pois hetkeksi, jolloin laite on alttiina satunnaisille katseille. Tällä asetuksella voit määrittää, miten kauan käyttäjä voi olla toimettomana, ennen kuin näyttö pimenee.</span><span class="sxs-lookup"><span data-stu-id="b2752-p103">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|<span data-ttu-id="b2752-120">Salli käyttäjille sovellusten lataaminen Microsoft Storesta</span><span class="sxs-lookup"><span data-stu-id="b2752-120">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="b2752-p104">Sallii käyttäjien ladata ja asentaa sovelluksia Microsoft Storesta. Sovellukset vaihtelevat peleistä tuottavuustyökaluihin, joten asetus on **käytössä**, mutta voit poistaa sen käytöstä lisäsuojausta varten.  </span><span class="sxs-lookup"><span data-stu-id="b2752-p104">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="b2752-123">Salli käyttäjien käyttää Cortanaa</span><span class="sxs-lookup"><span data-stu-id="b2752-123">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="b2752-124">Cortana-toiminto voi olla hyvin hyödyllinen.</span><span class="sxs-lookup"><span data-stu-id="b2752-124">Cortana can be very helpful!</span></span> <span data-ttu-id="b2752-125">Cortana voi ottaa asetukset käyttöön tai poistaa ne käytöstä, antaa ohjeita ja varmistaa, että olet ajan tasalla tapaamisista, joten pidämme **tämän asetuksen oletuksena** .</span><span class="sxs-lookup"><span data-stu-id="b2752-125">Cortana can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this setting **On** by default.</span></span>  <br/> |
|<span data-ttu-id="b2752-126">Salli käyttäjille Windows-vihjeiden ja -mainosten vastaanottaminen Microsoftilta</span><span class="sxs-lookup"><span data-stu-id="b2752-126">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="b2752-127">Windows-vihjeet voivat olla käteviä ja auttaa perehdyttämään käyttäjiä, kun uusia ominaisuuksia julkaistaan.</span><span class="sxs-lookup"><span data-stu-id="b2752-127">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="b2752-128">Pidä Windows 10 -laitteet ajan tasalla automaattisesti</span><span class="sxs-lookup"><span data-stu-id="b2752-128">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="b2752-129">Varmistaa, että Windows 10 -laitteet vastaanottavat automaattisesti päivityksiä.</span><span class="sxs-lookup"><span data-stu-id="b2752-129">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
   

