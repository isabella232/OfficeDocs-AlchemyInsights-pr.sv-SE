---
title: Fjärrkorrigering av problem med onboarding Windows 10-enheter till Microsoft Defender Advanced Threat Protection
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 44969436c99b182cb4202fa60e2deb7d6ea3f460e48ee4649de1cfb646970f34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034052"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Fjärrkorrigering av problem med onboarding Windows 10-enheter till Microsoft Defender Advanced Threat Protection

Om du kan komma åt fjärrdatorn gör du så här:

1. Ladda ned [diagnostikverktyget För klientanslutning.](https://go.microsoft.com/fwlink/?linkid=2143466)
2. Extrahera och kör MDATPAnalyzer.cmd.
3. Leta reda på diagnostikloggen i mappen MDATPClientAnalyzerResult, som är samma mapp där Analysverktyget laddades ned.
4. Om du vill hitta problem med anslutnings- eller proxyinställningar för Internet granskar du MDATPClientAnalyzer.txt.

Mer information finns i [Problem med onboarding-datorer.](https://go.microsoft.com/fwlink/?linkid=2143634)
