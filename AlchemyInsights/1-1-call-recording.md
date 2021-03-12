---
title: Inspelning av 1:1-samtal
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733867"
---
# <a name="11-call-recording"></a>Inspelning av 1:1-samtal

Administratörer måste vidta åtgärder nu för att fortsätta tillåta användare att spela in 1:1-samtal.
 
Från och med den 12 april 2021 börjar vi framtvinga ett nytt samtalsprincipalternativ för Teams *AllowCloudRecordingForCalls.* 

Funktionerna för inspelning av 1:1-samtal kontrolleras av *alternativet AllowCloudRecording* i Teams mötespolicy. Om användarna tillåts spela in Teams-möten kan de även spela in 1:1-samtal.

Om du föredrar att blockera alla användare från att spela in 1:1-samtal behöver du inte vidta någon åtgärd. *Policyalternativet AllowCloudRecordingForCalls* är $False alternativ som standard.

Den här ändringen beskrivs i följande meddelandecenterinlägg: [(Uppdaterad) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) introduktion till policyn för samtalsinspelning Om du vill ställa in policyalternativet för Teams måste du använda [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)

**Så här aktiverar du samtalsinspelning i 1:1-samtal:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

**Så här inaktiverar du samtalsinspelning i 1:1-samtal:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

