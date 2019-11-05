---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964337"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="f5ef6-102">Åtgärda leveransproblem för felkod 550 5.4.1 Relä åtkomst nekad</span><span class="sxs-lookup"><span data-stu-id="f5ef6-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="f5ef6-103">Det här problemet uppstår när [du kontrollerar om en e-postadress är giltig för att förhindra studsar](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) när du anger Office 365-nätverket.</span><span class="sxs-lookup"><span data-stu-id="f5ef6-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="f5ef6-104">Prova följande:</span><span class="sxs-lookup"><span data-stu-id="f5ef6-104">Try the following:</span></span>

1. <span data-ttu-id="f5ef6-105">Ta reda på om problemet är specifikt för en hel domän eller en enskild e-postadress:</span><span class="sxs-lookup"><span data-stu-id="f5ef6-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="f5ef6-106">Hela domänen: ibland måste domänen synkroniseras; försök att [ange domänen till intern och sedan tillbaka till auktoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="f5ef6-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
     - <span data-ttu-id="f5ef6-107">En e-postadress: ibland måste adressen synkroniseras; ändra SMTP-proxyadressen och sedan ändra tillbaka den kan hjälpa.</span><span class="sxs-lookup"><span data-stu-id="f5ef6-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="f5ef6-108">Ta reda på om problemet är specifikt för en grupp eller en offentlig mapp.</span><span class="sxs-lookup"><span data-stu-id="f5ef6-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="f5ef6-109">För vissa objekttyper kan objekten behöva skapas manuellt i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f5ef6-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="f5ef6-110">Om du behöver ytterligare hjälp, öppna ett supportärende och ange omfattningen av problemet (includidng typ av objekt som du skickar till) så att vi kan hjälpa dig bättre.</span><span class="sxs-lookup"><span data-stu-id="f5ef6-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>