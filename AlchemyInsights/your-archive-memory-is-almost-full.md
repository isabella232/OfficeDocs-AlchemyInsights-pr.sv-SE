---
title: Din arkivpostlåda är nästan full
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046770"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Din arkivpostlåda är nästan full

Om användaren får varningen **Din arkivpostlåda är nästan full**, eller du behöver öka storleken på arkivpostlådan. Här är några tips:

1. Om användaren har tilldelats en licens Exchange Online abonnemang 1 ska du uppgradera till en licens Exchange Online abonnemang **2** för att öka storleken från 50 GB till 100 GB.
1. Om användaren redan har tilldelats något av följande: Exchange Online abonnemang **2** eller ett Exchange Online abonnemang 1 med ett Exchange Online - arkivering-tillägg aktiverar du automatisk expansion arkivering:
 
    1. [Anslut till Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Kör följande kommandolet för användaren:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Kör följande kommandolet för att bekräfta att det är aktiverat för användaren:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Mer information finns i:

- [Aktivera obegränsad arkivering – hjälp för administratörer – Microsoft 365 och | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online – Tjänstbeskrivningar | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Uppgradera till ett annat företagsabonnemang | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

