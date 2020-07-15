---
title: Problem med onboarding-maskiner
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141837"
---
# <a name="issues-with-onboarding-machines"></a>Problem med onboarding-maskiner

Du kan ha problem med introduktionsdatorer till MDATP-tjänsten. Om du kan komma åt slutanvändarens dator gör du så här:

1. Hämta diagnostikverktyget [För klientanslutningsanalysator.](https://aka.ms/mdatpanalyzer)
2. Extrahera och kör MDATPAnalyzer.cmd.
3. Leta upp diagnostikloggen i mappen MDATPClientAnalyzerResult, samma mapp där analysverktyget hämtas.
4. Granska loggfilen, MDATPClientAnalyzer.txt, för att hitta problem med anslutnings- eller internetproxyinställningar.