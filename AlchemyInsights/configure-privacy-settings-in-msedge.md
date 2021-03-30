---
title: Konfigurera sekretessinställningar i Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405731"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="b649a-102">Konfigurera sekretessinställningar i Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b649a-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="b649a-103">Om Microsoft Edge är distribuerat på andra plattformar än Windows skickas som standard inte diagnostikdata och webbplatsinformation till Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b649a-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="b649a-104">Men om Microsoft Edge distribueras i Windows 10 skickas diagnostikdata och webbplatsinformation enligt användarnas inställningar för [Windows-diagnostikdata.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="b649a-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="b649a-105">Om du vill konfigurera hur Microsoft Edge hanterar datainsamling för din organisation använder du följande grupprinciper:</span><span class="sxs-lookup"><span data-stu-id="b649a-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="b649a-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) aktiverar rapportering av användning och kraschrelaterade data.</span><span class="sxs-lookup"><span data-stu-id="b649a-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="b649a-107">[SendSiteInfoToImproveServices skickar](https://go.microsoft.com/fwlink/?linkid=2132470) webbplatsinformation som används för att förbättra Microsofts tjänster.</span><span class="sxs-lookup"><span data-stu-id="b649a-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="b649a-108">Mer information finns i [Konfigurera principinställningar](https://go.microsoft.com/fwlink/?linkid=2132577).</span><span class="sxs-lookup"><span data-stu-id="b649a-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
