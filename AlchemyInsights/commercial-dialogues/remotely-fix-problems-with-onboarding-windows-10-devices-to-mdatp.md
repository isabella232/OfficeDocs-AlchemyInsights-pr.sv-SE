---
title: Fjärrstyrt åtgärda problem med att registrera Windows 10-enheter i Microsoft Defender Avancerat skydd
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750044"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="e0972-102">Fjärrstyrt åtgärda problem med att registrera Windows 10-enheter i Microsoft Defender Avancerat skydd</span><span class="sxs-lookup"><span data-stu-id="e0972-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="e0972-103">Om du kan komma åt fjärrdatorn gör du så här:</span><span class="sxs-lookup"><span data-stu-id="e0972-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="e0972-104">Ladda ned [diagnostikverktyget För klientanslutning.](https://go.microsoft.com/fwlink/?linkid=2143466)</span><span class="sxs-lookup"><span data-stu-id="e0972-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="e0972-105">Extrahera och kör MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="e0972-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="e0972-106">Leta reda på diagnostikloggen i mappen MDATPClientAnalyzerResult, som är samma mapp där Analysverktyget laddades ned.</span><span class="sxs-lookup"><span data-stu-id="e0972-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="e0972-107">Om du vill hitta problem med anslutnings- eller proxyinställningar för Internet granskar du MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="e0972-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="e0972-108">Mer information finns i [Problem med onboarding-datorer.](https://go.microsoft.com/fwlink/?linkid=2143634)</span><span class="sxs-lookup"><span data-stu-id="e0972-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
