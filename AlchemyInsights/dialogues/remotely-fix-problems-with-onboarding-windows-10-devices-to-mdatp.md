---
title: Fjärrstyrt åtgärda problem med att registrera Windows 10-enheter i Microsoft Defender Advanced Threat Protection
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694844"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Fjärrstyrt åtgärda problem med att registrera Windows 10-enheter till Microsoft Defender Advanced Threat Protection

Om du kan komma åt fjärrdatorn gör du så här:

1. Ladda ned [diagnostikverktyget För klientanslutningsanalys.](https://go.microsoft.com/fwlink/?linkid=2143466)
2. Extrahera och kör MDATPAnalyzer.cmd.
3. Leta reda på diagnostikloggen i mappen MDATPClientAnalyzerResult, som är samma mapp där Analysverktyget laddades ned.
4. Om du vill hitta problem med anslutnings- eller proxyinställningar för Internet granskar du loggfilen MDATPClientAnalyzer.txt.

Mer information finns i [Problem med onboarding-datorer.](https://go.microsoft.com/fwlink/?linkid=2143634)
