---
title: Läsa granskningsloggarna för borttagna händelser
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
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324751"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Läsa granskningsloggarna för borttagna händelser

Gör så här:

1. Gör något av följande:
   - I Microsoft 365 Efterlevnadscenter på <https://compliance.microsoft.com> går du till  \> **Lösningsgranskning.** Du kan också använda om du vill **gå direkt** till sidan <https://compliance.microsoft.com/auditlogsearch> Granskning.
   - Gå till Microsoft 365 Defender i <https://security.microsoft.com> portalen .  Du kan också använda om du vill **gå direkt** till sidan <https://security.microsoft.com/auditlogsearch> Granskning.

    **Obs!** Om du ser ett meddelande om att du måste aktivera funktionen kan du aktivera den nu. Om funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.

2. Konfigurera **följande** inställningar på **fliken** Sök på sidan Granskning:
   - **Datum och tidsintervall:** Välj datum/tid i **rutorna Start** **och** Slut.
   - **Aktiviteter:** Exchange **postlådeaktiviteter** och välj sedan följande värden:
     - **Meddelanden togs bort från mappen Borttaget**
     - **Meddelanden flyttades till mappen Borttaget**

       När du är klar klickar du utanför fönstret för att minimera **fönstret** Aktiviteter.

   - **Användare:** Acceptera det tomma standardvärdet för att returnera resultat för alla användare, eller ange en eller flera användare.

3. När du är klar klickar du på **Sök**. Aktiviteterna visas på den nya **sidan Granskningssökning.**

4. Välj en aktivitet i resultatet för att öppna den utfällade informationen. Mer information om det borttagna objektet, till exempel ämnesraden och platsen för objektet när det togs bort, visas i **fältet AffectedItems.**

   **Obs!** Du kan inte återställa borttagna objekt med granskningsloggfunktionen. Information om hur du återställer borttagna objekt [finns i Återskapa borttagna e-postmeddelanden i Outlook på webben](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Mer information finns i Söka i [granskningsloggen för att undersöka vanliga supportproblem.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
