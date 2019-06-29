---
title: 1332 OWA - regler för Inkorgen inte körs för en postlåda
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 7d1848830847fc6722da20e09a4875f49bf02bd3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35360935"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="ef22d-102">En Inkorgsregel fungerar inte som förväntat</span><span class="sxs-lookup"><span data-stu-id="ef22d-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="ef22d-103">Kontrollera följande inställningar:</span><span class="sxs-lookup"><span data-stu-id="ef22d-103">Verify the following settings:</span></span>

- <span data-ttu-id="ef22d-104">Ett meddelande kan omdirigeras, vidarebefordrade eller besvarade automatiskt baserat på regler för Inkorgen bara en gång.</span><span class="sxs-lookup"><span data-stu-id="ef22d-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="ef22d-105">En regel som omdirigerar (en inkorg eller e-flöde regel, även kallad transport-regeln) kan lägga till högst tio mottagare för vidarebefordran till ett meddelande.</span><span class="sxs-lookup"><span data-stu-id="ef22d-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="ef22d-106">Mer information finns i [Journal, Transport, och Inkorgen gränserna](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="ef22d-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="ef22d-107">Regler för Inkorgen fungerar inte på alternativa journal postlåda.</span><span class="sxs-lookup"><span data-stu-id="ef22d-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="ef22d-108">Mer information om alternativa journaler postlådan finns [alternativa journal postlåda](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="ef22d-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="ef22d-109">Om du vill lösa de här problemen finns i [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="ef22d-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="ef22d-110">Om följande problem inte gäller kör den diagnostiska rapporten Inkorgen regeln innan du eskalera problemet till Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="ef22d-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="ef22d-111">Öppna postlådan i Outlook på webben och klicka på **Inställningar** \> **Alternativ** \> **Ordna e-post** \> **regler för Inkorgen**.</span><span class="sxs-lookup"><span data-stu-id="ef22d-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="ef22d-112">Klicka på **om reglerna inte fungerar Klicka här för att generera en diagnostisk rapport**längst ned på sidan.</span><span class="sxs-lookup"><span data-stu-id="ef22d-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
