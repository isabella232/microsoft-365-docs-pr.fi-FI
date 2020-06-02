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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Lue tietoja siitä, miten voit määrittää Ehdollisen käytön käytännöt Microsoft 365 -kampanjoille, jotta voit lisätä huomattavasti lisäsuojaa.
ms.openlocfilehash: 58ee760877ee2fd7e53ef9463242657ab66a2b6e
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470643"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="09d52-103">Ehdollisen käytön käytäntöjen määrittäminen</span><span class="sxs-lookup"><span data-stu-id="09d52-103">Set up conditional access policies</span></span>

<span data-ttu-id="09d52-104">Tämä artikkeli koskee Microsoft 365 Business Premiumia.</span><span class="sxs-lookup"><span data-stu-id="09d52-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="09d52-105">[Ehdollisen käytön](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) käytännöt lisäävät huomattavaa lisäsuojaa.</span><span class="sxs-lookup"><span data-stu-id="09d52-105">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="09d52-106">Microsoft issa on joukko ehdollisen käytön peruskäytäntöjä, joita suositellaan kaikille asiakkaille.</span><span class="sxs-lookup"><span data-stu-id="09d52-106">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="09d52-107">Perusaikataulun käytännöt ovat joukko ennalta määritettyjä käytäntöjä, jotka auttavat suojaamaan organisaatioita monilta yleisiltä hyökkäyksiltä.</span><span class="sxs-lookup"><span data-stu-id="09d52-107">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="09d52-108">Näitä yleisiä hyökkäyksiä voivat olla salasanasumute, uusinta ja tietojenkalastelu.</span><span class="sxs-lookup"><span data-stu-id="09d52-108">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="09d52-109">Nämä käytännöt edellyttävät, että järjestelmänvalvojat ja käyttäjät kirjoittavat toisen todennuksen muodon (multifactor-todennuksen tai mfa-menetelmän), kun tietyt ehdot täyttyvät.</span><span class="sxs-lookup"><span data-stu-id="09d52-109">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="09d52-110">Jos käyttäjä esimerkiksi kirjautuu sisään toisesta maasta, sisäänkirjautumista voidaan pitää riskialttiina ja käyttäjän on annettava lisätodennuksen muoto.</span><span class="sxs-lookup"><span data-stu-id="09d52-110">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="09d52-111">Tällä hetkellä perusaikataulun käytännöt sisältävät seuraavat:</span><span class="sxs-lookup"><span data-stu-id="09d52-111">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="09d52-112">**Vaadi MFA järjestelmänvalvojille** &ndash; Edellyttää monivaiheista todennusta etuoikeutetummille järjestelmänvalvojan rooleille, myös yleiselle järjestelmänvalvojalle.</span><span class="sxs-lookup"><span data-stu-id="09d52-112">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="09d52-113">**Loppukäyttäjän suojaus** &ndash; Edellyttää monivaiheista todennusta käyttäjille vain, kun kirjautuminen on riskialtista.</span><span class="sxs-lookup"><span data-stu-id="09d52-113">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="09d52-114">**Estä vanha todennus** &ndash; Vanhemmat asiakassovellukset ja jotkin uudet sovellukset eivät käytä uudempia, turvallisempia todennusprotokollia.</span><span class="sxs-lookup"><span data-stu-id="09d52-114">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="09d52-115">Nämä vanhemmat sovellukset voivat ohittaa ehdollisen käytön käytännöt ja käyttää ympäristöäsi luvatta.</span><span class="sxs-lookup"><span data-stu-id="09d52-115">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="09d52-116">Tämä käytäntö estää pääsyn asiakkailta, jotka eivät tue ehdollista käyttöä.</span><span class="sxs-lookup"><span data-stu-id="09d52-116">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="09d52-117">**Vaadi MFA palvelunhallintaa** &ndash; varten Edellyttää monivaiheista todennusta hallintatyökalujen, kuten Azure-portaalin (jossa perusaikataulun käytännöt määritetään) käyttöä varten.</span><span class="sxs-lookup"><span data-stu-id="09d52-117">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="09d52-118">Microsoft suosittelee, että otat käyttöön kaikki nämä perusaikataulun käytännöt.</span><span class="sxs-lookup"><span data-stu-id="09d52-118">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="09d52-119">Kun nämä käytännöt on otettu käyttöön, järjestelmänvalvojia ja käyttäjiä pyydetään rekisteröitymään Azure Multii-Factor -todennukseen.</span><span class="sxs-lookup"><span data-stu-id="09d52-119">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="09d52-120">Lisätietoja näistä käytännöistä on kohdassa [Mitä ovat perusaikataulun käytännöt?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)</span><span class="sxs-lookup"><span data-stu-id="09d52-120">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="09d52-121">Perusaikataulun käytäntöjen määrittäminen</span><span class="sxs-lookup"><span data-stu-id="09d52-121">Set up baseline policies</span></span>

1. <span data-ttu-id="09d52-122">Siirry [Azure-portaaliin](https://portal.azure.com)ja siirry sitten **Azure Active** \> **Directoryn ehdolliseen käyttöön**.</span><span class="sxs-lookup"><span data-stu-id="09d52-122">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="09d52-123">Perusaikataulun käytännöt näkyvät sivulla.</span><span class="sxs-lookup"><span data-stu-id="09d52-123">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="09d52-124">![Sivu, jossa on luettelo ehdollisen käytön perusaikataulun käytännöistä.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="09d52-124">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="09d52-125">Katso seuraavat kunkin käytännön ohjeet:</span><span class="sxs-lookup"><span data-stu-id="09d52-125">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="09d52-126">Vaadi MFA järjestelmänvalvojille</span><span class="sxs-lookup"><span data-stu-id="09d52-126">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="09d52-127">Vaadi mfa käyttäjille</span><span class="sxs-lookup"><span data-stu-id="09d52-127">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="09d52-128">Estä vanha todennus</span><span class="sxs-lookup"><span data-stu-id="09d52-128">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="09d52-129">Vaadi mfa palvelunhallintaa varten</span><span class="sxs-lookup"><span data-stu-id="09d52-129">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="09d52-130">Voit määrittää useita lisäkäytäntöjä, kuten hyväksyttyjen asiakassovellusten vaatimista.</span><span class="sxs-lookup"><span data-stu-id="09d52-130">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="09d52-131">Lisätietoja on [Ehdollisen käytön ohjeissa](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="09d52-131">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
