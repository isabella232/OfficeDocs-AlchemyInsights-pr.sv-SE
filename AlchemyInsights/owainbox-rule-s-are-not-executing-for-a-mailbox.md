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
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>En regel för Inkorgen fungerar inte som förväntat

Kontrol lera följande inställningar i Outlook på webben:

- Ett meddelande kan dirigeras om, vidarebefordras eller besvaras automatiskt baserat på regler för Inkorgen bara en gång. En regler för omdirigering (regler för Inkorgen eller regel för e-post, som även kallas Transport regel) kan lägga till högst tio vidarebefordrade mottagare i ett meddelande. Mer information finns i [begränsningar för journal, transport och Inkorgen](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Regler för Inkorgen fungerar inte på den alternativa journal post lådan. Få reda på mer om den [alternativa journal post lådan.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

Information om hur du åtgärdar dessa problem finns i [KB 2829319](https://support.microsoft.com/kb/2829319).

Om föregående problem inte gäller kör du rapporten regel för Inkorgshanteraren innan du eskalerar problemet till Microsoft Support:

1. Öppna post lådan i Outlook på webben och klicka på <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Inställningar**  >  för **Visa alla Outlook-inställningar**  >  **E-post**  >  **Regler**.

2. Längst ned på sidan klickar **du på om reglerna inte fungerar klicka här för att skapa en diagnostikrapport**.
