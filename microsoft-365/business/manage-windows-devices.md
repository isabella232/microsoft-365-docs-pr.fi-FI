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
description: Microsoft suojaa 365 käyttöönotto paikallisen AD liittynyt Windows 10-laitteita.
ms.openlocfilehash: af0e78ef6e79bfd612b11a16538e7afcd377ffb0
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/15/2019
ms.locfileid: "34071546"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="3c0d3-103">Ota toimialueeseen liitetyt Windows 10 -laitteet Microsoft 365 Businessin hallittavaksi</span><span class="sxs-lookup"><span data-stu-id="3c0d3-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="3c0d3-104">Jos organisaatiossa käytetään Windows Server Active Directory tiloissa, voit määrittää Microsoft 365 liiketoiminnan suojaamaan Windows 10-laitteet, säilyttäen kuitenkin edellyttää paikallista todennusta tiloissa resurssien käytön.</span><span class="sxs-lookup"><span data-stu-id="3c0d3-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="3c0d3-105">Voit tehdä tämän ensimmäisen synkronoida Active Directoryn Azure Active Directoryn, rekisteröitymisestä Azure AD Windows 10-laitteiden ja ei tarvitse ottaa niitä mukaan 365 Microsoft Business management kannettavan laitteen kanssa.</span><span class="sxs-lookup"><span data-stu-id="3c0d3-105">You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="3c0d3-106">Määritä laitteet toimialueeseen liittymistä hallinnoi 365 Microsoft Business</span><span class="sxs-lookup"><span data-stu-id="3c0d3-106">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="3c0d3-107">Määrittämään organisaation toimialueeseen liittymistä laitteet hyötyvät Azure Active Directoryssa paikallisen Active Directoryn lisäksi annettuja ominaisuuksia voit toteuttaa **hybridi Azure AD liitetyt laitteet**.</span><span class="sxs-lookup"><span data-stu-id="3c0d3-107">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="3c0d3-108">Nämä ovat laitteita, jotka on liitetty toisiinsa sekä paikalliseen Active Directory-ja Azure-Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3c0d3-108">These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory.</span></span> <span data-ttu-id="3c0d3-109">Hybrid liittynyt Azure AD laitteet on suojattu ja hallinnoi 365 Microsoft Business.</span><span class="sxs-lookup"><span data-stu-id="3c0d3-109">Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business.</span></span> 
  
<span data-ttu-id="3c0d3-110">Noudattamalla alla tehdä laitteiden Windows 10 Azure AD liittynyt ja hallitsema Microsoft 365 Business hybridi.</span><span class="sxs-lookup"><span data-stu-id="3c0d3-110">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="3c0d3-111">Synkronoi käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directoryyn, suorita ohjattu synkronoinnin Directory ja Azure Active Directory muodostaa yhteyden [Office 365: ssä directory-synkronoinnin määrittäminen](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)kuvatulla.</span><span class="sxs-lookup"><span data-stu-id="3c0d3-111">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="3c0d3-112">Vaiheet ovat täsmälleen samat 365 Microsoft Business.</span><span class="sxs-lookup"><span data-stu-id="3c0d3-112">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="3c0d3-113">Ennen kuin suoritat vaiheen 3 Windows 10 Azure AD liittynyt Hybrid on laitteissa, sinun on Varmista, että tietokoneen on täytettävä seuraavat edellytykset:</span><span class="sxs-lookup"><span data-stu-id="3c0d3-113">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="3c0d3-114">Käytössäsi on uusin versio Azure AD muodosta.</span><span class="sxs-lookup"><span data-stu-id="3c0d3-114">You are running the latest version of Azure AD connect.</span></span>

   - <span data-ttu-id="3c0d3-115">Azure AD yhdistää kaikki tietokoneen haluat hybridi Azure AD liittynyt laitteiden objektit on synkronoitu.</span><span class="sxs-lookup"><span data-stu-id="3c0d3-115">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="3c0d3-116">Jos tietokoneen objektit kuuluvat tietyn organisaation yksiköt (OU), varmista, että nämä organisaatioyksiköiden määritetään synkronoitaviksi Azure AD muodostaa myös.</span><span class="sxs-lookup"><span data-stu-id="3c0d3-116">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="3c0d3-117">Aiemmin toimialueeseen liittymistä Windows 10 laitteet hybridi Azure AD Joined ja rekisteröityvän Intune (Microsoft Business-365) hallinnoinnin kannettavan laitteen rekisteröiminen:</span><span class="sxs-lookup"><span data-stu-id="3c0d3-117">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="3c0d3-118">Vaihe vaiheelta ohjeiden mukaisesti- [hybridi Azure liitetty Active Directory-laitteiden määrittämisestä](https://go.microsoft.com/fwlink/p/?linkid=872870).</span><span class="sxs-lookup"><span data-stu-id="3c0d3-118">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870).</span></span> <span data-ttu-id="3c0d3-119">Tämä mahdollistaa paikallisen Active Directory synkronointi liittynyt Windows 10-tietokoneisiin ja ne cloud valmis.</span><span class="sxs-lookup"><span data-stu-id="3c0d3-119">This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="3c0d3-120">Jotta voit rekisteröidä Windows 10-laitteen kannettavan laitteen hallintaan, katso ohjeet [Windows 10 Intune ryhmäkäytännön avulla laitteen rekisteröiminen](https://go.microsoft.com/fwlink/p/?linkid=872871) .</span><span class="sxs-lookup"><span data-stu-id="3c0d3-120">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions.</span></span> <span data-ttu-id="3c0d3-121">Voit määrittää ryhmäkäytännön paikallisen tietokoneen ääressä tasolla tai voit luoda joukkotoiminnot-palvelimen toimialueen ohjauskoneen tämän ryhmäkäytännön asetus.</span><span class="sxs-lookup"><span data-stu-id="3c0d3-121">You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span>