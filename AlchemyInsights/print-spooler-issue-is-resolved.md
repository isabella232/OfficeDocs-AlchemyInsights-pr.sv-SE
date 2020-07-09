---
title: Problemet med utskriftshanteraren är löst
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088409"
---
# <a name="print-spooler-issue-is-resolved"></a>Problemet med utskriftshanteraren är löst

Om enheten uppdaterades med Windows 10 **OS Build 19041.329**kan du ha observerat ett problem där vissa skrivare inte skrivs ut. Utskriftshanteraren kan utlösa ett fel eller stängas oväntat när du försöker skriva ut, och ingen utdata kommer från den berörda skrivaren. Det här problemet är löst i OS Build **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Pågående utredning**

LSASS-filen (Local Security Authority Subsystem Service)** (Isass.exe) **kan misslyckas på vissa enheter med felmeddelandet "En kritisk systemprocess, C:\WINDOWS\system32\Isass.exe, misslyckades med statuskoden c0000008. Maskinen måste nu startas om".  **Microsoft arbetar på en lösning och kommer att tillhandahålla en uppdatering i en kommande version.**

Mer information finns i kända problem med [Windows 10 Version 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).