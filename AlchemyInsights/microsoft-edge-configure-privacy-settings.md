---
title: Konfigurera sekretess inställningar för Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678861"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="4c382-102">Konfigurera sekretess inställningar för Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="4c382-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="4c382-103">Om Microsoft Edge distribueras på icke-Windows-plattformar skickas inte diagnostikdata och webbplatsinformation till Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4c382-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="4c382-104">Men om Microsoft Edge distribueras på Windows 10 skickas diagnostikdata och webbplatsinformation enligt användarnas [Windows-inställningar för diagnostikdata](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="4c382-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="4c382-105">Använd följande grup principer för att konfigurera hur Microsoft Edge hanterar data insamling för din organisation:</span><span class="sxs-lookup"><span data-stu-id="4c382-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="4c382-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): den här principen möjliggör rapportering av användning och kraschbaserade data.</span><span class="sxs-lookup"><span data-stu-id="4c382-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="4c382-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): den här principen skickar webbplatsinformation som används för att förbättra Microsoft-tjänsterna.</span><span class="sxs-lookup"><span data-stu-id="4c382-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="4c382-108">Mer information finns i [Konfigurera princip inställningar](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="4c382-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>