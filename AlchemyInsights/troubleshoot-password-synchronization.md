---
title: Felsöka lösenordssynkronisering
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732528"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="6a2e8-102">Felsöka lösenordssynkronisering</span><span class="sxs-lookup"><span data-stu-id="6a2e8-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="6a2e8-103">Så här felsöker du problem där inga lösenord synkroniseras med Azure AD Connect version 1.1.614.0 eller senare:</span><span class="sxs-lookup"><span data-stu-id="6a2e8-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="6a2e8-104">Öppna en ny Windows PowerShell-session på Din Azure AD Connect-server med alternativet **Kör som administratör.**</span><span class="sxs-lookup"><span data-stu-id="6a2e8-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="6a2e8-105">Kör **Obegränsad set-executionPolicy-fjärrsignerad** eller **Ange körningspolicy.**</span><span class="sxs-lookup"><span data-stu-id="6a2e8-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="6a2e8-106">Starta Azure AD Connect-guiden.</span><span class="sxs-lookup"><span data-stu-id="6a2e8-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="6a2e8-107">Navigera till sidan **Ytterligare uppgifter,** välj **Felsöka**och klicka på **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="6a2e8-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="6a2e8-108">På sidan Felsökning klickar du på **Starta för att starta felsökningsmenyn** i PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6a2e8-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="6a2e8-109">Välj **Felsök lösenordssynkronisering**på huvudmenyn .</span><span class="sxs-lookup"><span data-stu-id="6a2e8-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="6a2e8-110">På undermenyn väljer du **Lösenordssynkronisering fungerar inte alls**.</span><span class="sxs-lookup"><span data-stu-id="6a2e8-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="6a2e8-111">**Förstå resultatet av felsökningsuppgiften**</span><span class="sxs-lookup"><span data-stu-id="6a2e8-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="6a2e8-112">Felsökningsuppgiften utför följande kontroller:</span><span class="sxs-lookup"><span data-stu-id="6a2e8-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="6a2e8-113">Verifierar att lösenordssynkroniseringsfunktionen är aktiverad för din Azure AD-klientorganisation.</span><span class="sxs-lookup"><span data-stu-id="6a2e8-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="6a2e8-114">Verifierar att Azure AD Connect-servern inte är i mellanlagringsläge.</span><span class="sxs-lookup"><span data-stu-id="6a2e8-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="6a2e8-115">För varje befintlig lokal Active Directory-anslutning (som motsvarar en befintlig Active Directory-skog):</span><span class="sxs-lookup"><span data-stu-id="6a2e8-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="6a2e8-116">Verifierar att lösenordssynkroniseringsfunktionen är aktiverad.</span><span class="sxs-lookup"><span data-stu-id="6a2e8-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="6a2e8-117">Söker efter pulsslagshändelser för lösenordssynkronisering i windows-programhändelseloggarna.</span><span class="sxs-lookup"><span data-stu-id="6a2e8-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="6a2e8-118">För varje Active Directory-domän under den lokala Active Directory-anslutningen:</span><span class="sxs-lookup"><span data-stu-id="6a2e8-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="6a2e8-119">Verifierar att domänen kan nås från Azure AD Connect-servern.</span><span class="sxs-lookup"><span data-stu-id="6a2e8-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="6a2e8-120">Verifierar att AD DS-konton (Active Directory Domain Services) som används av den lokala Active Directory-anslutningen har rätt användarnamn, lösenord och behörigheter som krävs för lösenordssynkronisering.</span><span class="sxs-lookup"><span data-stu-id="6a2e8-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="6a2e8-121">Mer hjälp med felsökning av lösenordssynkronisering finns i [Felsöka lösenordssynkronisering med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="6a2e8-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  