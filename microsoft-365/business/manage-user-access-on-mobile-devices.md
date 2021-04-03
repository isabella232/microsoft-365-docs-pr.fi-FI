---
title: Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Lue lisää suojauskäytännöistä, joiden avulla voit hallita sitä, miten käyttäjät voivat käyttää Office-sovelluksia ja työtiedostoja mobiililaitteista.
ms.openlocfilehash: a48aa241c9e70cf087da3f1701e859dae7238024
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578383"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="f8dff-103">Käyttäjien Office-tiedostojen käytön hallinta mobiililaitteissa</span><span class="sxs-lookup"><span data-stu-id="f8dff-103">Manage how users access Office documents on mobile devices</span></span>

<span data-ttu-id="f8dff-104">Tämä artikkeli koskee Microsoft 365 Business Premiumia.</span><span class="sxs-lookup"><span data-stu-id="f8dff-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="f8dff-105">Käytäntöasetukset, jotka määrittävät, miten käyttäjät voivat käyttää Office-tiedostojen mobiililaitteillaan, ovat oletuksena **pois käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="f8dff-105">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="f8dff-106">Suosittelemme, että hyväksyt oletusarvot asennuksen aikana, jotta voit luoda android-, iOS- ja Windows 10 -sovelluskäytäntöjä, jotka koskevat kaikkia käyttäjiä.</span><span class="sxs-lookup"><span data-stu-id="f8dff-106">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="f8dff-107">Voit luoda lisää käytäntöjä asennuksen päätyttyä.</span><span class="sxs-lookup"><span data-stu-id="f8dff-107">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="f8dff-108">Asetukset, joilla hallitaan käyttäjien Office-tiedostojen käyttöä mobiililaitteilla</span><span class="sxs-lookup"><span data-stu-id="f8dff-108">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="f8dff-109">Käyttäjien Office-työtiedostojen käyttöä voidaan hallita seuraavilla asetuksilla:</span><span class="sxs-lookup"><span data-stu-id="f8dff-109">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="f8dff-110">Asetus</span><span class="sxs-lookup"><span data-stu-id="f8dff-110">Setting</span></span>  <br/> |<span data-ttu-id="f8dff-111">Kuvaus</span><span class="sxs-lookup"><span data-stu-id="f8dff-111">Description</span></span>  <br/> |
|<span data-ttu-id="f8dff-112">Office-sovellusten käyttäminen edellyttää PIN-koodia tai sormenjälkeä</span><span class="sxs-lookup"><span data-stu-id="f8dff-112">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="f8dff-113">Jos tämä asetus **on käytössä,** käyttäjien on annettava toinen todennusmuoto käyttäjänimen ja salasanan lisäksi, ennen kuin he voivat käyttää Office-sovelluksia mobiililaitteessa.</span><span class="sxs-lookup"><span data-stu-id="f8dff-113">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="f8dff-114">Palauta PIN-koodi, jos kirjautuminen epäonnistuu näin monta kertaa</span><span class="sxs-lookup"><span data-stu-id="f8dff-114">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="f8dff-115">Jos haluat estää luvatonta käyttäjä arvaamasta PIN-koodia sattumalta, PIN-koodi palautetaan määrittämäsi virheellisten syöttökertojen määrän jälkeen.</span><span class="sxs-lookup"><span data-stu-id="f8dff-115">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="f8dff-116">Vaadi käyttäjää kirjautumaan uudelleen, jos Office-sovellukset ovat olleet käyttämättöminä</span><span class="sxs-lookup"><span data-stu-id="f8dff-116">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="f8dff-117">Tämä asetus määrittää, kuinka kauan käyttäjä voi olla käyttämättömänä, ennen kuin häntä pyydetään kirjautumaan uudelleen sisään.</span><span class="sxs-lookup"><span data-stu-id="f8dff-117">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="f8dff-118">Estä työtiedostojen käyttö laitteissa, joiden suojaukset on murrettu</span><span class="sxs-lookup"><span data-stu-id="f8dff-118">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="f8dff-119">Kekseliäällä käyttäjällä voi olla laite, jonka suojaus on murrettu.</span><span class="sxs-lookup"><span data-stu-id="f8dff-119">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="f8dff-120">Tämä tarkoittaa, että käyttäjä voi muokata käyttöjärjestelmää, mikä voi tehdä laitteesta altis haittaohjelmille.</span><span class="sxs-lookup"><span data-stu-id="f8dff-120">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="f8dff-121">Tällaiset laitteet on estetty, kun tämä asetus on **käytössä**.</span><span class="sxs-lookup"><span data-stu-id="f8dff-121">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="f8dff-122">Älä salli käyttäjien kopioida sisältöä Office-sovelluksista henkilökohtaisiin sovelluksiin</span><span class="sxs-lookup"><span data-stu-id="f8dff-122">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="f8dff-123">Kun asetus **on Käytössä,** käyttäjä ei voi kopioida työtiedoston tietoja henkilökohtaiseen tiedostoon.</span><span class="sxs-lookup"><span data-stu-id="f8dff-123">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="f8dff-124">Jos asetus on **Ei käytössä,** käyttäjä voi kopioida tietoja työtiedostosta henkilökohtaiseen sovellukseen tai henkilökohtaiseen tiliin.</span><span class="sxs-lookup"><span data-stu-id="f8dff-124">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

