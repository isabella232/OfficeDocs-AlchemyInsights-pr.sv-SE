---
title: Identifiera aktivitet för inkorgstransaktion i gransknings loggar
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
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779069"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifiera aktivitet för inkorgstransaktion i gransknings loggar

Du kan använda gransknings loggs ökning i Microsoft 365 Security & Compliance Center för att visa händelser för Inkorgshanteraren (skapa, ändra och ta bort regler för Inkorgen).

1. Logga in på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå till sidan **Sök**  >  **gransknings loggs sökning** .

3. Välj datum intervall i fälten **start datum** och **slutdatum** .

4. Under **Exchange-postaktiviteter**kontrollerar du att fältet **aktiviteter** är inställt på **ny-InboxRule skapa/ändra/Aktivera/inaktivera regler för Inkorgen**.

5. Klicka på **Sök**.

Välj en gransknings post i resultatet. I den utfällbara informationen klickar du på **Mer information**. Information om inställningarna för regel för Inkorgen visas i **parameter** fältet.

Mer information finns i [avgöra om en användare har skapat en regel för Inkorgen](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
