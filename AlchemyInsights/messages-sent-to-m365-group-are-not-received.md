---
title: Meddelanden skickade till Microsoft 365-grupp har inte mottagits av alla medlemmar
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 29adc5a7b8b74280cb3fcd6369dc4fc3a3e8e957
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823805"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Meddelanden skickade till en Microsoft 365-grupp har inte mottagits av alla medlemmar

Säkerställ att alla gruppmedlemmar prenumererar på dessa e-postmeddelanden. Läs [Följ en grupp i Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36) för mer information.  

För att kontrollera meddelandestatus på medlemmar som prenumererar på grupp-e-postmeddelanden kan du köra följande kommande på [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Använd följande kommando i EXO PowerShell för att konfigurera att alla gruppmedlemmar får e-postmeddelanden skickade till Microsoft 365-gruppen:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Till exempel:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`