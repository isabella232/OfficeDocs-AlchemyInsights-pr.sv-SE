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
# <a name="your-archive-mailbox-is-almost-full"></a>Arkiv post lådan är nästan full

Om användaren får varningen **Arkiv post lådan är nästan full**, eller så måste du öka storleken på deras Arkiv post låda:

1. Om användaren har tilldelats en Exchange Online-prenumeration 1 kan du uppgradera till **Exchange Online abonnemang 2** -licens för att öka storleken från 50 GB till 1 GB.
1. Om användaren redan har tilldelats något av följande: **Exchange Online-abonnemang 2** eller en Exchange Online-prenumeration 1 med ett tillägg för Exchange Online-arkivering och Använd stegen nedan för att aktivera automatisk utökande arkivering:.
 
    1. [Anslut till Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Kör följande cmdleten för användaren:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Kör följande cmdleten för att bekräfta att den är aktive rad för användaren:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Mer information finns i:

- [ Aktivera obegränsad arkivering – hjälp för administratörer – Microsoft 365-efterlevnad | Microsoft-dok](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Begränsningar för Exchange Online-beskrivningar | Microsoft-dok](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Uppgradera till en annan företags plan | Microsoft-dok](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

