---
title: Ehdollisen käytön käytäntöjen määrittäminen Microsoft 365 -kampanjoille
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- MiniMaven
- MSB365
- OKR_SMB_M365
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
description: Lue tietoja ehdollisen käytön käytäntöjen määrittämisestä Microsoft 365 -kampanjoille, jotta voit lisätä huomattavaa lisäsuojausta.
ms.openlocfilehash: be3ca0da3d27e3ec49f1227e4482cfd7fcaae8cb
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550073"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="e30f1-103">Ehdollisen käytön käytäntöjen määrittäminen</span><span class="sxs-lookup"><span data-stu-id="e30f1-103">Set up conditional access policies</span></span>

<span data-ttu-id="e30f1-104">[Ehdollisen käytön](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) käytännöt lisäävät huomattavasti lisäsuojausta.</span><span class="sxs-lookup"><span data-stu-id="e30f1-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="e30f1-105">Microsoft tarjoaa joukon perustason ehdollisia käyttökäytäntöjä, joita suositellaan kaikille asiakkaille.</span><span class="sxs-lookup"><span data-stu-id="e30f1-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="e30f1-106">Perusaikataulun käytännöt ovat joukko ennalta määritettyjä käytäntöjä, jotka auttavat suojaamaan organisaatioita monilta yleisiltä hyökkäyksiltä.</span><span class="sxs-lookup"><span data-stu-id="e30f1-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="e30f1-107">Näitä yleisiä hyökkäyksiä voivat olla salasanasuihke, uusinta ja tietojenkalastelu.</span><span class="sxs-lookup"><span data-stu-id="e30f1-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="e30f1-108">Nämä käytännöt edellyttävät, että järjestelmänvalvojat ja käyttäjät kirjoittavat toisen todennusmuodon (monivaiheinen todennus tai mfa), kun tietyt ehdot täyttyvät.</span><span class="sxs-lookup"><span data-stu-id="e30f1-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="e30f1-109">Jos käyttäjä esimerkiksi kirjautuu sisään toisesta maasta, kirjautumista saatetaan pitää riskialttiina ja käyttäjän on annettava lisätodennusmuoto.</span><span class="sxs-lookup"><span data-stu-id="e30f1-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="e30f1-110">Tällä hetkellä perustason käytäntöjä ovat seuraavat:</span><span class="sxs-lookup"><span data-stu-id="e30f1-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="e30f1-111">**Vaadi mfa järjestelmänvalvojille** &ndash; Edellyttää monivaiheista todennusta etuoikeutetuimmille järjestelmänvalvojan rooleille, mukaan lukien yleinen järjestelmänvalvoja.</span><span class="sxs-lookup"><span data-stu-id="e30f1-111">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="e30f1-112">**Loppukäyttäjän suojaus** &ndash; Edellyttää monivaiheista todennusta käyttäjille vain, kun kirjautuminen on riskialtista.</span><span class="sxs-lookup"><span data-stu-id="e30f1-112">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="e30f1-113">**Estä vanha todennus** &ndash; Vanhemmat asiakassovellukset ja jotkin uudet sovellukset eivät käytä uudempia, turvallisempia todennusprotokollia.</span><span class="sxs-lookup"><span data-stu-id="e30f1-113">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="e30f1-114">Nämä vanhemmat sovellukset voivat ohittaa ehdollisen käytön käytännöt ja saada luvattoman pääsyn ympäristöösi.</span><span class="sxs-lookup"><span data-stu-id="e30f1-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="e30f1-115">Tämä käytäntö estää pääsyn asiakkailta, jotka eivät tue ehdollista käyttöoikeutta.</span><span class="sxs-lookup"><span data-stu-id="e30f1-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="e30f1-116">**Vaadi mfa palvelunhallintaa** &ndash; edellyttää monivaiheista todennusta hallintatyökalujen, kuten Azure-portaalin (jossa perusaikataulun käytännöt määritetään).</span><span class="sxs-lookup"><span data-stu-id="e30f1-116">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="e30f1-117">Microsoft suosittelee, että otat käyttöön kaikki nämä perusaikataulun käytännöt.</span><span class="sxs-lookup"><span data-stu-id="e30f1-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="e30f1-118">Kun nämä käytännöt on otettu käyttöön, järjestelmänvalvojia ja käyttäjiä pyydetään rekisteröitymään Azure Multii-Factor -todennusta varten.</span><span class="sxs-lookup"><span data-stu-id="e30f1-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="e30f1-119">Lisätietoja näistä käytännöistä on ohjeaiheessa [Mitä ovat perustason käytännöt?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)</span><span class="sxs-lookup"><span data-stu-id="e30f1-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="e30f1-120">Perusaikataulun käytäntöjen määrittäminen</span><span class="sxs-lookup"><span data-stu-id="e30f1-120">Set up baseline policies</span></span>

1. <span data-ttu-id="e30f1-121">Siirry [Azure-portaaliin](https://portal.azure.com)ja siirry sitten **Azure Active Directoryn** \> **ehdolliseen käyttöön**.</span><span class="sxs-lookup"><span data-stu-id="e30f1-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="e30f1-122">Perusaikataulun käytännöt näkyvät sivulla.</span><span class="sxs-lookup"><span data-stu-id="e30f1-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="e30f1-123">![Sivu, jossa on luettelo ehdollisen käytön perusaikataulun käytännöistä.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="e30f1-123">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="e30f1-124">Katso seuraavat tarkat ohjeet kustakin käytännöstä:</span><span class="sxs-lookup"><span data-stu-id="e30f1-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="e30f1-125">Vaadi mfa ylläpitäjät</span><span class="sxs-lookup"><span data-stu-id="e30f1-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="e30f1-126">Vaadi mfa käyttäjille</span><span class="sxs-lookup"><span data-stu-id="e30f1-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="e30f1-127">Estä vanha todennus</span><span class="sxs-lookup"><span data-stu-id="e30f1-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="e30f1-128">Vaadi mfa palvelunhallintaan</span><span class="sxs-lookup"><span data-stu-id="e30f1-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="e30f1-129">Voit määrittää useita lisäkäytäntöjä, kuten edellyttää hyväksyttyjä asiakassovelluksia.</span><span class="sxs-lookup"><span data-stu-id="e30f1-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="e30f1-130">Lisätietoja on [ehdollisen käytön dokumentaatiossa](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="e30f1-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
