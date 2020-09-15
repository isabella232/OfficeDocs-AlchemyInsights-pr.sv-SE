---
title: Skapa ett e-postmeddelande Catch alla
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
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713004"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="a6fec-102">Skapa ett e-postmeddelande Catch alla</span><span class="sxs-lookup"><span data-stu-id="a6fec-102">Create an email catch all</span></span>

<span data-ttu-id="a6fec-103">Det är starkt att använda en helt mer.</span><span class="sxs-lookup"><span data-stu-id="a6fec-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="a6fec-104">Det är bättre att erbjuda en studs tillbaka till avsändaren och meddela att det inte gick att skicka meddelanden till mottagaren.</span><span class="sxs-lookup"><span data-stu-id="a6fec-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="a6fec-105">Du kan också begränsa den övervakade post lådan så att den endast fångar upp tidigare giltiga e-postadresser.</span><span class="sxs-lookup"><span data-stu-id="a6fec-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="a6fec-106">Alla fångar alla post lådor får ett bra sätt att skicka skräp post och kan till och med fylla om de inte bör övervakas.</span><span class="sxs-lookup"><span data-stu-id="a6fec-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="a6fec-107">(Det finns begränsningar.)</span><span class="sxs-lookup"><span data-stu-id="a6fec-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="a6fec-108">Om du vill fortsätta följer du de här stegen:</span><span class="sxs-lookup"><span data-stu-id="a6fec-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="a6fec-109">Skapa en dynamisk distributions grupp & inkludera "alla mottagar typer".</span><span class="sxs-lookup"><span data-stu-id="a6fec-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="a6fec-110">Skapa en dedikerad post låda för att hämta e-post, till exempel catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="a6fec-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="a6fec-111">Ange DomainType till "InternalRelay" för den specifika domänen.</span><span class="sxs-lookup"><span data-stu-id="a6fec-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="a6fec-112">Om du senare tar bort Catch-alla ska du se till att återställa domänen till auktoritär.</span><span class="sxs-lookup"><span data-stu-id="a6fec-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="a6fec-113">Skapa en flödes schema regel för flöden så här:</span><span class="sxs-lookup"><span data-stu-id="a6fec-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="a6fec-114">Om avsändaren är "utanför organisationen"</span><span class="sxs-lookup"><span data-stu-id="a6fec-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="a6fec-115">Omdirigera meddelandet till Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="a6fec-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="a6fec-116">Förutom om mottagaren är medlem i allusers@domain.com (distributions gruppen innehåller alla medlemmar)</span><span class="sxs-lookup"><span data-stu-id="a6fec-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="a6fec-117">Kontrol lera att nya post lådor läggs till i den dynamiska distributions gruppen</span><span class="sxs-lookup"><span data-stu-id="a6fec-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
