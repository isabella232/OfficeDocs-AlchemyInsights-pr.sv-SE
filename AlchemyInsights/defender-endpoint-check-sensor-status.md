---
title: Defender Endpoint– kontrollera sensorstatus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676335"
---
# <a name="defender-endpoint-check-sensor-status"></a>Defender Endpoint– kontrollera sensorstatus

Panelen **Enheter med sensorproblem** finns på instrumentpanelen Säkerhetsåtgärder. Den här panelen ger information om den enskilda enhetens möjlighet att tillhandahålla sensordata och kommunicera med Defender för slutpunkt-tjänsten. Den rapporterar hur många enheter som kräver uppmärksamhet och hjälper dig att identifiera problematiska enheter och vidta åtgärder för att korrigera kända problem.

Två statusindikatorer på panelen anger information om antalet enheter som inte rapporterar korrekt till tjänsten:

- **Felkonfigurerad** Enheter som delvis kan rapportera sensordata till Defender för slutpunktstjänsten och kan ha konfigurationsfel som behöver korrigeras.
- **Inaktiv** Enheter som har slutat rapportera till Defender för slutpunktstjänsten i mer än sju dagar den senaste månaden.

Om du klickar på någon av grupperna dirigeras du till listan Enheter, filtrerad enligt dina val. I listan Enheter kan du filtrera hälsostatuslistan efter följande status:

- **Aktiv** Enheter som aktivt rapporterar till Defender för slutpunktstjänsten.
- **Felkonfigurerad** Enheter som delvis kan rapportera sensordata till Defender för slutpunkt-tjänsten men har konfigurationsfel som behöver korrigeras. Felkonfigurerade enheter kan ha en eller en kombination av följande problem:

    - Inga sensordata – Enheterna har slutat skicka sensordata. Begränsade aviseringar kan utlösas från enheten.
    - Nedsatt kommunikation – Möjligheten att kommunicera med en enhet är försämrad. Det kan hända att det inte fungerar att skicka filer för djupanalys, blockera filer, isolera enheten från nätverket och andra åtgärder som kräver kommunikation med enheten.
- **Inaktiv** Enheter som har stoppat rapporteringen till Defender för Slutpunkt-tjänsten.

Du kan ladda ned hela listan i CSV-format med hjälp av funktionen Exportera.

Mer information finns i Kontrollera [sensorhälsa i Microsoft Defender för slutpunkt](/microsoft-365/security/defender-endpoint/check-sensor-status).

Mer information om vad som orsakade att en enhet var inaktiv eller felaktigt konfigurerad finns i Åtgärda defekta sensor [i Microsoft Defender för Slutpunkt.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)
