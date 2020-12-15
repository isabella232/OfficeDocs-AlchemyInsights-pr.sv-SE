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
# <a name="microsoft-edge-configure-privacy-settings"></a>Konfigurera sekretess inställningar för Microsoft Edge

Om Microsoft Edge distribueras på icke-Windows-plattformar skickas inte diagnostikdata och webbplatsinformation till Microsoft. Men om Microsoft Edge distribueras på Windows 10 skickas diagnostikdata och webbplatsinformation enligt användarnas [Windows-inställningar för diagnostikdata](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).

Använd följande grup principer för att konfigurera hur Microsoft Edge hanterar data insamling för din organisation:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): den här principen möjliggör rapportering av användning och kraschbaserade data.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): den här principen skickar webbplatsinformation som används för att förbättra Microsoft-tjänsterna.

Mer information finns i [Konfigurera princip inställningar](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).