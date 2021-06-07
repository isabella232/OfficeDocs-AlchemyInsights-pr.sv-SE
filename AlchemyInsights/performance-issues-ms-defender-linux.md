---
title: Prestandaproblem för Microsoft Defender för Slutpunkt i Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794225"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Prestandaproblem för Microsoft Defender för Slutpunkt i Linux

Den här artikeln leder dig genom stegen för att identifiera prestandaproblem för Microsoft Defender för Endpoint på Linux.

Det är viktigt att du först kontrollerar att problemet är löst i den [senaste versionen.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

Information om hur du startar din undersökning [finns i Felsöka prestandaproblem för Microsoft Defender för Endpoint på Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Undantag

Undantag kan bidra till att minimera prestandaproblem. Granska undantagen innan du börjar så att alla ytterligare risker är kända och har dokumenterats.

Mer information finns i [Konfigurera och validera undantag för Microsoft Defender för Endpoint på Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)

När du har flera & mappar som ska undantas och de alla finns på samma monteringspunkt, kan det vara enklare att utesluta fästpunkten. Från och med februari version 101.22.80 kan du utesluta en hel monteringspunkt.

Om till exempel /mnt/backup är en monteringspunkt kan du lägga till /mnt/backup i exkluderingslistan genom att köra det här kommandot:

`$ mdatp exclusion folder add –path /mnt/backup`

**Obs!** Om du lägger till undantag ökar risken för att skadlig programvara inte identifieras och bör hanteras och implementeras med försiktighet.

## <a name="need-help"></a>Behöver du hjälp?

Samla in diagnostikdata innan du öppnar ett supportfall för att hjälpa dig på det mest effektiva sättet.
