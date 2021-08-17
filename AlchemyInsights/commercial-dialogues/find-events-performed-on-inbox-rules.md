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
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882653"
---
# <a name="find-events-performed-on-inbox-rules"></a>Hitta händelser som utförs på inkorgsregler

När inkorgsregler skapas, ändras eller tas bort registreras händelser i granskningsloggen. Så här granskar du dem:

1. Gör något av följande:
   - I den Microsoft 365 Efterlevnadscenter går <https://compliance.microsoft.com> du till **Lösningsgranskning.** \>  Du kan också använda om du vill **gå direkt** till sidan <https://compliance.microsoft.com/auditlogsearch> Granskning.
   - I Microsoft 365 Defender på <https://security.microsoft.com> går du till **Granska**. Du kan också använda om du vill **gå direkt** till sidan <https://security.microsoft.com/auditlogsearch> Granskning.

    > [!NOTE]
    > Om du ser ett meddelande om att du måste aktivera granskning kan du aktivera den nu. Om den här funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.

2. Konfigurera **följande** inställningar på **fliken** Sök på sidan Granskning:
   - **Datum och tidsintervall:** Välj datum/tid i **rutorna Start** **och** Slut.
   - **Aktiviteter:** Välj **Ny inkorgRegel Skapa inkorgsregel från Outlook Web App**

3. När du är klar klickar du på **Sök**. Aktiviteterna visas på den nya **sidan Granskningssökning.**

4. Välj en aktivitet i resultatet för att öppna den utfällade informationen. Under **Parametrar** ser du namnet på regeln, villkorsuppsättningen och de åtgärder som regeln kommer att utföra.

Mer information finns i Söka [i granskningsloggen för att undersöka vanliga supportproblem.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
