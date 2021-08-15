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
ms.openlocfilehash: e27c6433c65079af93f2a02a998b7179222336b0cae1149f4196f6fb6558ddac
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976883"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifiera aktivitet med inkorgsregel i granskningsloggar

Du kan använda granskningsloggsökning i Microsoft 365 Säkerhets- & säkerhetscenter för & för att visa inkorgsregelhändelser (skapa, ändra och ta bort inkorgsregler).

1. Logga in på [Microsoft 365 Kompatibilitetscenter.](https://protection.office.com/)

2. Gå till sidan **Sök**  >  **granskningsloggsökning.**

3. Välj datumintervallet i **fälten Startdatum** **och** Slutdatum.

4. Under **Exchange Postlådeaktiviteter** kontrollerar  du att fältet Aktiviteter är inställt på **Ny-InkorgRegel för skapa/ändra/aktivera/inaktivera inkorgsregel.**

5. Klicka **på Sök**.

Välj en granskningspost i resultatet. Klicka på Mer information i den **utfällade informationen.** Information om inställningarna för inkorgsregel visas i **fältet** Parametrar.

Mer information finns i Avgöra [om en användare har skapat en inkorgsregel](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
