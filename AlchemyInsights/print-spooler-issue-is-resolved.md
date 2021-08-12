---
title: Problem med utskriftshanteraren har lösts
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911356"
---
# <a name="print-spooler-issue-is-resolved"></a>Problem med utskriftshanteraren har lösts

Om enheten uppdaterades med Windows 10 **OS version 19041.329** kan du ha observerat ett problem där vissa skrivare inte kan skrivas ut.   Utskriftshanteraren kan ge ett fel eller stängas oväntat vid försök att skriva ut och inga utdata kommer från den aktuella skrivaren. Det här problemet är löst i **OS-version 19041.331**, [KB4567523.](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)  

**Pågående undersökning**

LSASS-filen (Local Security Authority Subsystem Service) (**Isass.exe**) kan misslyckas på vissa enheter med felmeddelandet "En kritisk systemprocess, C:\WINDOWS\system32\Isass.exe, misslyckades med statuskoden c0000008. Nu måste datorn startas om."  **Microsoft arbetar på en lösning och kommer att tillhandahålla en uppdatering i en kommande version.**

Mer information finns i Windows 10 [version 2004.](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)