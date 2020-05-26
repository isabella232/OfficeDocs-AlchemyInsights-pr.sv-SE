---
title: Behöver du hjälp med e-post skicka gränser?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358359"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="09e14-102">Behöver du hjälp med e-post skicka gränser?</span><span class="sxs-lookup"><span data-stu-id="09e14-102">Need help with email sending limits?</span></span>

<span data-ttu-id="09e14-103">Nedan visas de **genomdesignasändande gränser** som tillämpas i tjänsten.</span><span class="sxs-lookup"><span data-stu-id="09e14-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="09e14-104">Mer information om dessa gränser finns [här](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="09e14-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="09e14-105">För att avskräcka från leverans av oönskade massmeddelanden tillämpar vi mottagare per användare **för alla utgående och interna meddelanden.**</span><span class="sxs-lookup"><span data-stu-id="09e14-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="09e14-106">Den här gränsen är **10 000 mottagare per dag.**</span><span class="sxs-lookup"><span data-stu-id="09e14-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="09e14-107">Kunder som behöver skicka legitim kommersiell masssupport (till exempel kundnyhetsbrev) bör använda tredjepartsleverantörer som är specialiserade på dessa tjänster.</span><span class="sxs-lookup"><span data-stu-id="09e14-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="09e14-108">**När**gränsen för mottagarfrekvensen har uppnåtts kan meddelanden inte skickas från postlådan förrän antalet mottagare som har skickats meddelanden under de senaste 24 timmarna sjunker under gränsen.</span><span class="sxs-lookup"><span data-stu-id="09e14-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="09e14-109">Användaren kommer inte att kunna skicka meddelanden förrän den punkten.</span><span class="sxs-lookup"><span data-stu-id="09e14-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="09e14-110">Meddelandehastighetsgränsen på **30 meddelanden per minut** tillämpas i alla SKU:er.</span><span class="sxs-lookup"><span data-stu-id="09e14-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="09e14-111">Detta avgör hur många meddelanden en användare kan skicka från sitt Exchange Online-konto inom en angiven period.</span><span class="sxs-lookup"><span data-stu-id="09e14-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="09e14-112">Det **maximala antalet mottagare som tillåts i fälten Till, Kopia och Hemlig kopia** för ett enskilt e-postmeddelande, för alla SKU:er, är **1 000 mottagare.**</span><span class="sxs-lookup"><span data-stu-id="09e14-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="09e14-113">Om du vill anpassa den här gränsen går [du hit](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="09e14-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
