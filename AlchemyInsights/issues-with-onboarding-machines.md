---
title: Problem med registreringsdatorer till Microsoft Defender for Endpoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901585"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a>Problem med registreringsdatorer till Microsoft Defender for Endpoint

Du kan ha problem med registreringsdatorer till MDE-tjänsten. Om du kan komma åt slutanvändarens dator gör du följande:

1. Ladda ned den senaste förhandsversionen av diagnostikverktyget [MDE Client Analyzer](https://aka.ms/betamdeanalyzer).
2. Högerklicka på **MDEClientAnalyzer.cmd** och välj Kör som administratör.
3. Följ de riktlinjer som föreslås i **MDEClientAnalyzer.htm**.
4. Mer utförliga loggar finns i den skapade undermappen med namnet **MDEClientAnalyzerResult**.
5. Om det krävs ytterligare vägledning kontaktar du [Microsoft Defender for Endpoint-support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) och tillhandahåller den resulterande MDEClientAnalyzerResult.zip-filen för analys.
