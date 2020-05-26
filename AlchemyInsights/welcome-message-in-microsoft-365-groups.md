---
title: Välkomstmeddelande i Microsoft 365-grupper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358336"
---
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="24da9-102">Välkomstmeddelande i Microsoft 365-grupper</span><span class="sxs-lookup"><span data-stu-id="24da9-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="24da9-103">Nya användare som går med i Microsoft 365-gruppen får välkomstmeddelande om egenskapen "UnifiedGroupWelcomeMessageEnabled" är sann.</span><span class="sxs-lookup"><span data-stu-id="24da9-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="24da9-104">Om du vill inaktivera välkomstmeddelandet använder du följande [EXO PowerShell-kommando:](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="24da9-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
