---
title: Ehdollisten käyttö oikeus käytäntöjen määrittäminen Microsoft 365-kampanjoille
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
description: Lue lisä tietoja ehdollisten käyttö käytäntöjen määrittämisestä Microsoft 365-kampanjoille.
ms.openlocfilehash: 614e3a6e13a14114f40ecf87bf936d4165744503
ms.sourcegitcommit: 91ff1d4339f0f043c2b43997d87d84677c79e279
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2019
ms.locfileid: "36982377"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="aa5b0-103">Määritä ehdolliset käyttö oikeus käytännöt</span><span class="sxs-lookup"><span data-stu-id="aa5b0-103">Set up conditional access policies</span></span>

<span data-ttu-id="aa5b0-104">[Ehdollisen käytön käytännöt lisäävät aineeksi](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) lisä suojausta.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="aa5b0-105">Microsoft tarjoaa perusaikataulun ehdollisten käyttö oikeus käytäntöjen joukon, jota suositellaan kaikille asiakkaille.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="aa5b0-106">Perusaikataulun käytännöt ovat joukko esimääritettyjä käytäntöjä, jotka auttavat suojaamaan organisaatioita monista yleisistä hyökkäyksistä.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="aa5b0-107">Näitä yleisiä hyökkäyksiä voivat olla Sala sanan suihkutus, uusinta toisto ja tietojenkalastelu.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="aa5b0-108">Nämä käytännöt edellyttävät, että järjestelmänvalvojat ja käyttäjät syöttäisivät toisen todennus muodon (jota kutsutaan nimellä Monivaiheinen todennus tai MFA), kun tietyt ehdot täyttyvät.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="aa5b0-109">Jos käyttäjä on esimerkiksi kirjauduttava sisään toisesta maasta, kirjautumista voidaan pitää riskialttiina ja käyttäjän on annettava lisä todennus muoto.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="aa5b0-110">Tällä hetkellä perusaikataulun käytäntöjä ovat seuraavat:</span><span class="sxs-lookup"><span data-stu-id="aa5b0-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="aa5b0-111">**Vaadi järjestelmänvalvojien makrotaloudellinen** tuki – vaatii usean tekijän todennuksen suosituimmille järjestelmänvalvojan rooleille, mukaan lukien yleinen järjestelmänvalvoja.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="aa5b0-112">**Loppu käyttäjän suojaus** – vaatii usean tekijän todennuksen käyttäjille vain silloin, kun kirjautuminen on riskialtista.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="aa5b0-113">**Estä aiempi todennus** – vanhemmat asiakas sovellukset ja jotkin uudet sovellukset eivät käytä uudempia, turvallisempia todennus protokollia.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="aa5b0-114">Nämä vanhemmat sovellukset voivat ohittaa ehdolliset käyttö käytännöt ja käyttää ympäristöäsi luvattomasti.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="aa5b0-115">Tämä käytäntö estää pääsyn asiakkailta, jotka eivät tue ehdollista pääsyä.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="aa5b0-116">**Vaadi palvelun hallinnan MFA-tuki** – vaatii monivaiheisen todennuksen hallinta työkalujen, kuten Azure-portaalin, käyttöä varten (Jos määrität peruskäytännöt).</span><span class="sxs-lookup"><span data-stu-id="aa5b0-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="aa5b0-117">Microsoft suosittelee, että otat kaikki nämä perusaikataulun käytännöt käyttöön.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="aa5b0-118">Kun nämä käytännöt on otettu käyttöön, ylläpitäjiä ja käyttäjiä kehotetaan rekisteröitymään Azure Multii-Factor-todennukseen.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="aa5b0-119">Lisä tietoja näistä käytännöistä on Ohje aiheessa [Mitä ovat perusaikataulun käytännöt](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="aa5b0-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="aa5b0-120">Määritä perusaikataulun käytännöt</span><span class="sxs-lookup"><span data-stu-id="aa5b0-120">Set up baseline policies</span></span>

1. <span data-ttu-id="aa5b0-121">Siirry [Azure-portaaliin](https://portal.azure.com)ja siirry sitten **Azure Active Directoryn** \> **ehdolliseen pääsyyn**.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="aa5b0-122">Perusaikataulun käytännöt on lueteltu sivulla.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="aa5b0-123">![Sivu, joka sisältää ehdollisen käytön peruskäytännöt.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="aa5b0-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="aa5b0-124">Katso seuraavat erityiset ohjeet kutakin käytäntöä varten:</span><span class="sxs-lookup"><span data-stu-id="aa5b0-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="aa5b0-125">Vaadi järjestelmänvalvojien MFA</span><span class="sxs-lookup"><span data-stu-id="aa5b0-125">Require MFA for admins</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="aa5b0-126">Vaadi MFA-käyttäjille</span><span class="sxs-lookup"><span data-stu-id="aa5b0-126">Require MFA for users</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="aa5b0-127">Estä aiempi todennus</span><span class="sxs-lookup"><span data-stu-id="aa5b0-127">Block legacy authentication</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="aa5b0-128">Vaadi MFA palvelun hallintaa varten</span><span class="sxs-lookup"><span data-stu-id="aa5b0-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="aa5b0-129">Voit määrittää useita lisä käytäntöjä, kuten hyväksyttyjen asiakas sovellusten vaatiminen.</span><span class="sxs-lookup"><span data-stu-id="aa5b0-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="aa5b0-130">Lisä tietoja on [ehdollisen käytön ohjeissa](https://docs.microsoft.com/azure/active-directory/conditional-access/) .</span><span class="sxs-lookup"><span data-stu-id="aa5b0-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>