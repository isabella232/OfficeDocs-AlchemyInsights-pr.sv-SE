---
title: 'Fel: Reglerna på den här datorn matchar inte'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/09/2020
ms.locfileid: "44618031"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Fel: Reglerna på den här datorn matchar inte

Information om hur du ser uppdaterad status för det här kända problemet finns [i Reglerna på den här datorn matchar inte reglerna för Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Outlook-teamet har implementerat en korrigering i Build 12928.10000. Korrigeringen är redan på Insider Fast och kommer att gå till Monthly Channel i slutet av juni 2020. När du har den fasta bygga kan du få prompten "Vilka regler vill du behålla" en sista gång. Välj Server när du uppmanas att göra det och gå sedan tillbaka till Outlook och aktivera alla regler som har inaktiverats igen.

Tills korrigeringen är tillgänglig kan du använda följande lösning:

**Lösning**: I de senaste rapporterna har problemet uppstått för dem som bara har skapat klientregler i Outlook-skrivbordet. Om du fortsätter att stöta på problemet kan du överväga att ta bort reglerna och sedan skapa och redigera regler endast i OWA (Outlook Web App) tills problemet är löst.

Om du inte kan ta bort reglerna manuellt kan du köra ett Outlook-kommando när du startar Outlook genom att köra Outlook.exe /cleanrules. Detta tar bort både klient- och serverregler. Alla regler för alla konton i Outlook-profilen tas bort. Det här kommandot dokumenteras ytterligare i artikeln Kommandoradsväxlar.