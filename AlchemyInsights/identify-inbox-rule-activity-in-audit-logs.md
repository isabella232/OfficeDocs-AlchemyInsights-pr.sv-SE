---
title: Identifiera aktivitet med inkorgsregel i granskningsloggar
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331141"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifiera aktivitet med inkorgsregel i granskningsloggar

Du kan använda granskningsloggsökning i Microsoft 365 Efterlevnadscenter om du vill visa inkorgsregelhändelser (skapa, ändra och ta bort inkorgsregler).

1. Gör något av följande:
   - I Microsoft 365 Efterlevnadscenter på <https://compliance.microsoft.com> går du till  \> **Lösningsgranskning.** Du kan också använda om du vill **gå direkt** till sidan <https://compliance.microsoft.com/auditlogsearch> Granskning.
   - Gå till Microsoft 365 Defender i <https://security.microsoft.com> portalen .  Du kan också använda om du vill **gå direkt** till sidan <https://security.microsoft.com/auditlogsearch> Granskning.

2. Konfigurera **följande** inställningar på **fliken** Sök på sidan Granskning:
   - **Datum och tidsintervall:** Välj datum/tid i **rutorna Start** **och** Slut.
   - **Aktiviteter:** Välj ett eller flera av följande värden:
     - **Ny inkorgRegel för att skapa inkorg från Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Uppdatera regler för Inkorgen Outlook klient**

3. När du är klar klickar du på **Sök**. Aktiviteterna visas på den nya **sidan Granskningssökning.**

4. Välj en aktivitet i resultatet för att öppna den utfällade informationen. Information om inställningarna för inkorgsregel visas i **fältet** Parametrar.

Mer information finns i Avgöra [om en användare har skapat en inkorgsregel](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
