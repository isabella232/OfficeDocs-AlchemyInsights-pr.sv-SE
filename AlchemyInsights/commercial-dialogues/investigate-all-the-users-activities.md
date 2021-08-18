---
title: Undersöka alla användarnas aktiviteter
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332361"
---
# <a name="investigate-all-the-users-activities"></a>Undersöka alla användarnas aktiviteter

Gör så här:

1. Gör något av följande:
   - I Microsoft 365 Efterlevnadscenter på <https://compliance.microsoft.com> går du till  \> **Lösningsgranskning.** Du kan också använda om du vill **gå direkt** till sidan <https://compliance.microsoft.com/auditlogsearch> Granskning.
   - Gå till Microsoft 365 Defender i <https://security.microsoft.com> portalen .  Du kan också använda om du vill **gå direkt** till sidan <https://security.microsoft.com/auditlogsearch> Granskning.

    **Obs!** Om du ser ett meddelande om att du måste aktivera funktionen kan du aktivera den nu. Om funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.

2. Konfigurera **följande** inställningar på **fliken** Sök på sidan Granskning:
   - **Datum och tidsintervall:** Välj datum/tid i **rutorna Start** **och** Slut.
   - **Aktiviteter**: Om du är intresserad av en viss aktivitet väljer du den i listan. I annat fall returnerar **standardvärdet Visa resultat för alla** aktiviteter alla aktiviteter.
   - **Användare:** Acceptera det tomma standardvärdet för att returnera resultat för alla användare, eller ange en eller flera användare.

3. När du är klar klickar du på **Sök**. Aktiviteterna visas på den nya **sidan Granskningssökning.** Du ser **IP-adressen,** **användaren och** **aktivitetsnamnet.**

4. Om du vill  ladda ned resultaten väljer du \> **Exportera ladda ned alla resultat.**

5. Välj en aktivitet i resultatet för att öppna den utfällade informationen.

Mer information finns i Söka [i granskningsloggen för att undersöka vanliga supportproblem.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
