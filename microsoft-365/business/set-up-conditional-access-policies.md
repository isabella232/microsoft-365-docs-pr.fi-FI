---
title: Ehdollisen käyttöoikeuden Microsoft 365 kampanjoiden käytäntöjen määrittäminen
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
search.appverid:
- BCS160
- MET150
- MOE150
description: Tietoja ehdollisen käyttöoikeuden käytäntöjen määrittäminen Microsoft 365 kampanjoita.
ms.openlocfilehash: 7d8e1f16019d151478aae57b1593b0e0758e5b19
ms.sourcegitcommit: 7e46db0b35c188ee6a7b40ab3eb2d76ff6c101c5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/19/2019
ms.locfileid: "35086321"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="bfe64-103">Ehdollisen käyttöoikeuden käytäntöjen määrittäminen</span><span class="sxs-lookup"><span data-stu-id="bfe64-103">Set up conditional access policies</span></span>

<span data-ttu-id="bfe64-104">[Ehdollisen käyttöoikeuden](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) käytäntöjä lisätä substancial suojausta.</span><span class="sxs-lookup"><span data-stu-id="bfe64-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="bfe64-105">Microsoft tarjoaa joukon perusaikataulun ehdollisen käyttöoikeuden käytäntöjä, joita suositellaan kaikille asiakkaille.</span><span class="sxs-lookup"><span data-stu-id="bfe64-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="bfe64-106">Perusaikataulun käytännöt ovat valmiita käytäntöjä, jotka suojaavat hyökkäyksiltä monia yhteisiä organisaatioita.</span><span class="sxs-lookup"><span data-stu-id="bfe64-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="bfe64-107">Yleisiä nämä hyökkäykset voivat olla salasana ruiskun, replay ja phishing.</span><span class="sxs-lookup"><span data-stu-id="bfe64-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="bfe64-108">Nämä käytännöt edellyttävät Järjestelmänvalvojat ja käyttäjät voivat syöttää toisen lomakkeen todennusta (jota kutsutaan useaan tekijään perustuvan todennuksen tai MFA) kun tietyt ehdot täyttyvät.</span><span class="sxs-lookup"><span data-stu-id="bfe64-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="bfe64-109">Esimerkiksi jos käyttäjä sisään eri maasta, kirjautumissivulta voidaan harkita riskialtis ja käyttäjän on annettava todennusta uuden lomakkeen.</span><span class="sxs-lookup"><span data-stu-id="bfe64-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="bfe64-110">Perusaikataulun käytännöt ovat tällä hetkellä seuraavat:</span><span class="sxs-lookup"><span data-stu-id="bfe64-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="bfe64-111">**MFA edellyttävät järjestelmänvalvojat** – edellyttää monitasoisen todennuksen ensisijaisessa järjestelmänvalvoja-roolien mukaan lukien Yleinen järjestelmänvalvoja.</span><span class="sxs-lookup"><span data-stu-id="bfe64-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="bfe64-112">**Käyttäjän suojaus** — vaatii monitasoisen todennuksen käyttäjille vain, kun jokin merkki on riskialtista.</span><span class="sxs-lookup"><span data-stu-id="bfe64-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="bfe64-113">**Vanhan mallin mukainen todennus estää** — vanhemmat asiakassovellukset ja joitakin uusia apps et käytä uudempia, turvallisempia, todennusprotokollia.</span><span class="sxs-lookup"><span data-stu-id="bfe64-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="bfe64-114">Nämä vanhat apps voit ohittaa ehdollisen käyttöoikeuden käytäntöjä ja ympäristön yrityksiin hankkia luvaton pääsy.</span><span class="sxs-lookup"><span data-stu-id="bfe64-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="bfe64-115">Tämä käytäntö estää käytön asiakkailta, jotka eivät tue ehdollisen käyttöoikeuden.</span><span class="sxs-lookup"><span data-stu-id="bfe64-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="bfe64-116">**Huoltohallinnan edellyttävät MFA** — monitasoisen todennuksen vaatii pääsyä hallintatyökaluihin, mukaan lukien Azure portal (jossa voit määrittää perusaikataulun käytännöt).</span><span class="sxs-lookup"><span data-stu-id="bfe64-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="bfe64-117">Microsoft suosittelee, että otat kaikki nämä käytännöt perusaikataulun.</span><span class="sxs-lookup"><span data-stu-id="bfe64-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="bfe64-118">Kun nämä käytännöt on otettu käyttöön, järjestelmänvalvojat- ja käyttäjät pyydetään rekisteröitymään Multii Azure-tekijä authentication.</span><span class="sxs-lookup"><span data-stu-id="bfe64-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="bfe64-119">Lisätietoja näistä käytännöistä Katso [mitä perusaikataulun käytännöt ovat](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="bfe64-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="bfe64-120">Perusaikataulun käytäntöjen määrittäminen</span><span class="sxs-lookup"><span data-stu-id="bfe64-120">Set up baseline policies</span></span>

1. <span data-ttu-id="bfe64-121">Siirry [Azure portal](https://portal.azure.com)ja siirry **Azure Active Directory** \> **Ehdollisen käyttöoikeuden**.</span><span class="sxs-lookup"><span data-stu-id="bfe64-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="bfe64-122">Perusaikataulun käytännöt on lueteltu sivulla.</span><span class="sxs-lookup"><span data-stu-id="bfe64-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="bfe64-123">![Ehdollisen käyttöoikeuden käytäntöjä perusaikataulun sisältävällä sivulla.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="bfe64-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="bfe64-124">Lisätietoja käytäntöjen seuraavat ohjeet:</span><span class="sxs-lookup"><span data-stu-id="bfe64-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="bfe64-125">MFA edellyttävät Järjestelmänvalvojat</span><span class="sxs-lookup"><span data-stu-id="bfe64-125">Require MFA for admins</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="bfe64-126">Reequire MFA-käyttäjille</span><span class="sxs-lookup"><span data-stu-id="bfe64-126">Reequire MFA for users</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="bfe64-127">Estä vanhan mallin mukainen todennus</span><span class="sxs-lookup"><span data-stu-id="bfe64-127">Block legacy authentication</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="bfe64-128">Vaadi MFA hallinta</span><span class="sxs-lookup"><span data-stu-id="bfe64-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="bfe64-129">Voit määrittää useita muita käytäntöjä esimerkiksi asiakkaan hyväksytyn apps.</span><span class="sxs-lookup"><span data-stu-id="bfe64-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="bfe64-130">Katso lisätietoja [Ehdollinen Access in ohjeista](https://docs.microsoft.com/azure/active-directory/conditional-access/) .</span><span class="sxs-lookup"><span data-stu-id="bfe64-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>