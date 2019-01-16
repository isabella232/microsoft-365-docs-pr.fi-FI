---
title: Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa
ms.author: sirkkuw
author: sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
f1_keywords:
- 'O365E_BCSSetup4OfficeMobile '
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Lisätietoja suojaus käytännöt, joiden avulla suojatun access Office apps, mobiililaitteista.
ms.openlocfilehash: 75dbe79acccabd851c43259a165e79bfe3c509c0
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983183"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="d4373-103">Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa</span><span class="sxs-lookup"><span data-stu-id="d4373-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="d4373-p101">Käytäntöasetukset, jotka määrittävät, miten käyttäjät voivat käyttää Office-tiedostojen mobiililaitteillaan, ovat oletuksena **pois käytöstä**. On suositeltavaa hyväksyä oletusarvot asennuksen aikana kaikkia käyttäjiä koskevien sovelluskäytäntöjen luomiseksi Androidille, iOS:lle ja Windows 10:lle. Voit luoda lisää käytäntöjä asennuksen päätyttyä.</span><span class="sxs-lookup"><span data-stu-id="d4373-p101">Policy settings that control how users access Office files from their mobile devices are **Off** by default. We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users. You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="d4373-107">Asetukset, joilla hallitaan käyttäjien Office-tiedostojen käyttöä mobiililaitteilla</span><span class="sxs-lookup"><span data-stu-id="d4373-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="d4373-108">Käyttäjien Office-työtiedostojen käyttöä voidaan hallita seuraavilla asetuksilla:</span><span class="sxs-lookup"><span data-stu-id="d4373-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="d4373-109">Asetus</span><span class="sxs-lookup"><span data-stu-id="d4373-109">Setting</span></span>  <br/> |<span data-ttu-id="d4373-110">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="d4373-110">Description</span></span>  <br/> |
|<span data-ttu-id="d4373-111">Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä</span><span class="sxs-lookup"><span data-stu-id="d4373-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="d4373-112">Jos tämä asetus on **käytössä**, käyttäjien on annettava toinen todennusmuoto käyttäjänimensä ja salasanansa lisäksi, ennen kuin he voivat käyttää Office-sovelluksia mobiililaitteillaan.</span><span class="sxs-lookup"><span data-stu-id="d4373-112">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="d4373-113">Palauta PIN-koodi, jos kirjautuminen epäonnistuu näin monta kertaa</span><span class="sxs-lookup"><span data-stu-id="d4373-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="d4373-114">Jos haluat estää luvatonta käyttäjää arvaamasta PIN-koodia sattumalta, PIN-koodi palautetaan määrittämäsi virheellisten syöttökertojen määrän jälkeen.</span><span class="sxs-lookup"><span data-stu-id="d4373-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="d4373-115">Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä</span><span class="sxs-lookup"><span data-stu-id="d4373-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="d4373-116">Tämä asetus määrittää, kuinka kauan käyttäjä voi olla toimimatta, ennen kuin häntä kehotetaan kirjautumaan sisään uudelleen.</span><span class="sxs-lookup"><span data-stu-id="d4373-116">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="d4373-117">Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu</span><span class="sxs-lookup"><span data-stu-id="d4373-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="d4373-p102">Kekseliäällä käyttäjällä voi olla laite, jonka suojaus on murrettu. Tämä tarkoittaa, että käyttäjä voi muokata käyttöjärjestelmää, minkä vuoksi laite voi altistua helpommin haittaohjelmille. Tällaiset laitteet on estetty, kun tämä asetus on **käytössä**.  </span><span class="sxs-lookup"><span data-stu-id="d4373-p102">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="d4373-121">Salli käyttäjille sisällön kopiointi Office-sovelluksista henkilökohtaisiin sovelluksiin</span><span class="sxs-lookup"><span data-stu-id="d4373-121">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="d4373-p103">Oletuksena tämä sallitaan, mutta kun asetus on **käytössä**, käyttäjä voi kopioida työtiedoston tietoja henkilökohtaiseen tiedostoon. Jos asetus on **pois käytöstä**, käyttäjä ei voi kopioida tietoja työtiedostosta henkilökohtaiseen sovellukseen tai henkilökohtaisen tiliin.  </span><span class="sxs-lookup"><span data-stu-id="d4373-p103">We allow this by default, but when the setting is **On**, the user can copy information in a work file to a personal file. If the setting is **Off**, the user can't copy information from a work file to a personal app or personal account.  </span></span><br/> |
   

