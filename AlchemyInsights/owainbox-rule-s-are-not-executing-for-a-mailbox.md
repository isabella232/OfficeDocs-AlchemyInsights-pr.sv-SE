---
title: 1332 OWA-Inkorgshanteraren körs inte för en post låda
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721609"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="5e3d0-102">En regel för Inkorgen fungerar inte som förväntat</span><span class="sxs-lookup"><span data-stu-id="5e3d0-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="5e3d0-103">Kontrol lera följande inställningar i Outlook på webben:</span><span class="sxs-lookup"><span data-stu-id="5e3d0-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="5e3d0-104">Ett meddelande kan dirigeras om, vidarebefordras eller besvaras automatiskt baserat på regler för Inkorgen bara en gång.</span><span class="sxs-lookup"><span data-stu-id="5e3d0-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="5e3d0-105">En regler för omdirigering (regler för Inkorgen eller regel för e-post, som även kallas Transport regel) kan lägga till högst tio vidarebefordrade mottagare i ett meddelande.</span><span class="sxs-lookup"><span data-stu-id="5e3d0-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="5e3d0-106">Mer information finns i [begränsningar för journal, transport och Inkorgen](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="5e3d0-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="5e3d0-107">Regler för Inkorgen fungerar inte på den alternativa journal post lådan.</span><span class="sxs-lookup"><span data-stu-id="5e3d0-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="5e3d0-108">Få reda på mer om den [alternativa journal post lådan.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)</span><span class="sxs-lookup"><span data-stu-id="5e3d0-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="5e3d0-109">Information om hur du åtgärdar dessa problem finns i [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="5e3d0-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="5e3d0-110">Om föregående problem inte gäller kör du rapporten regel för Inkorgshanteraren innan du eskalerar problemet till Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="5e3d0-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="5e3d0-111">Öppna post lådan i Outlook på webben och klicka på</span><span class="sxs-lookup"><span data-stu-id="5e3d0-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="5e3d0-112">**Inställningar**  >  för **Visa alla Outlook-inställningar**  >  **E-post**  >  **Regler**.</span><span class="sxs-lookup"><span data-stu-id="5e3d0-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="5e3d0-113">Längst ned på sidan klickar **du på om reglerna inte fungerar klicka här för att skapa en diagnostikrapport**.</span><span class="sxs-lookup"><span data-stu-id="5e3d0-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
