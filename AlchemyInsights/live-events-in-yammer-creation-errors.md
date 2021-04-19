---
title: Fel när livehändelser ska skapas i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825533"
---
# <a name="live-events-in-yammer-creation-errors"></a>Fel när livehändelser ska skapas i Yammer

**Skapa en livehändelse i Yammer**

Alternativet för att skapa en livehändelse visas alltid i Yammer. I vissa fall kanske inte användare uppfyller kraven för att skapa en livehändelse och de får då ett felmeddelande när de försöker skapa den. Nedan hittar du vanliga orsaker för det här problemet och olika sätt att lösa det för slutanvändarna.

**Vem kan skapa livehändelser**
- En licens för Office 365 Enterprise E1, E3 eller E5 eller en licens för Office 365 A3 eller A5.
- Behörighet att skapa livehändelser i administrationscentret för Microsoft Teams.
- Behörighet att skapa livehändelser i Microsoft Stream (för händelser som produceras med en extern sändningsapp eller enhet).
- Fullständigt gruppmedlemskap i organisationen (får inte vara gäst eller från en annan organisation).
- Schemaläggning av privata möten, skärmdelning och IP-videodelning är aktiverat i principen för Teams-möten.

**Principer för att skapa livehändelser**

Yammer följer de principer för livehändelser som anges i Office 365-klientorganisationen för Stream. Som standard kan alla i din organisation skapa en livehändelse. Administratörer kan [ändra den här inställningen vilket kan hindra användarna från att skapa en livehändelse](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating). Det är viktigt att kontrollera att användarna har behörighet att skapa livehändelser om de får ett principfel.
