---
title: Behöver du hjälp med begränsningarna för att skicka e-post?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836297"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="6e158-102">Behöver du hjälp med begränsningarna för att skicka e-post?</span><span class="sxs-lookup"><span data-stu-id="6e158-102">Need help with email sending limits?</span></span>

<span data-ttu-id="6e158-103">Nedan visas de **avsiktliga sändningsbegränsningarna** som tillämpas i tjänsten.</span><span class="sxs-lookup"><span data-stu-id="6e158-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="6e158-104">Mer information om de här begränsningarna finns [här](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="6e158-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="6e158-105">För att hindra att oönskade massmeddelanden levereras tillämpar vi **begränsningar för alla utgående och interna meddelanden** per användare.</span><span class="sxs-lookup"><span data-stu-id="6e158-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="6e158-106">Den här gränsen ligger på **10 000 mottagare per dag** för alla SKU:er.</span><span class="sxs-lookup"><span data-stu-id="6e158-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="6e158-107">Kunder som behöver skicka legitima, kommersiella massutskick (till exempel kundbrev) bör använda tredjepartsleverantörer som specialiserar sig i dessa tjänster.</span><span class="sxs-lookup"><span data-stu-id="6e158-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="6e158-108">**Obs**: När gränsen har nåtts går det inte att skicka meddelanden från postlådan förrän antalet mottagare som under det senaste dygnet har mottagit meddelanden blir färre än gränsvärdet.</span><span class="sxs-lookup"><span data-stu-id="6e158-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="6e158-109">Användaren kan inte skicka meddelanden förrän det har skett.</span><span class="sxs-lookup"><span data-stu-id="6e158-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="6e158-110">Gränsen för meddelandehastigheten på **30 meddelanden per minut** gäller för alla SKU:er.</span><span class="sxs-lookup"><span data-stu-id="6e158-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="6e158-111">Det här anger hur många meddelanden en användare kan skicka från sitt Exchange Online-konto inom en viss tidsperiod.</span><span class="sxs-lookup"><span data-stu-id="6e158-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="6e158-112">Det **högsta antalet mottagare som tillåts i fälten Till, Kopia och Hemlig kopia** för ett enskilt e-postmeddelande är **1 000** för alla SKU:er.</span><span class="sxs-lookup"><span data-stu-id="6e158-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="6e158-113">Om du vill anpassa den här gränsen kan du göra det [här](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="6e158-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
