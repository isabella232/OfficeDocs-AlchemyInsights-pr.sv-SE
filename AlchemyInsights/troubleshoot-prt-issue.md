---
title: Felsöka problem med PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573902"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="df55f-102">Felsöka problem med PRT</span><span class="sxs-lookup"><span data-stu-id="df55f-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="df55f-103">För att alla enheter ska kunna bli autentiserade måste de vara fullständigt registrerade och i gott skick och kunna skaffa en primär uppdateringstoken (PRT).</span><span class="sxs-lookup"><span data-stu-id="df55f-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="df55f-104">För registrerings processen för Azure AD Join måste enheter finnas i ett företags nätverk.</span><span class="sxs-lookup"><span data-stu-id="df55f-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="df55f-105">Den fungerar också via VPN, men det finns vissa villkor för detta.</span><span class="sxs-lookup"><span data-stu-id="df55f-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="df55f-106">Vi har hört att kunder behöver hjälp med att felsöka registrerings processen för Azure AD Join under fjärran slut omständigheter.</span><span class="sxs-lookup"><span data-stu-id="df55f-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="df55f-107">Här är en uppdelning av vad som händer under registrerings processen.</span><span class="sxs-lookup"><span data-stu-id="df55f-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="df55f-108">**Molnbaserad miljö för moln (använder Azure AD-hash för lösen ord eller direktautentisering)**</span><span class="sxs-lookup"><span data-stu-id="df55f-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="df55f-109">Detta registrerings flöde kallas också "Sync Join".</span><span class="sxs-lookup"><span data-stu-id="df55f-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="df55f-110">Windows 10 upptäcker en SCP-post när användaren loggar in på enheten.</span><span class="sxs-lookup"><span data-stu-id="df55f-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="df55f-111">Enheten försöker först hämta klient information från klient-SCP i registret [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="df55f-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="df55f-112">Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="df55f-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="df55f-113">Om det Miss lyckas kommunicerar enheten med lokal Active Directory (AD) för att hämta klient information från tjänst anslutnings punkten (SCP).</span><span class="sxs-lookup"><span data-stu-id="df55f-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="df55f-114">För att verifiera SCP, hänvisa till det här [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="df55f-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="df55f-115">Vi rekommenderar att du aktiverar SCP i ANNONSen och bara använder klient platsens SCP för initial verifiering.</span><span class="sxs-lookup"><span data-stu-id="df55f-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="df55f-116">Windows 10 försöker kommunicera med Azure AD under system kontexten för att autentisera sig mot Azure AD.</span><span class="sxs-lookup"><span data-stu-id="df55f-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="df55f-117">Du kan kontrol lera om enheten kan komma åt Microsoft-resurser under system kontot med hjälp av test enhetens registrerings skript för registrering.</span><span class="sxs-lookup"><span data-stu-id="df55f-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="df55f-118">Windows 10 skapar ett självsignerat certifikat och lagrar det under datorobjektet i den lokala ANNONSen.</span><span class="sxs-lookup"><span data-stu-id="df55f-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="df55f-119">Detta kräver att en domänkontrollant används för att kontrol raden.</span><span class="sxs-lookup"><span data-stu-id="df55f-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="df55f-120">Ett enhets objekt som har ett certifikat synkroniseras till Azure AD via Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="df55f-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="df55f-121">Synkroniseringen är 30 minuter som standard, men det beror på konfigurationen av Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="df55f-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="df55f-122">Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="df55f-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="df55f-123">I det här steget ska du kunna se ämnes enheten i "förestående" tillstånd under enhets bladet i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="df55f-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="df55f-124">Vid nästa användar inloggning till Windows 10 kommer registreringen att genomföras.</span><span class="sxs-lookup"><span data-stu-id="df55f-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="df55f-125">Om du använder VPN och en utloggning-inloggning avslutar domän anslutningen kan du utlösa registrering manuellt:</span><span class="sxs-lookup"><span data-stu-id="df55f-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="df55f-126">Skicka en dsregcmd/Join lokalt i administratörs tolken eller fjärrans luta via PSExec till datorn.</span><span class="sxs-lookup"><span data-stu-id="df55f-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="df55f-127">Till exempel PsExec-s \\ win10client01 cmd, dsregcmd/Join</span><span class="sxs-lookup"><span data-stu-id="df55f-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="df55f-128">Mer information om hybrid kopplings problem finns i [Felsöka problem med enheter](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="df55f-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
