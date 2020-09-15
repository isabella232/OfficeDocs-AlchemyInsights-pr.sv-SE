---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717379"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Åtgärda leverans problem för felkod 550 5.4.1 Relä åtkomst nekad

Det här problemet uppstår när [du kontrollerar om en e-postadress är giltig för att förhindra bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) när du anger Microsoft Network. Prova följande:

1. Avgöra om problemet är specifikt för en hel domän eller en enskild e-post adress:
    - Hela domänen: domänen måste synkroniseras. pröva att [ange domänen som intern och sedan tillbaka till auktoritär](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - En e-postadress: ibland måste adressen synkroniseras; att ändra SMTP-proxyadress och sedan ändra tillbaka den kan hjälpa dig.
2. Avgöra om problemet är specifikt för en grupp eller en gemensam mapp. För vissa objekt typer kan objekten behöva skapas manuellt i Azure Active Directory.

Om du behöver mer hjälp kan du öppna ett support ärende och ange omfattningen för problemet (inklusive den typ av objekt som du skickar till) så att du lättare får till gång till det.