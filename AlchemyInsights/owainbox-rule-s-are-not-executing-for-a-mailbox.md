---
title: 1332 OWA – inkorgsregelerna körs inte för en postlåda
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
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040920"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>En inkorgsregel fungerar inte som förväntat

Kontrollera följande inställningar i Outlook på webben:

- Ett meddelande kan endast omdirigeras, vidarebefordras eller besvaras automatiskt baserat på regler för Inkorgen en gång. En omdirigeringsregel (en inkorgsregel eller e-postflödesregel, kallas även transportregel) kan lägga till maximalt tio mottagare för vidarebefordran i ett meddelande. Mer information finns i Gränser [för journal-, transport- och inkorgsregel.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- Inkorgsregler fungerar inte på den alternativa journalpostlådan. Mer information om den alternativa postlådan för journaler finns i [Alternativ journalföringspostlåda.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

Information om hur du åtgärdar dessa problem [finns i KB 2829319](https://support.microsoft.com/kb/2829319).

Om de tidigare problemen inte gäller bör du köra diagnostikrapporten för inkorgsregeln innan du eskalerar problemet till Microsoft Support:

1. Öppna postlådan i Outlook på webben klicka på <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Inställningar**  >  **Visa alla Outlook Inställningar**  >  **E-post**  >  **Regler.**

2. Längst ned på sidan klickar du på **Om reglerna inte fungerar klickar du här för att skapa en diagnostikrapport.**
