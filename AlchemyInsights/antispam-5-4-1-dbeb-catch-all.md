---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821465"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="ebe8b-102">Korrigera leveransproblem för felkod 550 5.4.1 Nekad reläåtkomst</span><span class="sxs-lookup"><span data-stu-id="ebe8b-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="ebe8b-103">Det här problemet inträffar när [du kontrollerar om en e-postadress är giltig för att förhindra återstuds när](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) du går till Microsoft-nätverket.</span><span class="sxs-lookup"><span data-stu-id="ebe8b-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="ebe8b-104">Prova följande:</span><span class="sxs-lookup"><span data-stu-id="ebe8b-104">Try the following:</span></span>

1. <span data-ttu-id="ebe8b-105">Avgör om problemet är specifikt för en hel domän eller en enda e-postadress:</span><span class="sxs-lookup"><span data-stu-id="ebe8b-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="ebe8b-106">Hela domänen: Ibland behöver domänen synkroniseras. Prova [att ange domänen som Intern och sedan tillbaka till Auktoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="ebe8b-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="ebe8b-107">Enskild e-postadress: Ibland behöver adressen synkroniseras. Det kan vara bra att ändra smtp-proxyadressen och sedan ändra tillbaka den.</span><span class="sxs-lookup"><span data-stu-id="ebe8b-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="ebe8b-108">Avgör om problemet är specifikt för en grupp eller offentlig mapp.</span><span class="sxs-lookup"><span data-stu-id="ebe8b-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="ebe8b-109">För vissa objekttyper kan objekten behöva skapas manuellt i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ebe8b-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="ebe8b-110">Om du behöver mer hjälp kan du öppna ett support ärende och ange omfattningen av problemet (inklusive typen av objekt som du skickar till) så att vi kan hjälpa dig bättre.</span><span class="sxs-lookup"><span data-stu-id="ebe8b-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>