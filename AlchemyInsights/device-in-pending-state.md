---
title: Enhet i vänte läge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679993"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="b7e46-102">Enhet i vänte läge</span><span class="sxs-lookup"><span data-stu-id="b7e46-102">Device in pending state</span></span>

<span data-ttu-id="b7e46-103">**Förutsättningar**</span><span class="sxs-lookup"><span data-stu-id="b7e46-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="b7e46-104">Om du ställer in enhets registreringarna första gången bör du kontrol lera att du har granskat [introduktionen till enhets hantering i Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) som hjälper dig att hämta enheter under kontrollen av Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b7e46-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="b7e46-105">Om du registrerar enheter till Azure AD direkt och registrerar dem i Intune måste du se till att du har [konfigurerat Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) och har [licensierat](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) först.</span><span class="sxs-lookup"><span data-stu-id="b7e46-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="b7e46-106">Se till att du har behörighet att utföra åtgärder i Azure AD och lokala annonser.</span><span class="sxs-lookup"><span data-stu-id="b7e46-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="b7e46-107">Endast globala administratörer i Azure AD kan hantera inställningar för enhets registreringar.</span><span class="sxs-lookup"><span data-stu-id="b7e46-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="b7e46-108">Om du konfigurerar automatiska registreringar i lokala Active Directory måste du dessutom vara administratör för Active Directory och AD FS (om tillämpligt).</span><span class="sxs-lookup"><span data-stu-id="b7e46-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="b7e46-109">För registrerings processen för Azure AD Join krävs enheter för företags nätverk.</span><span class="sxs-lookup"><span data-stu-id="b7e46-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="b7e46-110">Den fungerar också via VPN, men det finns vissa villkor för detta.</span><span class="sxs-lookup"><span data-stu-id="b7e46-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="b7e46-111">Vi har hört att kunder behöver hjälp med att felsöka registrerings processen för Azure AD Join under andra arbets förhållanden.</span><span class="sxs-lookup"><span data-stu-id="b7e46-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="b7e46-112">**Molnbaserad miljö för moln (använder Azure AD-hash för lösen ord eller direktautentisering)**</span><span class="sxs-lookup"><span data-stu-id="b7e46-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="b7e46-113">Detta registrerings flöde kallas också "Sync Join".</span><span class="sxs-lookup"><span data-stu-id="b7e46-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="b7e46-114">Här är en uppdelning av vad som händer under registrerings processen:</span><span class="sxs-lookup"><span data-stu-id="b7e46-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="b7e46-115">Windows 10 upptäcker tjänst anslutnings punktens post (SCP) när användaren loggar in på enheten.</span><span class="sxs-lookup"><span data-stu-id="b7e46-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="b7e46-116">Enheten försöker först hämta klient information från klient-SCP i registret [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="b7e46-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="b7e46-117">Mer information finns i [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="b7e46-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="b7e46-118">Om det Miss lyckas kommunicerar enheten med lokal Active Directory för att få information om klient organisationen från SCP.</span><span class="sxs-lookup"><span data-stu-id="b7e46-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="b7e46-119">Om du vill verifiera SCP läser du det här [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="b7e46-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="b7e46-120">Vi rekommenderar att du aktiverar SCP i Active Directory och bara använder klientens SCP för initial verifiering.</span><span class="sxs-lookup"><span data-stu-id="b7e46-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="b7e46-121">Windows 10 försöker kommunicera med Azure AD under system kontexten för att autentisera sig mot Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b7e46-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="b7e46-122">Du kan kontrol lera om enheten kan komma åt Microsoft-resurser under system kontot med hjälp av [test enhetens registrerings skript för registrering](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="b7e46-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="b7e46-123">Windows 10 skapar ett egensignerat certifikat och lagrar det under datorobjektet i lokala Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b7e46-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="b7e46-124">Detta kräver att en domänkontrollant används för att kontrol raden.</span><span class="sxs-lookup"><span data-stu-id="b7e46-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="b7e46-125">Enhets objekt med certifikat synkroniseras till Azure AD via Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b7e46-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="b7e46-126">Synkroniseringen är 30 minuter som standard, men det beror på konfigurationen av Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b7e46-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="b7e46-127">Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="b7e46-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="b7e46-128">I det här steget ska du kunna se ämnes enheten i "**förestående**" tillstånd under enhets bladet i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="b7e46-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="b7e46-129">Vid nästa användar inloggning till Windows 10 kommer registreringen att genomföras.</span><span class="sxs-lookup"><span data-stu-id="b7e46-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="b7e46-130">Om du använder VPN och utloggning/inloggning säger upp domän anslutningen kan du utlösa registreringen manuellt.</span><span class="sxs-lookup"><span data-stu-id="b7e46-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="b7e46-131">Så här gör du:</span><span class="sxs-lookup"><span data-stu-id="b7e46-131">To do that:</span></span>
    >
    > <span data-ttu-id="b7e46-132">Skicka ett `dsregcmd /join` lokalt i administratörs meddelande eller fjärrans luta via PsExec till datorn.</span><span class="sxs-lookup"><span data-stu-id="b7e46-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="b7e46-133">Till exempel: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="b7e46-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="b7e46-134">Vanliga frågor och [svar](https://docs.microsoft.com/azure/active-directory/devices/faq)om Azure Active Directory-registrering.</span><span class="sxs-lookup"><span data-stu-id="b7e46-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
