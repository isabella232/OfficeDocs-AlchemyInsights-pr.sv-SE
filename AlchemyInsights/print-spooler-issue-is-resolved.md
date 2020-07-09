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
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="b126a-102">Problemet med utskriftshanteraren är löst</span><span class="sxs-lookup"><span data-stu-id="b126a-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="b126a-103">Om enheten uppdaterades med Windows 10 **OS Build 19041.329**kan du ha observerat ett problem där vissa skrivare inte skrivs ut.</span><span class="sxs-lookup"><span data-stu-id="b126a-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="b126a-104">Utskriftshanteraren kan utlösa ett fel eller stängas oväntat när du försöker skriva ut, och ingen utdata kommer från den berörda skrivaren.</span><span class="sxs-lookup"><span data-stu-id="b126a-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="b126a-105">Det här problemet är löst i OS Build **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="b126a-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="b126a-106">**Pågående utredning**</span><span class="sxs-lookup"><span data-stu-id="b126a-106">**Ongoing investigation**</span></span>

<span data-ttu-id="b126a-107">LSASS-filen (Local Security Authority Subsystem Service)\*\* (Isass.exe) \*\*kan misslyckas på vissa enheter med felmeddelandet "En kritisk systemprocess, C:\WINDOWS\system32\Isass.exe, misslyckades med statuskoden c0000008.</span><span class="sxs-lookup"><span data-stu-id="b126a-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="b126a-108">Maskinen måste nu startas om".</span><span class="sxs-lookup"><span data-stu-id="b126a-108">The machine must now be restarted".</span></span>  <span data-ttu-id="b126a-109">**Microsoft arbetar på en lösning och kommer att tillhandahålla en uppdatering i en kommande version.**</span><span class="sxs-lookup"><span data-stu-id="b126a-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="b126a-110">Mer information finns i kända problem med [Windows 10 Version 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="b126a-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>