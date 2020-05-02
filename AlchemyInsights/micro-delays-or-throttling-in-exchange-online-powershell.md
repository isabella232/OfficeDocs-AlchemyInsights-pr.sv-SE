---
title: Mikrofördröjningar eller begränsningar i Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/30/2020
ms.locfileid: "43948029"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrofördröjningar eller begränsningar i Exchange Online PowerShell

Du kanske får varningar om att mikrofördröjning tillämpats (”Micro delay applied”) eller upplever fördröjningar när du kör skript och cmdlets i Exchange Online. Här är två förslag gällande detta:

- Du kan prova att använda [Exchange Online v2 PowerShell-modulen](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), som innehåller CMDlets som baseras på REST API och har mycket bättre prestanda. Det här kan vara en bra lösning för många Get- CMDlets som används ofta.
- Om du behöver använda CMDlets som inte finns med i v2-modulen än läser du om hur du [kör PowerShell-cmdlets för ett stort antal användare i Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#). Den här artikeln innehåller information om hur du kringgår förväntade PowerShell-begränsningar i Exchange Online.
