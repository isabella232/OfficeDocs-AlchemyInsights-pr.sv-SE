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
ms.openlocfilehash: 3bda32b55be9c2fa671376e73b06aadfbe976363
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630195"
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
