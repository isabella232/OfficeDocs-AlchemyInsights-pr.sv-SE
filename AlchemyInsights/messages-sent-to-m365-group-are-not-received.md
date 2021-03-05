---
title: Meddelanden skickade till Microsoft 365-grupp har inte mottagits av alla medlemmar
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 080c060f5675065704c7209bd15e4cbb1236b8db
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480701"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="73442-102">Meddelanden skickade till en Microsoft 365-grupp har inte mottagits av alla medlemmar</span><span class="sxs-lookup"><span data-stu-id="73442-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="73442-103">Säkerställ att alla gruppmedlemmar prenumererar på dessa e-postmeddelanden.</span><span class="sxs-lookup"><span data-stu-id="73442-103">Ensure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="73442-104">Läs [Följ en grupp i Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36) för mer information.</span><span class="sxs-lookup"><span data-stu-id="73442-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="73442-105">För att kontrollera meddelandestatus på medlemmar som prenumererar på grupp-e-postmeddelanden kan du köra följande kommande på [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span><span class="sxs-lookup"><span data-stu-id="73442-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

<span data-ttu-id="73442-106">Använd följande kommando i EXO PowerShell för att konfigurera att alla gruppmedlemmar får e-postmeddelanden skickade till Microsoft 365-gruppen:</span><span class="sxs-lookup"><span data-stu-id="73442-106">Use the following EXO PowerShell command to configure all group members to receive emails sent to Microsoft 365 group in their inbox:</span></span>

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

<span data-ttu-id="73442-107">Till exempel:</span><span class="sxs-lookup"><span data-stu-id="73442-107">For example:</span></span>

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`