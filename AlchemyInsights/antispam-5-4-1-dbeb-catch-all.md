---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707929"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Åtgärda leveransproblem för felkod 550 5.4.1 Relay Access Nekad

Det hÃ¤r problemet uppstÃ¥r vid [kontroll av om en e-postadress är giltig för att förhindra bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) nÃ¤r du går in i Microsoft-nätverket. Prova följande:

1. Ta reda på om problemet är specifikt för en hel domän eller en enda e-postadress:
    - Hela domänen: Ibland måste domänen synkroniseras. prova [att ställa in domänen på Internt och sedan tillbaka till Auktoritär .](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Enkel e-postadress: Ibland måste adressen synkroniseras. ändra smtp proxyadress och sedan ändra tillbaka det kan hjälpa.
2. Ta reda på om problemet är specifikt för en grupp eller gemensam mapp. För vissa objekttyper kan objekten behöva skapas manuellt i Azure Active Directory.

Om du behöver ytterligare hjälp kan du öppna en supportbiljett och ange problemets omfattning (inklusive vilken typ av objekt du skickar till) så att vi kan hjälpa dig bättre.