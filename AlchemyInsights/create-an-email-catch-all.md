---
title: Skapa ett e-postmeddelande för att få tag på allt
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816218"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="182ef-102">Skapa ett e-postmeddelande för att få tag på allt</span><span class="sxs-lookup"><span data-stu-id="182ef-102">Create an email catch all</span></span>

<span data-ttu-id="182ef-103">Man avråder starkt från att använda en fångad information.</span><span class="sxs-lookup"><span data-stu-id="182ef-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="182ef-104">Det är bättre att tillhandahålla ett studsa tillbaka till avsändaren så att avsändare vet att deras meddelande inte kunde levereras som adresserat så att de kan vidta åtgärder.</span><span class="sxs-lookup"><span data-stu-id="182ef-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="182ef-105">Du kan också begränsa den övervakade postlådan till att endast fånga upp tidigare giltiga e-postadresser.</span><span class="sxs-lookup"><span data-stu-id="182ef-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="182ef-106">All catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitor.</span><span class="sxs-lookup"><span data-stu-id="182ef-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="182ef-107">(Det finns mottagande gränser.)</span><span class="sxs-lookup"><span data-stu-id="182ef-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="182ef-108">Följ de här anvisningarna om du bestämmer dig för att fortsätta:</span><span class="sxs-lookup"><span data-stu-id="182ef-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="182ef-109">Skapa en dynamisk distributionsgrupp där & "Alla mottagartyper".</span><span class="sxs-lookup"><span data-stu-id="182ef-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="182ef-110">Skapa en dedikerad postlåda för att fånga upp e-postmeddelanden, till exempel catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="182ef-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="182ef-111">För den specifika domänen anger du DomainType till "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="182ef-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="182ef-112">Om du senare tar bort alla, se till att ange domänen som Auktoritativ.</span><span class="sxs-lookup"><span data-stu-id="182ef-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="182ef-113">Skapa en transportregel för e-postflöde enligt följande:</span><span class="sxs-lookup"><span data-stu-id="182ef-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="182ef-114">Om avsändaren är "utanför organisationen"</span><span class="sxs-lookup"><span data-stu-id="182ef-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="182ef-115">Omdirigera meddelandet till Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="182ef-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="182ef-116">Förutom om mottagaren är medlem i allusers@domain.com (distributionsgruppen innehåller alla medlemmar)</span><span class="sxs-lookup"><span data-stu-id="182ef-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="182ef-117">Kontrollera att nya postlådor läggs till i gruppen Dynamisk distribution</span><span class="sxs-lookup"><span data-stu-id="182ef-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
