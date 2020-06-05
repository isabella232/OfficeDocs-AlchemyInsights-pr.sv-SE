---
title: 1332 OWA - Inkorgsregeln eller -regler körs inte för en postlåda
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576578"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>En inkorgsregel fungerar inte som förväntat

Kontrollera följande inställningar i Outlook på webben:

- Ett meddelande kan omdirigeras, vidarebefordras eller besvaras automatiskt baserat på Inkorgsregler endast en gång. En omdirigeringsregel (en inkorgsregel eller regel för e-postflöde, även kallad transportregel) kan lägga till högst tio vidarebefordringsmottagare i ett meddelande. Mer information finns i [regelgränser för journal, transport och inkorg](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Inkorgsregler fungerar inte på den alternativa journalpostlådan. Mer information om den alternativa journalpostlådan finns i [Alternativ journalpostlåda](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Åtgärda dessa problem finns i [KB 2829319](https://support.microsoft.com/kb/2829319).

Om de tidigare problemen inte gäller kör du diagnostikrapporten för inkorgsregeln innan du eskalerar problemet till Microsoft Support:

1. Öppna postlådan i Outlook på webben och klicka på <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Inställningar**  >  **Visa alla Outlook-inställningar**  >  **E-post**  >  **Regler**.

2. Längst ned på sidan klickar du på **Om reglerna inte fungerar klickar du här för att generera en diagnostikrapport**.
