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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830051"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrofördröjningar eller begränsningar i Exchange Online PowerShell

Du kanske får varningar om att mikrofördröjning tillämpats (”Micro delay applied”) eller upplever fördröjningar när du kör skript och cmdlets i Exchange Online. Här är två förslag gällande detta:

- Du kan prova att använda [Exchange Online v2 PowerShell-modulen](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), som innehåller CMDlets som baseras på REST API och har mycket bättre prestanda. Det här kan vara en bra lösning för många Get- CMDlets som används ofta.
- Om du behöver använda CMDlets som inte finns med i v2-modulen än läser du om hur du [kör PowerShell-cmdlets för ett stort antal användare i Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#). Den här artikeln innehåller information om hur du kringgår förväntade PowerShell-begränsningar i Exchange Online.
