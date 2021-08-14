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
ms.openlocfilehash: cb97aa790264c23aae15fed49c353c7fb0d6209d9492c6881f1b1091fe80d7b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868552"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrofördröjningar eller begränsningar i Exchange Online PowerShell

Du kanske får varningar om att mikrofördröjning tillämpats (”Micro delay applied”) eller upplever fördröjningar när du kör skript och cmdlets i Exchange Online. Här är några förslag på hur du löser det:

- Kör vår diagnostik för att slappna av klientorganisationens PowerShell-begränsningsprinciper. Den här lösningen löser problemet för det mesta.
- Om problemet ändå inte går att lösa använder du [Exchange Online v2 PowerShell-modulen](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), som innehåller CMDlets som är baserade på REST API och som är betydligt mer performant. Det här kan vara en bra lösning för många Get- CMDlets som används ofta.
- Om du behöver använda CMDlets som inte ingår i v2-modulen kan du läsa Köra [PowerShell-cmdlets](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)för många användare i Office 365 , som handlar om hur du kommer runt begränsningsgränser för PowerShell i Exchange Online.
