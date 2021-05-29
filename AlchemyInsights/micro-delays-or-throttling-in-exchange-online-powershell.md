---
title: Mikrofördröjningar eller begränsningar i Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702144"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="3c6ed-102">Mikrofördröjningar eller begränsningar i Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="3c6ed-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="3c6ed-103">Du kanske får varningar om att mikrofördröjning tillämpats (”Micro delay applied”) eller upplever fördröjningar när du kör skript och cmdlets i Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="3c6ed-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="3c6ed-104">Här är några förslag på hur du löser det:</span><span class="sxs-lookup"><span data-stu-id="3c6ed-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="3c6ed-105">Kör vår diagnostik för att slappna av klientorganisationens PowerShell-begränsningsprinciper.</span><span class="sxs-lookup"><span data-stu-id="3c6ed-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="3c6ed-106">Den här lösningen löser problemet för det mesta.</span><span class="sxs-lookup"><span data-stu-id="3c6ed-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="3c6ed-107">Om problemet ändå inte går att lösa använder du [Exchange Online v2 PowerShell-modulen](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), som innehåller CMDlets som är baserade på REST API och som är betydligt mer performant.</span><span class="sxs-lookup"><span data-stu-id="3c6ed-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="3c6ed-108">Det här kan vara en bra lösning för många Get- CMDlets som används ofta.</span><span class="sxs-lookup"><span data-stu-id="3c6ed-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="3c6ed-109">Om du behöver använda CMDlets som inte ingår i v2-modulen kan du läsa Köra [PowerShell-cmdlets](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)för många användare i Office 365 , som handlar om hur du kommer runt begränsningsgränser för PowerShell i Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="3c6ed-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
