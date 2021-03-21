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
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="13b72-102">Problem med registreringsdatorer till Microsoft Defender for Endpoint</span><span class="sxs-lookup"><span data-stu-id="13b72-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="13b72-103">Du kan ha problem med registreringsdatorer till MDE-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="13b72-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="13b72-104">Om du kan komma åt slutanvändarens dator gör du följande:</span><span class="sxs-lookup"><span data-stu-id="13b72-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="13b72-105">Ladda ned den senaste förhandsversionen av diagnostikverktyget [MDE Client Analyzer](https://aka.ms/betamdeanalyzer).</span><span class="sxs-lookup"><span data-stu-id="13b72-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="13b72-106">Högerklicka på **MDEClientAnalyzer.cmd** och välj Kör som administratör.</span><span class="sxs-lookup"><span data-stu-id="13b72-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="13b72-107">Följ de riktlinjer som föreslås i **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="13b72-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="13b72-108">Mer utförliga loggar finns i den skapade undermappen med namnet **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="13b72-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="13b72-109">Om det krävs ytterligare vägledning kontaktar du [Microsoft Defender for Endpoint-support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) och tillhandahåller den resulterande MDEClientAnalyzerResult.zip-filen för analys.</span><span class="sxs-lookup"><span data-stu-id="13b72-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
