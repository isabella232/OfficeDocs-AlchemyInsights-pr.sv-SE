---
title: EndPoint Manager – baslinjer för säkerhet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421092"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – baslinjer för säkerhet

Säkerhetsbaslinjer är förkonfigurerade grupper med Windows-inställningar som hjälper dig att tillämpa de säkerhetsinställningar som rekommenderas av relevanta säkerhetsteam. Dessa baslinjer kan anpassas så att de bara ger de inställningar och värden du önskar. Mer information om säkerhetsbaslinjer finns i Använda [säkerhetsbaslinjer för att konfigurera Windows 10-enheter i Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines)

Det finns för närvarande baslinjer för dessa produkter:

- Inställningar för Windows MDM-säkerhet
- Microsoft Defender för EndPoint-säkerhet
- Microsoft Edge

Alla baslinjer uppdateras regelbundet och släpps i stegvisa versioner. Varje version lägger till och tar bort inställningar från den föregående versionen för att säkerställa att baslinjen uppfyller aktuella riktlinjer. Med konsolen säkerhetsbaslinjer i Slutpunktssäkerhet kan olika versioner jämföras genom att ändringarna från version till version blir synliga.

Information om hur du på effektivast sätt ändrar vilken version av originalplan som distribueras finns i Hantera profiler för [säkerhetsbaslinje i Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)

När du har distribuerat en säkerhetsbaslinje kan du övervaka statusen för distributionen och granska inställningarna enhet för enhet.

**Obs!** Det kan ta upp till 24 timmar innan rapportdata för baslinjer visas från den första distributionen till en enhet och upp till 6 timmar för ytterligare uppdateringar. 

Den vanligaste orsaken till att en baslinjeinställning inte används är att samma inställning används i en annan profil. Det här scenariot kan undersökas för specifik enhet genom att välja enheten från noden Enhetsstatus i profilen Baslinje för säkerhet. Mer information finns i [Lösa konflikter för säkerhetsbaslinjer.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)