---
title: Problem med utskrifts hanteraren är löst
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
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801859"
---
# <a name="print-spooler-issue-is-resolved"></a>Problem med utskrifts hanteraren är löst

Om enheten har uppdaterats med Windows 10  **OS version 19041,329**kanske du har iakttagit ett problem där vissa skrivare inte kan skriva ut. Utskrifts hanteraren kan utlösa fel eller avsluta oväntat när du försöker skriva ut, och ingen utskrift kommer från den aktuella skrivaren. Det här problemet löses i OS version  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Pågående undersökning**

Den lokala LSASS-filen (Subsystem File System) (**Isass.exe**) kanske inte fungerar på vissa enheter med fel meddelandet "en kritisk system process, C:\WINDOWS\system32\Isass.exe, misslyckades med status kod c0000008. Datorn måste nu startas om.  **Microsoft jobbar med en lösning och tillhandahåller en uppdatering i en kommande version.**

Mer information finns i  [Windows 10 Version 2004 kända problem](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).