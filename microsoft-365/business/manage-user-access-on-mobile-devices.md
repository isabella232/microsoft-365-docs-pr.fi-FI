---
title: Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4OfficeMobile
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
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
description: Lue lisä tietoja suojaus käytännöistä, joiden avulla voit suojata Office-sovellusten käyttö oikeudet mobiililaitteilla.
ms.openlocfilehash: 39d28a3a78fb06d0020c484b1782b544f6a8c656
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593817"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="c811d-103">Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa</span><span class="sxs-lookup"><span data-stu-id="c811d-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="c811d-104">Käytäntöasetukset, jotka määrittävät, miten käyttäjät voivat käyttää Office-tiedostojen mobiililaitteillaan, ovat oletuksena **pois käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="c811d-104">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="c811d-105">Microsoft suosittelee, että hyväksyt oletus arvot asennuksen aikana, jotta voit luoda sovellus käytäntöjä Androidille, iOS:lle ja Windows 10: lle, jotka koskevat kaikkia käyttäjiä.</span><span class="sxs-lookup"><span data-stu-id="c811d-105">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="c811d-106">Voit luoda lisää käytäntöjä asennuksen päätyttyä.</span><span class="sxs-lookup"><span data-stu-id="c811d-106">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="c811d-107">Asetukset, joilla hallitaan käyttäjien Office-tiedostojen käyttöä mobiililaitteilla</span><span class="sxs-lookup"><span data-stu-id="c811d-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="c811d-108">Käyttäjien Office-työtiedostojen käyttöä voidaan hallita seuraavilla asetuksilla:</span><span class="sxs-lookup"><span data-stu-id="c811d-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="c811d-109">Asetus</span><span class="sxs-lookup"><span data-stu-id="c811d-109">Setting</span></span>  <br/> |<span data-ttu-id="c811d-110">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="c811d-110">Description</span></span>  <br/> |
|<span data-ttu-id="c811d-111">Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä</span><span class="sxs-lookup"><span data-stu-id="c811d-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="c811d-112">Jos tämä asetus on **käytössä**, käyttäjien on annettava toinen todennus muoto käyttäjä nimen ja Sala sanan lisäksi, ennen kuin he voivat käyttää Office-sovelluksia mobiililaitteellasi.</span><span class="sxs-lookup"><span data-stu-id="c811d-112">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="c811d-113">Palauta PIN-koodi, jos kirjautuminen epäonnistuu näin monta kertaa</span><span class="sxs-lookup"><span data-stu-id="c811d-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="c811d-114">Jos haluat estää luvatonta käyttäjä arvaamasta PIN-koodia sattumalta, PIN-koodi palautetaan määrittämäsi virheellisten syöttökertojen määrän jälkeen.</span><span class="sxs-lookup"><span data-stu-id="c811d-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="c811d-115">Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä</span><span class="sxs-lookup"><span data-stu-id="c811d-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="c811d-116">Tämä asetus määrittää, kuinka kauan käyttäjä voi olla käyttämättömänä, ennen kuin häntä pyydetään Kirjautu maan uudelleen sisään.</span><span class="sxs-lookup"><span data-stu-id="c811d-116">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="c811d-117">Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu</span><span class="sxs-lookup"><span data-stu-id="c811d-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="c811d-118">Kekseliäällä käyttäjällä voi olla laite, jonka suojaus on murrettu.</span><span class="sxs-lookup"><span data-stu-id="c811d-118">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="c811d-119">Tämä tarkoittaa, että käyttäjä voi muokata käyttö järjestelmää, joka voi tehdä laitteesta alttiimpi haitta ohjelmille.</span><span class="sxs-lookup"><span data-stu-id="c811d-119">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="c811d-120">Tällaiset laitteet on estetty, kun tämä asetus on **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="c811d-120">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="c811d-121">Älä salli käyttäjien kopioida sisältöä Office-sovelluksista omiin sovelluksiin</span><span class="sxs-lookup"><span data-stu-id="c811d-121">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="c811d-122">Kun asetus on **käytössä**, käyttäjä ei voi kopioida työtiedoston tietoja henkilökohtaiseen tiedostoon.</span><span class="sxs-lookup"><span data-stu-id="c811d-122">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="c811d-123">Jos asetus on **poissa käytöstä**, käyttäjä voi kopioida tietoja työtiedostosta henkilökohtaiseen sovellukseen tai henkilökohtaiseen tiliin.</span><span class="sxs-lookup"><span data-stu-id="c811d-123">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

