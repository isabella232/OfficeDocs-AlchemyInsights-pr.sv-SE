---
title: Skapa ett e-postmeddelande Catch alla
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
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713004"
---
# <a name="create-an-email-catch-all"></a>Skapa ett e-postmeddelande Catch alla

Det är starkt att använda en helt mer. Det är bättre att erbjuda en studs tillbaka till avsändaren och meddela att det inte gick att skicka meddelanden till mottagaren. Du kan också begränsa den övervakade post lådan så att den endast fångar upp tidigare giltiga e-postadresser. 

Alla fångar alla post lådor får ett bra sätt att skicka skräp post och kan till och med fylla om de inte bör övervakas. (Det finns begränsningar.) 

Om du vill fortsätta följer du de här stegen:

1. Skapa en dynamisk distributions grupp & inkludera "alla mottagar typer".

2. Skapa en dedikerad post låda för att hämta e-post, till exempel catchall@domain.com.

3. Ange DomainType till "InternalRelay" för den specifika domänen. Om du senare tar bort Catch-alla ska du se till att återställa domänen till auktoritär.

4. Skapa en flödes schema regel för flöden så här:

    - Om avsändaren är "utanför organisationen"
    - Omdirigera meddelandet till Catchall@domain.com
    - Förutom om mottagaren är medlem i allusers@domain.com (distributions gruppen innehåller alla medlemmar)
    - Kontrol lera att nya post lådor läggs till i den dynamiska distributions gruppen
