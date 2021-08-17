---
title: Hitta händelser som utförs på inkorgsregler
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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313517"
---
# <a name="find-events-performed-on-inbox-rules"></a>Hitta händelser som utförs på inkorgsregler

När inkorgsregler skapas, ändras eller tas bort registreras händelser i granskningsloggen. Så här granskar du dem:

1. Gör något av följande:
   - I Microsoft 365 Efterlevnadscenter på <https://compliance.microsoft.com> går du till  \> **Lösningsgranskning.** Du kan också använda om du vill **gå direkt** till sidan <https://compliance.microsoft.com/auditlogsearch> Granskning.
   - Gå till Microsoft 365 Defender i <https://security.microsoft.com> portalen .  Du kan också använda om du vill **gå direkt** till sidan <https://security.microsoft.com/auditlogsearch> Granskning.

    **Obs!** Om du ser ett meddelande om att du måste aktivera granskning kan du aktivera den nu. Om den här funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.
1. Välj fältet Aktiviteter och leta reda Exchange postlådeaktiviteter och välj sedan New-InboxRule Skapa inkorgsregel från Outlook Web App. När du är klar klickar du utanför fönstret för att minimera fönstret Aktiviteter.
1. Ange datumintervallet och välj sedan användarnamnet för den användare du vill undersöka i fältet Användare. Du kan välja fler än en användare i taget.
1. Välj Sök. Aktiviteterna visas under Resultat.
1. Om du vill visa information väljer du en aktivitet och sedan Mer information. Under Parametrar ser du namnet på regeln, villkorsuppsättningen och de åtgärder som regeln kommer att utföra.

2. Konfigurera **följande** inställningar på **fliken** Sök på sidan Granskning:
   - **Datum och tidsintervall:** Välj datum/tid i **rutorna Start** **och** Slut.
   - **Aktiviteter:** Välj **Ny inkorgRegel Skapa inkorgsregel från Outlook Web App**

3. När du är klar klickar du på **Sök**. Aktiviteterna visas på den nya **sidan Granskningssökning.**

4. Välj en aktivitet i resultatet för att öppna den utfällade informationen. Under **Parametrar** ser du namnet på regeln, villkorsuppsättningen och de åtgärder som regeln kommer att utföra.

Mer information finns i Söka [i granskningsloggen för att undersöka vanliga supportproblem.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
