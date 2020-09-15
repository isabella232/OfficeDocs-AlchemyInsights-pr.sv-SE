---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717379"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="83e89-102">Åtgärda leverans problem för felkod 550 5.4.1 Relä åtkomst nekad</span><span class="sxs-lookup"><span data-stu-id="83e89-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="83e89-103">Det här problemet uppstår när [du kontrollerar om en e-postadress är giltig för att förhindra bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) när du anger Microsoft Network.</span><span class="sxs-lookup"><span data-stu-id="83e89-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="83e89-104">Prova följande:</span><span class="sxs-lookup"><span data-stu-id="83e89-104">Try the following:</span></span>

1. <span data-ttu-id="83e89-105">Avgöra om problemet är specifikt för en hel domän eller en enskild e-post adress:</span><span class="sxs-lookup"><span data-stu-id="83e89-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="83e89-106">Hela domänen: domänen måste synkroniseras. pröva att [ange domänen som intern och sedan tillbaka till auktoritär](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="83e89-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="83e89-107">En e-postadress: ibland måste adressen synkroniseras; att ändra SMTP-proxyadress och sedan ändra tillbaka den kan hjälpa dig.</span><span class="sxs-lookup"><span data-stu-id="83e89-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="83e89-108">Avgöra om problemet är specifikt för en grupp eller en gemensam mapp.</span><span class="sxs-lookup"><span data-stu-id="83e89-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="83e89-109">För vissa objekt typer kan objekten behöva skapas manuellt i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="83e89-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="83e89-110">Om du behöver mer hjälp kan du öppna ett support ärende och ange omfattningen för problemet (inklusive den typ av objekt som du skickar till) så att du lättare får till gång till det.</span><span class="sxs-lookup"><span data-stu-id="83e89-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>