---
title: Felsökning av importtjänstjobb som fastnat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125495"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="41257-102">Felsökning av importtjänstjobb som fastnat</span><span class="sxs-lookup"><span data-stu-id="41257-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="41257-103">Om du har problem med att importtjänstjobb har fastnat eller misslyckats kan du undersöka och prova följande:</span><span class="sxs-lookup"><span data-stu-id="41257-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="41257-104">Kontrollera storleken på PST-filen.</span><span class="sxs-lookup"><span data-stu-id="41257-104">Review the size of of the PST file.</span></span> <span data-ttu-id="41257-105">Den rekommenderade storleken på en PST-fil för import är högst 20 GB.</span><span class="sxs-lookup"><span data-stu-id="41257-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="41257-106">Om du misstänker att objekten hoppats över på grund av skadade objekt kör du Scanpst.exe diagnostisera och åtgärda fel i PST-filer.</span><span class="sxs-lookup"><span data-stu-id="41257-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="41257-107">Om du ser felet "MapiExceptionShutoffQuotaExceeded" under importen kontrollerar du att målpostlådan har tillräcklig kapacitet för att importera önskade PST-filer.</span><span class="sxs-lookup"><span data-stu-id="41257-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="41257-108">Mer information om felsökning av problem med PST-importjobb finns [i Felsöka problem med PST-importjobb.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="41257-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="41257-109">Mer information om hur du åtgärdar problem när du importerar PSTs till Outlook finns i Åtgärda problem med att [importera en PST-Outlook (microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)</span><span class="sxs-lookup"><span data-stu-id="41257-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>