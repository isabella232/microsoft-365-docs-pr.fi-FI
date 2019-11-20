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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
description: Lue lisä tietoja ehdollisten käyttö käytäntöjen määrittämisestä Microsoft 365-kampanjoille.
ms.openlocfilehash: aebdb733c2dd9a05947335ad4f151104d801568e
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718825"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="b989f-103">Määritä ehdolliset käyttö oikeus käytännöt</span><span class="sxs-lookup"><span data-stu-id="b989f-103">Set up conditional access policies</span></span>

<span data-ttu-id="b989f-104">[Ehdollisen käytön](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) käytännöt lisäävät huomattavasti lisä suojausta.</span><span class="sxs-lookup"><span data-stu-id="b989f-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="b989f-105">Microsoft tarjoaa perusaikataulun ehdollisten käyttö oikeus käytäntöjen joukon, jota suositellaan kaikille asiakkaille.</span><span class="sxs-lookup"><span data-stu-id="b989f-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="b989f-106">Perusaikataulun käytännöt ovat joukko esimääritettyjä käytäntöjä, jotka auttavat suojaamaan organisaatioita monista yleisistä hyökkäyksistä.</span><span class="sxs-lookup"><span data-stu-id="b989f-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="b989f-107">Näitä yleisiä hyökkäyksiä voivat olla Sala sanan suihkutus, uusinta toisto ja tietojenkalastelu.</span><span class="sxs-lookup"><span data-stu-id="b989f-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="b989f-108">Nämä käytännöt edellyttävät, että järjestelmänvalvojat ja käyttäjät syöttäisivät toisen todennus muodon (jota kutsutaan nimellä Monivaiheinen todennus tai MFA), kun tietyt ehdot täyttyvät.</span><span class="sxs-lookup"><span data-stu-id="b989f-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="b989f-109">Jos käyttäjä on esimerkiksi kirjauduttava sisään toisesta maasta, kirjautumista voidaan pitää riskialttiina ja käyttäjän on annettava lisä todennus muoto.</span><span class="sxs-lookup"><span data-stu-id="b989f-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="b989f-110">Tällä hetkellä perusaikataulun käytäntöjä ovat seuraavat:</span><span class="sxs-lookup"><span data-stu-id="b989f-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="b989f-111">**Edellytä, että järjestelmänvalvojien** &ndash; MFA edellyttää usean tekijän todennusta etuoikeutetuimpia järjestelmänvalvojan rooleja varten, mukaan lukien yleinen järjestelmänvalvoja.</span><span class="sxs-lookup"><span data-stu-id="b989f-111">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="b989f-112">**Loppu käyttäjän suojaus** &ndash; vaatii usean tekijän todennuksen käyttäjille vain silloin, kun kirjautuminen on riskialtista.</span><span class="sxs-lookup"><span data-stu-id="b989f-112">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="b989f-113">**Estä vanha todennus** &ndash; vanhemmat asiakas sovellukset ja jotkin uudet sovellukset eivät käytä uudempia, turvallisempia todennus protokollia.</span><span class="sxs-lookup"><span data-stu-id="b989f-113">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="b989f-114">Nämä vanhemmat sovellukset voivat ohittaa ehdolliset käyttö käytännöt ja käyttää ympäristöäsi luvattomasti.</span><span class="sxs-lookup"><span data-stu-id="b989f-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="b989f-115">Tämä käytäntö estää pääsyn asiakkailta, jotka eivät tue ehdollista pääsyä.</span><span class="sxs-lookup"><span data-stu-id="b989f-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="b989f-116">**Vaadi MFA for Service Management** &ndash; edellyttää monivaiheista todennusta, jotta voit käyttää hallinta työkaluja, mukaan lukien Azure Portal (jossa määrität peruskäytännöt).</span><span class="sxs-lookup"><span data-stu-id="b989f-116">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="b989f-117">Microsoft suosittelee, että otat kaikki nämä perusaikataulun käytännöt käyttöön.</span><span class="sxs-lookup"><span data-stu-id="b989f-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="b989f-118">Kun nämä käytännöt on otettu käyttöön, ylläpitäjiä ja käyttäjiä kehotetaan rekisteröitymään Azure Multii-Factor-todennukseen.</span><span class="sxs-lookup"><span data-stu-id="b989f-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="b989f-119">Lisä tietoja näistä käytännöistä on Ohje aiheessa [Mitä ovat perusaikataulun käytännöt](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="b989f-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="b989f-120">Määritä perusaikataulun käytännöt</span><span class="sxs-lookup"><span data-stu-id="b989f-120">Set up baseline policies</span></span>

1. <span data-ttu-id="b989f-121">Siirry [Azure-portaaliin](https://portal.azure.com)ja siirry sitten **Azure Active Directoryn** \> **ehdolliseen pääsyyn**.</span><span class="sxs-lookup"><span data-stu-id="b989f-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="b989f-122">Perusaikataulun käytännöt on lueteltu sivulla.</span><span class="sxs-lookup"><span data-stu-id="b989f-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="b989f-123">![Sivu, joka sisältää ehdollisen käytön peruskäytännöt.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="b989f-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="b989f-124">Katso seuraavat erityiset ohjeet kutakin käytäntöä varten:</span><span class="sxs-lookup"><span data-stu-id="b989f-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="b989f-125">Vaadi järjestelmänvalvojien MFA</span><span class="sxs-lookup"><span data-stu-id="b989f-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="b989f-126">Vaadi MFA-käyttäjille</span><span class="sxs-lookup"><span data-stu-id="b989f-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="b989f-127">Estä aiempi todennus</span><span class="sxs-lookup"><span data-stu-id="b989f-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="b989f-128">Vaadi MFA palvelun hallintaa varten</span><span class="sxs-lookup"><span data-stu-id="b989f-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="b989f-129">Voit määrittää useita lisä käytäntöjä, kuten hyväksyttyjen asiakas sovellusten vaatiminen.</span><span class="sxs-lookup"><span data-stu-id="b989f-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="b989f-130">Lisä tietoja on [ehdollisen käyttö oikeus dokumentaatiossa](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="b989f-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
