---
title: Skapa en e-postfångst alla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286309"
---
# <a name="create-an-email-catch-all"></a>Skapa en e-postfångst alla

Användning av en fångst allt är starkt avskräckt. Det är bättre att ge en studs tillbaka till avsändaren låta avsändare vet att deras budskap inte kunde levereras som behandlas så att de kan vidta åtgärder. Du kan också begränsa den övervakade postlådan så att den bara fångar tidigare giltiga e-postadresser. 

Alla fångar alla brevlåda kommer att få en hel del spam och kan så småningom fylla om inte övervakas noga. (Det finns mottagningsgränser.) 

Om du bestämmer dig för att fortsätta följer du dessa steg:

1. Skapa en dynamisk distributionsgrupp & innehålla "Alla mottagartyper".

2. Skapa en dedikerad postlåda för att fånga e-postmeddelanden, till exempel catchall@domain.com.

3. För den specifika domänen anger du DomainType till "InternalRelay". Om du senare tar bort fångsten alla, se till att ställa in domänen tillbaka till auktoritativ.

4. Skapa en e-postflödestransportregel enligt följande:

    - Om avsändaren är "Utanför organisationen"
    - Omdirigera meddelandet till Catchall@domain.com
    - Förutom om mottagaren är medlem i allusers@domain.com (distributionsgruppen innehåller alla medlemmar)
    - Se till att verifiera att nya postlådor läggs till i den dynamiska distributionsgruppen
