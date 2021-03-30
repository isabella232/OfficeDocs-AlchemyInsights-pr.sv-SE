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
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Konfigurera sekretessinställningar i Microsoft Edge

Om Microsoft Edge är distribuerat på andra plattformar än Windows skickas som standard inte diagnostikdata och webbplatsinformation till Microsoft. Men om Microsoft Edge distribueras i Windows 10 skickas diagnostikdata och webbplatsinformation enligt användarnas inställningar för [Windows-diagnostikdata.](https://go.microsoft.com/fwlink/?linkid=2132472)

Om du vill konfigurera hur Microsoft Edge hanterar datainsamling för din organisation använder du följande grupprinciper:
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) aktiverar rapportering av användning och kraschrelaterade data.
- [SendSiteInfoToImproveServices skickar](https://go.microsoft.com/fwlink/?linkid=2132470) webbplatsinformation som används för att förbättra Microsofts tjänster.

Mer information finns i [Konfigurera principinställningar](https://go.microsoft.com/fwlink/?linkid=2132577).
