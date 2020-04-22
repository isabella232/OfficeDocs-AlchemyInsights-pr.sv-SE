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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707929"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="a2e20-102">Åtgärda leveransproblem för felkod 550 5.4.1 Relay Access Nekad</span><span class="sxs-lookup"><span data-stu-id="a2e20-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="a2e20-103">Det hÃ¤r problemet uppstÃ¥r vid [kontroll av om en e-postadress är giltig för att förhindra bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) nÃ¤r du går in i Microsoft-nätverket.</span><span class="sxs-lookup"><span data-stu-id="a2e20-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="a2e20-104">Prova följande:</span><span class="sxs-lookup"><span data-stu-id="a2e20-104">Try the following:</span></span>

1. <span data-ttu-id="a2e20-105">Ta reda på om problemet är specifikt för en hel domän eller en enda e-postadress:</span><span class="sxs-lookup"><span data-stu-id="a2e20-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="a2e20-106">Hela domänen: Ibland måste domänen synkroniseras. prova [att ställa in domänen på Internt och sedan tillbaka till Auktoritär .](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="a2e20-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="a2e20-107">Enkel e-postadress: Ibland måste adressen synkroniseras. ändra smtp proxyadress och sedan ändra tillbaka det kan hjälpa.</span><span class="sxs-lookup"><span data-stu-id="a2e20-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="a2e20-108">Ta reda på om problemet är specifikt för en grupp eller gemensam mapp.</span><span class="sxs-lookup"><span data-stu-id="a2e20-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="a2e20-109">För vissa objekttyper kan objekten behöva skapas manuellt i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a2e20-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="a2e20-110">Om du behöver ytterligare hjälp kan du öppna en supportbiljett och ange problemets omfattning (inklusive vilken typ av objekt du skickar till) så att vi kan hjälpa dig bättre.</span><span class="sxs-lookup"><span data-stu-id="a2e20-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>