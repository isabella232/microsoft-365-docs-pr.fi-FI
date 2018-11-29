---
title: Käyttää tiloissa Azure AD liitetty laite 365 Microsoft Business resurssit
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Opi hyödyntämään tiloissa resurssien käyttöä, kuten Windows 10-laite on liitetty liiketoiminnan rivin apps, jaettujen tiedostojen ja tulostimien Azure Active Directory-hakemistopalvelusta.
ms.openlocfilehash: 0a5d4b0828888fcb99676223000c446479f84ddc
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982253"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="5b17f-103">Käyttää tiloissa Azure AD liitetty laite 365 Microsoft Business resurssit</span><span class="sxs-lookup"><span data-stu-id="5b17f-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="5b17f-p101">Windows 10-laitteeseen, joka on liittynyt Azure Active Directory on käsitellä kaikkia pilvi-pohjainen Office 365-apps ja suojataan Microsoft 365 Business. Voit myös sallia pääsyn paikalliseen resursseja, kuten viiva, Business (LOB) apps, jaettujen tiedostojen ja tulostimien, synkronoi paikallisen Active Directory Azure Active Directoryn kanssa [Azure AD-yhteyden](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect)avulla. Katso lisätietoja [Azure Active Directoryn hallinta esittely](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) .</span><span class="sxs-lookup"><span data-stu-id="5b17f-p101">Any Windows 10 device that is Azure Active Directory joined will have access to all cloud-based resources such as your Office 365 apps and can be protected by Microsoft 365 Business. To also allow access to on-premises resources like Line Of Business (LOB) apps, file shares, and printers, you must synchronize your on-premises Active Directory with Azure Active Directory by using [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). See [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) to learn more.</span></span> 
  
## <a name="run-azure-ad-connect"></a><span data-ttu-id="5b17f-107">Suorita Azure AD muodostaa</span><span class="sxs-lookup"><span data-stu-id="5b17f-107">Run Azure AD Connect</span></span>

<span data-ttu-id="5b17f-108">Tee seuraavat toimet organisaation Azure AD liittynyt laitteissa tiloissa resurssien käytön.</span><span class="sxs-lookup"><span data-stu-id="5b17f-108">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="5b17f-109">Synkronoi käyttäjät, ryhmät ja yhteystiedot paikallisesta Active Directorysta Azure Active Directoryyn, ohjatun kansion synkronoinnin ja Azure AD Yhdistä [Office 365 directory-synkronoinnin määrittäminen](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)kuvataan.</span><span class="sxs-lookup"><span data-stu-id="5b17f-109">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="5b17f-p102">Kun directory-synkronointi on valmis, varmista, että organisaation Windows 10 laitteet liitetty Azure AD. Tämä vaihe tehdään erikseen kunkin Windows 10-laitteen. Lisätietoja [laitteiden Windows Microsoft 365 Business käyttäjien määrittäminen](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="5b17f-p102">After the directory synchronization has completed, make sure your organization's Windows 10 devices are Azure AD joined. This step is done individually on each Windows 10 device. See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="5b17f-p103">Kun Windows 10-laitteet on liitetty Azure AD, jokaisella käyttäjällä tulisi uudelleen niiden laitteiden ja kirjautumisen käyttäjätiedot Microsoft 365 Business kanssa. Kaikki laitteet on nyt omissa tiloissa sekä resurssien käytön.</span><span class="sxs-lookup"><span data-stu-id="5b17f-p103">Once the Windows 10 devices are Azure AD joined, each user should reboot their devices and login with their Microsoft 365 Business credentials. All devices will now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="5b17f-p104">Ei lisätoimia pääsyä tiloissa Azure AD resurssit on liitetty laitteita. Tämä on sisäinen toiminto käytettävissä Windows 10.</span><span class="sxs-lookup"><span data-stu-id="5b17f-p104">No additional steps are required to get access to on-premise resources for Azure AD joined devices. This is built-in functionality available in Windows 10.</span></span> 
  
<span data-ttu-id="5b17f-117">Jos organisaatiosi ei ole valmis ottamaan Azure AD liittynyt laitteen kokoonpanosta edellä kuvatun, kannattaa asentaa [hybridi Azure AD Joined laitteen kokoonpanotietoja](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="5b17f-117">If your organization is not ready to deploy in the Azure AD Joined Device Configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a><span data-ttu-id="5b17f-118">Huomioon otettavia laitteita Windows Azure AD liittäminen</span><span class="sxs-lookup"><span data-stu-id="5b17f-118">Considerations when joining your Windows devices to Azure AD</span></span>

<span data-ttu-id="5b17f-119">Azure AD liittäminen Windows-laite, joka on aiemmin ollut toimialueeseen liittymistä tai työryhmässä, sinun on otettava huomioon seuraavat rajoitukset:</span><span class="sxs-lookup"><span data-stu-id="5b17f-119">If you are Azure AD joining a Windows device that has previously been domain-joined or in a workgroup, you need to consider the following limitations:</span></span>
  
- <span data-ttu-id="5b17f-p105">Azure AD laite liitetään, se luo uuden käyttäjän ei viittaa olemassa olevaan profiiliin. Voit korjata tämän ongelman profiilit on siirrettävä manuaalisesti. Käyttäjäprofiili sisältää tietoja, kuten Suosikit, paikallisia tiedostoja, selaimesi asetuksia, Käynnistä-valikkoasetukset jne. Paras tapa on löytää kolmannen osapuolen työkalu yhdistää olemassa olevat tiedostot ja asetukset uuteen profiiliin</span><span class="sxs-lookup"><span data-stu-id="5b17f-p105">When a device Azure AD joins, it creates a new user without referencing an existing profile. To fix this, profiles need to be manually migrated. A user profile contains information like favorites, local files, browser settings, Start menu settings, etc. A best approach is to find a third-party tool to map existing files and settings to the new profile</span></span>
    
- <span data-ttu-id="5b17f-p106">Jos laite käyttää ryhmän Policy Objects (GPO), joitakin ryhmäkäytäntöobjekteja ei ole välttämättä verrattavissa [Kokoonpano tarjoaja](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) Intune. Löydä vastaavaa CSP aiemmin ryhmäkäytäntöobjekteja [MMAT työkalun](https://www.microsoft.com/download/details.aspx?id=45520) suorittaminen</span><span class="sxs-lookup"><span data-stu-id="5b17f-p106">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune. Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span> 
    
- <span data-ttu-id="5b17f-p107">Käyttäjät eivät voi todentaa Active Directory-todennus riippuvat sovellukset. Tämä vanha app käytön arvioiminen ja harkitse päivittämistä app, joka käyttää nykyaikaisia Auth Jos mahdollista.</span><span class="sxs-lookup"><span data-stu-id="5b17f-p107">Users will not be able to authenticate to applications that depend on Active Directory authentication. To deal with this evaluate using a legacy app and consider updating to an app that uses modern Auth if possible.</span></span>
    
- <span data-ttu-id="5b17f-p108">Active Directory-tulostimen etsimisen ei toimi. Voit korjata tämän ongelman suoraan tulostimen polut tarjoavat kaikille käyttäjille tai hyödyntää [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="5b17f-p108">Active Directory printer discovery will not work. To fix this, provide direct printer paths for all users or leverage [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
    

