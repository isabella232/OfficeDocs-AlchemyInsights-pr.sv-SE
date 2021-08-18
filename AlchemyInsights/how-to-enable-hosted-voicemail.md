---
title: Så här aktiverar du Värd för röstmeddelanden
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318666"
---
# <a name="how-to-enable-hosted-voicemail"></a>Så här aktiverar du Värd för röstmeddelanden

För att kunna aktivera **röstmeddelanden måste HostedVoicemail** vara inställt på $true.

Egenskapen **HostedVoicemail** för användaren som använder Remote PowerShell (RPS).

Mer information om hur du ansluter till RPS finns i [Microsoft Teams PowerShell-översikt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) för mer information om hur du ansluter till RPS.

1. Administratören Teams vara inloggad på Remote PowerShell för Teams.
1. Från PowerShell-kommandotolken kan Teams-administratör köra **set-csuser user@contoso.com -HostedVoiceMail $true** där sip uri är för den användaren i fråga.

**Obs!** Det kan ta upp till 24 timmar innan ändringar av principer replikeras.