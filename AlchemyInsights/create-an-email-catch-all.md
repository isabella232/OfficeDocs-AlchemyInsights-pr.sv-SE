---
title: Skapa en e-postfångst alla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286309"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="19b11-102">Skapa en e-postfångst alla</span><span class="sxs-lookup"><span data-stu-id="19b11-102">Create an email catch all</span></span>

<span data-ttu-id="19b11-103">Användning av en fångst allt är starkt avskräckt.</span><span class="sxs-lookup"><span data-stu-id="19b11-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="19b11-104">Det är bättre att ge en studs tillbaka till avsändaren låta avsändare vet att deras budskap inte kunde levereras som behandlas så att de kan vidta åtgärder.</span><span class="sxs-lookup"><span data-stu-id="19b11-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="19b11-105">Du kan också begränsa den övervakade postlådan så att den bara fångar tidigare giltiga e-postadresser.</span><span class="sxs-lookup"><span data-stu-id="19b11-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="19b11-106">Alla fångar alla brevlåda kommer att få en hel del spam och kan så småningom fylla om inte övervakas noga.</span><span class="sxs-lookup"><span data-stu-id="19b11-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="19b11-107">(Det finns mottagningsgränser.)</span><span class="sxs-lookup"><span data-stu-id="19b11-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="19b11-108">Om du bestämmer dig för att fortsätta följer du dessa steg:</span><span class="sxs-lookup"><span data-stu-id="19b11-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="19b11-109">Skapa en dynamisk distributionsgrupp & innehålla "Alla mottagartyper".</span><span class="sxs-lookup"><span data-stu-id="19b11-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="19b11-110">Skapa en dedikerad postlåda för att fånga e-postmeddelanden, till exempel catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="19b11-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="19b11-111">För den specifika domänen anger du DomainType till "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="19b11-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="19b11-112">Om du senare tar bort fångsten alla, se till att ställa in domänen tillbaka till auktoritativ.</span><span class="sxs-lookup"><span data-stu-id="19b11-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="19b11-113">Skapa en e-postflödestransportregel enligt följande:</span><span class="sxs-lookup"><span data-stu-id="19b11-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="19b11-114">Om avsändaren är "Utanför organisationen"</span><span class="sxs-lookup"><span data-stu-id="19b11-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="19b11-115">Omdirigera meddelandet till Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="19b11-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="19b11-116">Förutom om mottagaren är medlem i allusers@domain.com (distributionsgruppen innehåller alla medlemmar)</span><span class="sxs-lookup"><span data-stu-id="19b11-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="19b11-117">Se till att verifiera att nya postlådor läggs till i den dynamiska distributionsgruppen</span><span class="sxs-lookup"><span data-stu-id="19b11-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
