---
title: Skapa ett e-postmeddelande för att få tag på allt
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816218"
---
# <a name="create-an-email-catch-all"></a>Skapa ett e-postmeddelande för att få tag på allt

Man avråder starkt från att använda en fångad information. Det är bättre att tillhandahålla ett studsa tillbaka till avsändaren så att avsändare vet att deras meddelande inte kunde levereras som adresserat så att de kan vidta åtgärder. Du kan också begränsa den övervakade postlådan till att endast fånga upp tidigare giltiga e-postadresser. 

All catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitor. (Det finns mottagande gränser.) 

Följ de här anvisningarna om du bestämmer dig för att fortsätta:

1. Skapa en dynamisk distributionsgrupp där & "Alla mottagartyper".

2. Skapa en dedikerad postlåda för att fånga upp e-postmeddelanden, till exempel catchall@domain.com.

3. För den specifika domänen anger du DomainType till "InternalRelay". Om du senare tar bort alla, se till att ange domänen som Auktoritativ.

4. Skapa en transportregel för e-postflöde enligt följande:

    - Om avsändaren är "utanför organisationen"
    - Omdirigera meddelandet till Catchall@domain.com
    - Förutom om mottagaren är medlem i allusers@domain.com (distributionsgruppen innehåller alla medlemmar)
    - Kontrollera att nya postlådor läggs till i gruppen Dynamisk distribution
