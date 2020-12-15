---
title: Så här aktiverar du röst brev låda
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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679164"
---
# <a name="how-to-enable-hosted-voicemail"></a>Så här aktiverar du röst brev låda

För att aktivera röst brev låda måste **HostedVoicemail** vara inställt på $True.

Egenskapen **HostedVoicemail** för användaren med Remote POWERSHELL (RPS).

Mer information om hur du ansluter till RPS finns i [Microsoft Teams PowerShell-översikten](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) för att få mer information om hur du ansluter till RPS.

1. Teams-administratören bör vara inloggad i fjärr-PowerShell för Teams.
1. Från PowerShell uppmana team administratören att köra **set-csuser user@contoso.com-HostedVoiceMail $True** där SIP URI är av en användare.

> [!NOTE]
> Ändringar i policyn kan ta upp till 24 timmar att replikera.