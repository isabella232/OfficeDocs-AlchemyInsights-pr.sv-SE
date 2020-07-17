---
title: Meddelanden som skickas till Microsoft 365-gruppen tas inte emot av alla medlemmar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/06/2020
ms.locfileid: "45051518"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="9405a-102">Meddelanden som skickas till en Microsoft 365-grupp tas inte emot av alla medlemmar</span><span class="sxs-lookup"><span data-stu-id="9405a-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="9405a-103">Se till att alla gruppmedlemmar prenumererar på att ta emot e-postmeddelandena.</span><span class="sxs-lookup"><span data-stu-id="9405a-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="9405a-104">Se [Följ en grupp i Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="9405a-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="9405a-105">Om du vill kontrollera meddelandestatus för medlemmar som prenumererar på gruppmeddelanden kör du följande kommando på [EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="9405a-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`