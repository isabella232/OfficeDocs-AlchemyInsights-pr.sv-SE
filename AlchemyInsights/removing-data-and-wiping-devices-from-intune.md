---
title: Ta bort data och rensa enheter från Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440465"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Ta bort data och rensa enheter från Intune

Fjärråtgärderna Enhetsåterställning och Enhetsrensning kan användas för att ta bort företagsdata som hanteras av Intune eller för att utföra en fabriksåterställning och återställa enheten till standardinställningarna.

1. Logga in på Microsoft 365 Device Management och gå till **Enheter**  >  **alla enheter**.
2. Markera den enhet som du vill rensa.
3. Välj den typ av fjärrrensning du vill göra. Dra bara bort organisationsinformation, medan fullständiga rensningar återställer enheten till fabriksinställningarna.
4. Välj **Ja** för att bekräfta. Tills rensningen är klar visas åtgärdsstatusen Enhet som Gå i pension i väntan.</br>
    När åtgärden är klar ser du inte längre den mobila enheten i listan över hanterade enheter.

**Anm.)** Företagsdata kan inte tas bort från enheter som är anslutna till Azure AD.

Fullständig information om effekten av åtgärderna Gå tillbaka och Rensa, inklusive vad som behålls och vad som tas bort, finns i [Ta bort enheter med hjälp av rensning, dra tillbaka eller manuellt avregistrera enheten](https://docs.microsoft.com/intune/devices-wipe).

Information om hur du raderar alla data från en macOS-enhet finns i [Radera alla data från en macOS-enhet](https://docs.microsoft.com/intune/device-erase).