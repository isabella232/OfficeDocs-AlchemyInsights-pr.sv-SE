---
title: Felsöka lösenordssynkronisering
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387895"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="1427c-102">Felsöka lösenordssynkronisering</span><span class="sxs-lookup"><span data-stu-id="1427c-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="1427c-103">Om du vill felsöka problem med lösenordssynkronisering börjar du med den här felsökningsuppgiften för AAD Connect för att ta reda på varför lösenord inte synkroniseras.</span><span class="sxs-lookup"><span data-stu-id="1427c-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="1427c-104">Börja med att gå till [Hantera direktsynkronisering](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="1427c-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="1427c-105">Öppna en ny Windows PowerShell-session på din Azure AD Connect-server och välj alternativet **Kör som administratör.**</span><span class="sxs-lookup"><span data-stu-id="1427c-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="1427c-106">Kör Set-ExecutionPolicy RemoteSigned eller Set-ExecutionPolicy Obegränsad.</span><span class="sxs-lookup"><span data-stu-id="1427c-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="1427c-107">Starta Azure AD Connect-guiden.</span><span class="sxs-lookup"><span data-stu-id="1427c-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="1427c-108">Gå till sidan Ytterligare uppgifter > **felsöka**  >  **nästa**.</span><span class="sxs-lookup"><span data-stu-id="1427c-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="1427c-109">Välj **Starta** för att öppna felsökningsmenyn för PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1427c-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="1427c-110">Välj **Felsöka lösenordssynkronisering**.</span><span class="sxs-lookup"><span data-stu-id="1427c-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="1427c-111">Problemet är vanligtvis att ett lösenord inte synkroniseras för ett visst användarkonto.</span><span class="sxs-lookup"><span data-stu-id="1427c-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="1427c-112">**Anteckningar** Lösenordssynkronisering misslyckas om den senaste lyckades lösenordssynkroniseringen var för en tid sedan.</span><span class="sxs-lookup"><span data-stu-id="1427c-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="1427c-113">Mer hjälp med felsökning av lösenordssynkronisering finns i [Felsöka synkronisering av lösenordshÃ¶kning med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="1427c-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>