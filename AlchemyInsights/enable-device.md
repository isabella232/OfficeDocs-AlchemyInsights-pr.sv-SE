---
title: Aktivera enhet
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256986"
---
# <a name="enable-device"></a>Aktivera enhet

**Så här aktiverar du enheten med powershell-kommandot**

Kör följande kommandon:

- Så här hämtar du enhetsobjekt: `Get-MsolDevice -Name <Name>`
- Så här aktiverar du enhet: `Enable-MsolDevice -DeviceId <DeviceId>`

Mer information om hur du konfigurerar hybridkoppling på hanterade domäner finns i [Konfigurera hybridkoppling.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
