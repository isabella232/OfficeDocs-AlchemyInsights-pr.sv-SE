---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932295"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Korrigera leveransproblem för felkod 550 5.4.1 Nekad reläåtkomst

Det här problemet inträffar när [du kontrollerar om en e-postadress är giltig för att förhindra återstuds när](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) du går till Microsoft-nätverket. Prova följande:

1. Avgör om problemet är specifikt för en hel domän eller en enda e-postadress:
    - Hela domänen: Ibland behöver domänen synkroniseras. Prova [att ange domänen som Intern och sedan tillbaka till Auktoritativ](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Enskild e-postadress: Ibland behöver adressen synkroniseras. Det kan vara bra att ändra smtp-proxyadressen och sedan ändra tillbaka den.
2. Avgör om problemet är specifikt för en grupp eller offentlig mapp. För vissa objekttyper kan objekten behöva skapas manuellt i Azure Active Directory.

Om du behöver mer hjälp kan du öppna ett support ärende och ange omfattningen av problemet (inklusive typen av objekt som du skickar till) så att vi kan hjälpa dig bättre.