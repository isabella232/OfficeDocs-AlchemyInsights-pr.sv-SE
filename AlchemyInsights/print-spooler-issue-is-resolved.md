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
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="c8bca-102">Problem med utskrifts hanteraren är löst</span><span class="sxs-lookup"><span data-stu-id="c8bca-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="c8bca-103">Om enheten har uppdaterats med Windows 10  **OS version 19041,329**kanske du har iakttagit ett problem där vissa skrivare inte kan skriva ut.</span><span class="sxs-lookup"><span data-stu-id="c8bca-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="c8bca-104">Utskrifts hanteraren kan utlösa fel eller avsluta oväntat när du försöker skriva ut, och ingen utskrift kommer från den aktuella skrivaren.</span><span class="sxs-lookup"><span data-stu-id="c8bca-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="c8bca-105">Det här problemet löses i OS version  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="c8bca-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="c8bca-106">**Pågående undersökning**</span><span class="sxs-lookup"><span data-stu-id="c8bca-106">**Ongoing investigation**</span></span>

<span data-ttu-id="c8bca-107">Den lokala LSASS-filen (Subsystem File System) (**Isass.exe**) kanske inte fungerar på vissa enheter med fel meddelandet "en kritisk system process, C:\WINDOWS\system32\Isass.exe, misslyckades med status kod c0000008.</span><span class="sxs-lookup"><span data-stu-id="c8bca-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="c8bca-108">Datorn måste nu startas om.</span><span class="sxs-lookup"><span data-stu-id="c8bca-108">The machine must now be restarted".</span></span>  <span data-ttu-id="c8bca-109">**Microsoft jobbar med en lösning och tillhandahåller en uppdatering i en kommande version.**</span><span class="sxs-lookup"><span data-stu-id="c8bca-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="c8bca-110">Mer information finns i  [Windows 10 Version 2004 kända problem](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="c8bca-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>