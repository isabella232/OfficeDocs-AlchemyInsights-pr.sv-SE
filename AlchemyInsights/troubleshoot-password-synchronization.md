---
title: Felsöka Lösenordssynkronisering
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664944"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="feddb-102">Felsöka Lösenordssynkronisering</span><span class="sxs-lookup"><span data-stu-id="feddb-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="feddb-103">För att felsöka problem med Lösenordssynkronisering kan du börja använda denna åtgärd för att ansluta till AAD för att avgöra varför lösen ord inte synkroniseras.</span><span class="sxs-lookup"><span data-stu-id="feddb-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="feddb-104">Börja genom att gå till [Hantera direkt synkronisering](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="feddb-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="feddb-105">Öppna en ny Windows PowerShell-session på din Azure AD Connect-Server och välj alternativet **Kör som administratör** .</span><span class="sxs-lookup"><span data-stu-id="feddb-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="feddb-106">Kör Set-ExecutionPolicy RemoteSigned eller Set-ExecutionPolicy unrestricted.</span><span class="sxs-lookup"><span data-stu-id="feddb-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="feddb-107">Starta Azure AD Connect-guiden.</span><span class="sxs-lookup"><span data-stu-id="feddb-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="feddb-108">Gå till sidan Ytterligare aktiviteter > **Felsöka**  >  **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="feddb-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="feddb-109">Välj **Starta** för att öppna fel söknings menyn i PowerShell.</span><span class="sxs-lookup"><span data-stu-id="feddb-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="feddb-110">Välj **Felsök Lösenordssynkronisering**.</span><span class="sxs-lookup"><span data-stu-id="feddb-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="feddb-111">Problemet är vanligt vis att ett lösen ord inte är synkroniserat för ett visst användar konto.</span><span class="sxs-lookup"><span data-stu-id="feddb-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="feddb-112">**Anteckningar** Det går inte att synkronisera lösen ord om den senaste lyckade lösen ords synkroniseringen var för lite sedan.</span><span class="sxs-lookup"><span data-stu-id="feddb-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="feddb-113">Mer hjälp med att felsöka Lösenordssynkronisering finns i [Felsöka lösen ord för Lösenordssynkronisering med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="feddb-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>