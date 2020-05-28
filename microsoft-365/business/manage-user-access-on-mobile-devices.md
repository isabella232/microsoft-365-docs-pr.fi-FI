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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Lue tietoja suojauskäytännöistä, joiden avulla voit hallita sitä, miten käyttäjät käyttävät Office-sovelluksia ja työtiedostoja mobiililaitteista.
ms.openlocfilehash: f613e518c3607010cae55443456be9d3ddc3d689
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403074"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="faab3-103">Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa</span><span class="sxs-lookup"><span data-stu-id="faab3-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="faab3-104">Käytäntöasetukset, jotka määrittävät, miten käyttäjät voivat käyttää Office-tiedostojen mobiililaitteillaan, ovat oletuksena **pois käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="faab3-104">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="faab3-105">Suosittelemme, että hyväksyt oletusarvot asennuksen aikana luodaksesi sovelluskäytäntöjä Androidille, iOS:lle ja Windows 10:lle, jotka koskevat kaikkia käyttäjiä.</span><span class="sxs-lookup"><span data-stu-id="faab3-105">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="faab3-106">Voit luoda lisää käytäntöjä asennuksen päätyttyä.</span><span class="sxs-lookup"><span data-stu-id="faab3-106">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="faab3-107">Asetukset, joilla hallitaan käyttäjien Office-tiedostojen käyttöä mobiililaitteilla</span><span class="sxs-lookup"><span data-stu-id="faab3-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="faab3-108">Käyttäjien Office-työtiedostojen käyttöä voidaan hallita seuraavilla asetuksilla:</span><span class="sxs-lookup"><span data-stu-id="faab3-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="faab3-109">Asetus</span><span class="sxs-lookup"><span data-stu-id="faab3-109">Setting</span></span>  <br/> |<span data-ttu-id="faab3-110">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="faab3-110">Description</span></span>  <br/> |
|<span data-ttu-id="faab3-111">Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä</span><span class="sxs-lookup"><span data-stu-id="faab3-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="faab3-112">Jos tämä asetus on **Käytössä**, käyttäjien on annettava toinen todennusmuoto käyttäjätunnuksensa ja salasanansa lisäksi, ennen kuin he voivat käyttää Office-sovelluksia mobiililaitteessaan.</span><span class="sxs-lookup"><span data-stu-id="faab3-112">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="faab3-113">Palauta PIN-koodi, jos kirjautuminen epäonnistuu näin monta kertaa</span><span class="sxs-lookup"><span data-stu-id="faab3-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="faab3-114">Jos haluat estää luvatonta käyttäjä arvaamasta PIN-koodia sattumalta, PIN-koodi palautetaan määrittämäsi virheellisten syöttökertojen määrän jälkeen.</span><span class="sxs-lookup"><span data-stu-id="faab3-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="faab3-115">Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä</span><span class="sxs-lookup"><span data-stu-id="faab3-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="faab3-116">Tämä asetus määrittää, kuinka kauan käyttäjä voi olla käyttämättömänä, ennen kuin häntä kehotetaan kirjautumaan uudelleen sisään.</span><span class="sxs-lookup"><span data-stu-id="faab3-116">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="faab3-117">Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu</span><span class="sxs-lookup"><span data-stu-id="faab3-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="faab3-118">Kekseliäällä käyttäjällä voi olla laite, jonka suojaus on murrettu.</span><span class="sxs-lookup"><span data-stu-id="faab3-118">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="faab3-119">Tämä tarkoittaa, että käyttäjä voi muokata käyttöjärjestelmää, joka voi tehdä laitteesta alttiimman haittaohjelmille.</span><span class="sxs-lookup"><span data-stu-id="faab3-119">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="faab3-120">Tällaiset laitteet on estetty, kun tämä asetus on **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="faab3-120">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="faab3-121">Älä salli käyttäjien kopioida sisältöä Office-sovelluksista henkilökohtaisiin sovelluksiin</span><span class="sxs-lookup"><span data-stu-id="faab3-121">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="faab3-122">Kun asetus on **Käytössä**, käyttäjä ei voi kopioida työtiedoston tietoja henkilökohtaiseen tiedostoon.</span><span class="sxs-lookup"><span data-stu-id="faab3-122">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="faab3-123">Jos asetus on **Ei käytössä**, käyttäjä voi kopioida tietoja työtiedostosta henkilökohtaiseen sovellukseen tai henkilökohtaiseen tiliin.</span><span class="sxs-lookup"><span data-stu-id="faab3-123">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

