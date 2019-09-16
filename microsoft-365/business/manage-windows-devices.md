---
title: Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
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
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Lue lisä tietoja siitä, miten Microsoft 365 voi suojata paikallisia mainoksia, jotka on liitetty Windows 10-laitteisiin.
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992225"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="b1177-103">Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi</span><span class="sxs-lookup"><span data-stu-id="b1177-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="b1177-104">Jos organisaatiosi käyttää paikallista Windows Server Active Directorya, voit määrittää Microsoft 365 Businessin suojaamaan Windows 10-laitteitasi samalla, kun ylläpidämme paikallisen todennuksen edellyttävien paikallisten resurssien käyttö oikeuksia.</span><span class="sxs-lookup"><span data-stu-id="b1177-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="b1177-105">Voit määrittää tämän ensin synkronoimalla Active Directory-hakemisto palvelun Azure Active Directoryn kanssa, jonka jälkeen rekisteröit Windows 10-laitteet Azure AD:N avulla ja rekisteröimällä ne mobiililaitteiden hallintaan Microsoft 365 Businessilla.</span><span class="sxs-lookup"><span data-stu-id="b1177-105">You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
<span data-ttu-id="b1177-106">Seuraavassa videossa kerrotaan, miten tämä määritetään tavallisimmille skenaariolle.</span><span class="sxs-lookup"><span data-stu-id="b1177-106">The following video details the steps for how to set this up for the most common scenario.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="b1177-107">Toimi alueeseen liitettyjen laitteiden määrittäminen Microsoft 365 Businessin hallitsemista varten</span><span class="sxs-lookup"><span data-stu-id="b1177-107">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="b1177-108">Jos haluat määrittää organisaatiosi toimi alueeseen liitetyt laitteet hyödyntämään Azure Active Directoryn tarjoamia ominaisuuksia paikallisen Active Directoryn lisäksi, voit ottaa käyttöön **hybridi Azure AD-liitetyt laitteet**.</span><span class="sxs-lookup"><span data-stu-id="b1177-108">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="b1177-109">Nämä ovat laitteita, jotka on liitetty paikalliseen Active Directoryyn ja Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="b1177-109">These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory.</span></span> <span data-ttu-id="b1177-110">Hybridi-Azure AD liitetyt laitteet voidaan suojata ja hallita Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="b1177-110">Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business.</span></span> 
  
<span data-ttu-id="b1177-111">Suorita seuraavat vaiheet, jotta Windows 10-laitteesi hybridi-Azure AD yhdistetään ja sitä hallinnoi Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="b1177-111">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="b1177-112">Synkronoi käyttäjät, ryhmät ja yhteys tiedot paikallisesta Active Directorysta Azure Active Directoryyn suorittamalla ohjattu hakemiston synkronointi ja Azure Active Directory Connect kuvatulla tavalla kohdassa [Office 365 Directory-synkronointi](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="b1177-112">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="b1177-113">Vaiheet ovat täsmälleen samat Microsoft 365-liike toiminnan osalta.</span><span class="sxs-lookup"><span data-stu-id="b1177-113">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="b1177-114">Ennen kuin suoritat vaiheen 3, jotta Windows 10-laitteet voivat olla hybridi-Azure AD liittynyt, sinun on varmistettava, että seuraavat edellytykset täyttyvät:</span><span class="sxs-lookup"><span data-stu-id="b1177-114">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="b1177-115">Käytössäsi on Azure AD Connectin uusin versio.</span><span class="sxs-lookup"><span data-stu-id="b1177-115">You are running the latest version of Azure AD connect.</span></span>

   - <span data-ttu-id="b1177-116">Azure AD Connect on synkronoinut kaikki niiden laitteiden tieto kone objektit, joihin haluat hybridi Azure AD-liittyneen.</span><span class="sxs-lookup"><span data-stu-id="b1177-116">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="b1177-117">Jos tieto kone objektit kuuluvat tiettyihin organisaatio yksiköihin (OU), varmista, että ne on määritetty synkronoitaviksi myös Azure AD Connectin avulla.</span><span class="sxs-lookup"><span data-stu-id="b1177-117">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="b1177-118">Rekisteröi olemassa olevat toimi alue-liitetyt Windows 10-laitteet hybridi-Azure AD-Liittymiksi ja rekisteröimällä ne mobiililaitteiden hallintaan Intune-laitteella (Microsoft 365 Business):</span><span class="sxs-lookup"><span data-stu-id="b1177-118">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="b1177-119">Noudata vaiheittaisia ohjeita [hybridi Azure Active Directoryn liitettyjen laitteiden määrittämisestä](https://go.microsoft.com/fwlink/p/?linkid=872870).</span><span class="sxs-lookup"><span data-stu-id="b1177-119">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870).</span></span> <span data-ttu-id="b1177-120">Tämä mahdollistaa paikallisen Active Directory-synkronoinnin liityttyä Windows 10-tieto koneisiin ja tekee niistä pilvi valmiina.</span><span class="sxs-lookup"><span data-stu-id="b1177-120">This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="b1177-121">Jos haluat rekisteröidä Windows 10-laitteen mobiililaitteiden hallintaa varten, Katso ohjeet [Windows 10-laitteen ilmoittamisen Intune-toiminnolla ryhmä käytännön avulla](https://go.microsoft.com/fwlink/p/?linkid=872871) .</span><span class="sxs-lookup"><span data-stu-id="b1177-121">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions.</span></span> <span data-ttu-id="b1177-122">Voit määrittää ryhmä käytännön paikallisen tieto koneen tasolla tai joukko toimintoja varten, voit luoda tämän ryhmä käytäntö asetuksen toimi alueen ohjaus kone palvelimessa.</span><span class="sxs-lookup"><span data-stu-id="b1177-122">You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span>