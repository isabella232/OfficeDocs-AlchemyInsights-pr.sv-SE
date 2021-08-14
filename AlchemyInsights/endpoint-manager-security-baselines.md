---
title: EndPoint Manager – Säkerhetsbaslinjer
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
- "10064"
- "9003771"
ms.openlocfilehash: c13bc161b19a5fef1352beb28bdcc20110111a9a61a47433d82e1e69aff7f88d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978179"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – Säkerhetsbaslinjer

Säkerhetsbaslinjer är förkonfigurerade grupper med Windows-inställningar som hjälper dig att använda de säkerhetsinställningar som rekommenderas av relevanta säkerhetsteam. Dessa baslinjer kan anpassas så att endast önskade inställningar och värden levereras. Mer information om säkerhetsbaslinjer finns i [Använda säkerhetsbaslinjer för att konfigurera Windows 10-enheter i Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Det finns för närvarande baslinjer för dessa produkter:

- Säkerhetsinställningar för Windows MDM
- Säkerhet för Microsoft Defender för Endpoint
- Microsoft Edge

Alla baslinjer uppdateras regelbundet och publiceras i stegvisa versioner. Varje version lägger till och tar bort inställningar från den tidigare versionen för att säkerställa att baslinjen uppfyller aktuella riktlinjer. Med säkerhetsbaslinjekonsolen i Endpoint-säkerhet kan olika versioner jämföras genom att göra ändringarna från version till version synliga.

Mer information om hur du bäst ändrar vilken version av baslinjen som distribueras finns i [Hantera säkerhetsbaslinjeprofiler i Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

När du har distribuerat en säkerhetsbaslinje kan du övervaka distributionstillståndet och granska inställningarna för varje enhet.

**Obs!** Det kan ta upp till 24 timmar innan rapporteringsdata för baslinjer visas från den första distributionen till en enhet och upp till 6 timmar för ytterligare uppdateringar. 

Den vanligaste orsaken till att en baslinjeinställning inte används är att samma inställning används i en annan profil. Det här scenariot kan undersökas för specifika enheter genom att välja enheten i noden Enhetsstatus i profilen Säkerhetsbaslinje. Mer information finns i [Lösa konflikter för säkerhetsbaslinjer](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).