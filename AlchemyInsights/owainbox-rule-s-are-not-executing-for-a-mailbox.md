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
ms.openlocfilehash: 218a05a8d321b76dd07345ea48d6b3e158cc120e
ms.sourcegitcommit: 77f704672b7c7de541899e25c022ff10c111e304
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2019
ms.locfileid: "36204078"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>En Inkorgsregel fungerar inte som förväntat

Kontrollera följande inställningar:

- Ett meddelande kan omdirigeras, vidarebefordrade eller besvarade automatiskt baserat på regler för Inkorgen bara en gång. En regel som omdirigerar (en inkorg eller e-flöde regel, även kallad transport-regeln) kan lägga till högst tio mottagare för vidarebefordran till ett meddelande. Mer information finns i [Journal, Transport, och Inkorgen gränserna](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Regler för Inkorgen fungerar inte på alternativa journal postlåda. Mer information om alternativa journaler postlådan finns [alternativa journal postlåda](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Om du vill lösa de här problemen finns i [KB 2829319](https://support.microsoft.com/kb/2829319).

Om följande problem inte gäller kör den diagnostiska rapporten Inkorgen regeln innan du eskalera problemet till Microsoft Support:

1. Öppna postlådan i Outlook på webben och klicka på <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Inställningar** > **Visa alla Outlook-inställningar** > **e** > **regler**.

2. Klicka på **om reglerna inte fungerar Klicka här för att generera en diagnostisk rapport**längst ned på sidan.
