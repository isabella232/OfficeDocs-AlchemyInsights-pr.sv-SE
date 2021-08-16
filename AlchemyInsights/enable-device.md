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
ms.openlocfilehash: 4722ccf6847fc6c02616dbc62d59a2a87c089f77ae79c0a916211af6c5f2a6d0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003510"
---
# <a name="enable-device"></a>Aktivera enhet

**Så här aktiverar du enheten med PowerShell-kommandot**

Kör följande kommandon:

- Så här hämtar du enhetsobjekt: `Get-MsolDevice -Name <Name>`
- Så här aktiverar du enheten: `Enable-MsolDevice -DeviceId <DeviceId>`

Mer information om hur du konfigurerar hybridkoppling för hanterade domäner finns i [Konfigurera hybridkoppling.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
