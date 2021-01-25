---
title: Arkiv post lådan är nästan full
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974665"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="c2def-102">Arkiv post lådan är nästan full</span><span class="sxs-lookup"><span data-stu-id="c2def-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="c2def-103">Om användaren får varningen **Arkiv post lådan är nästan full**, eller så måste du öka storleken på deras Arkiv post låda:</span><span class="sxs-lookup"><span data-stu-id="c2def-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="c2def-104">Om användaren har tilldelats en Exchange Online-prenumeration 1 kan du uppgradera till **Exchange Online abonnemang 2** -licens för att öka storleken från 50 GB till 1 GB.</span><span class="sxs-lookup"><span data-stu-id="c2def-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="c2def-105">Om användaren redan har tilldelats något av följande: **Exchange Online-abonnemang 2** eller en Exchange Online-prenumeration 1 med ett tillägg för Exchange Online-arkivering och Använd stegen nedan för att aktivera automatisk utökande arkivering:.</span><span class="sxs-lookup"><span data-stu-id="c2def-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="c2def-106">[Anslut till Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="c2def-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="c2def-107">Kör följande cmdleten för användaren:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="c2def-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="c2def-108">Kör följande cmdleten för att bekräfta att den är aktive rad för användaren:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="c2def-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="c2def-109">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="c2def-109">For more information see:</span></span>

- [<span data-ttu-id="c2def-110"> Aktivera obegränsad arkivering – hjälp för administratörer – Microsoft 365-efterlevnad | Microsoft-dok</span><span class="sxs-lookup"><span data-stu-id="c2def-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="c2def-111">Begränsningar för Exchange Online-beskrivningar | Microsoft-dok</span><span class="sxs-lookup"><span data-stu-id="c2def-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="c2def-112">Uppgradera till en annan företags plan | Microsoft-dok</span><span class="sxs-lookup"><span data-stu-id="c2def-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

