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
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="7578c-102">Problem med onboarding-maskiner</span><span class="sxs-lookup"><span data-stu-id="7578c-102">Issues with onboarding machines</span></span>

<span data-ttu-id="7578c-103">Du kan ha problem med introduktionsdatorer till MDATP-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="7578c-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="7578c-104">Om du kan komma åt slutanvändarens dator gör du så här:</span><span class="sxs-lookup"><span data-stu-id="7578c-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="7578c-105">Hämta diagnostikverktyget [För klientanslutningsanalysator.](https://aka.ms/mdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="7578c-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="7578c-106">Extrahera och kör MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="7578c-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="7578c-107">Leta upp diagnostikloggen i mappen MDATPClientAnalyzerResult, samma mapp där analysverktyget hämtas.</span><span class="sxs-lookup"><span data-stu-id="7578c-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="7578c-108">Granska loggfilen, MDATPClientAnalyzer.txt, för att hitta problem med anslutnings- eller internetproxyinställningar.</span><span class="sxs-lookup"><span data-stu-id="7578c-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>