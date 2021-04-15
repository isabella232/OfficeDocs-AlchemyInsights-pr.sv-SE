---
title: 'Fel: Reglerna på den här datorn matchar inte'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782970"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Fel: Reglerna på den här datorn matchar inte

Information om uppdaterad status för det här kända problemet finns i Reglerna på den här datorn [matchar inte reglerna i Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Outlook-teamet har implementerat en korrigering i version 12928.10000. Korrigeringen är redan i Insider – snabbt och kommer till Månadskanal i slutet av juni 2020. När du har den åtgärdade versionen kan du få frågan "Vilka regler vill du behålla" en sista gång. Välj Server när du uppmanas att göra det och gå sedan tillbaka till Outlook och återaktivera alla regler som har inaktiverats.

Tills korrigeringen är tillgänglig kan du använda följande lösning:

**Lösning:** I de senaste rapporterna har problemet uppstått för de som endast har skapat klientregler i skrivbordsversionen av Outlook. Om du fortsätter att köra på problemet kan du ta bort reglerna och sedan skapa och redigera regler endast i OWA (Outlook Web App) tills problemet är löst.

Om du inte kan ta bort reglerna manuellt kan du köra ett Outlook-kommando när du startar Outlook genom att köra Outlook.exe /cleanrules. Detta tar bort både klient- och serverregler. Alla regler för alla konton i Outlook-profilen tas bort. Det här kommandot beskrivs ytterligare i artikeln Kommandoradsväxlar.

