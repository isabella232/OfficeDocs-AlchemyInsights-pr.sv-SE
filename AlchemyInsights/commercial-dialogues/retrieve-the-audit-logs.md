---
title: Hämta granskningsloggarna
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 88d28898923c1381c001c15445da90901b7e8761
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320461"
---
# <a name="retrieve-the-audit-logs"></a>Hämta granskningsloggarna

När du först öppnar granskningsloggen är den tom. Du måste göra en sökning för att se vad som finns där. Gör så här för att göra en allmän sökning för alla aktiviteter:

1. Gör något av följande:
   - I Microsoft 365 Efterlevnadscenter på <https://compliance.microsoft.com> går du till  \> **Lösningsgranskning.** Du kan också använda om du vill **gå direkt** till sidan <https://compliance.microsoft.com/auditlogsearch> Granskning.
   - Gå till Microsoft 365 Defender i <https://security.microsoft.com> portalen .  Du kan också använda om du vill **gå direkt** till sidan <https://security.microsoft.com/auditlogsearch> Granskning.

2. Konfigurera **följande** inställningar på **fliken** Sök på sidan Granskning:
   - **Datum och tidsintervall:** Välj datum/tid i **rutorna Start** **och** Slut.
   - **Aktiviteter:** Kontrollera **att Visa resultat för alla aktiviteter** är markerat.
   - **Användare:** Acceptera det tomma standardvärdet för att returnera resultat för alla användare, eller ange en eller flera användare.

3. När du är klar klickar du på **Sök**. Aktiviteterna visas på den nya **sidan Granskningssökning.**

4. Välj en aktivitet i resultatet för att öppna den utfällade informationen. Du ser mer information, till exempel klient, användare som utfört en åtgärd osv.

Mer information finns i Söka [i granskningsloggen för att undersöka vanliga supportproblem.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
