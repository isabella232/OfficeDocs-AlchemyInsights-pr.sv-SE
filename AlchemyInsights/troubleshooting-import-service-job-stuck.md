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
# <a name="troubleshooting-import-service-job-stuck"></a>Felsökning av importtjänstjobb som fastnat

Om du har problem med att importtjänstjobb har fastnat eller misslyckats kan du undersöka och prova följande:

- Kontrollera storleken på PST-filen. Den rekommenderade storleken på en PST-fil för import är högst 20 GB.

- Om du misstänker att objekten hoppats över på grund av skadade objekt kör du Scanpst.exe diagnostisera och åtgärda fel i PST-filer.

- Om du ser felet "MapiExceptionShutoffQuotaExceeded" under importen kontrollerar du att målpostlådan har tillräcklig kapacitet för att importera önskade PST-filer.

Mer information om felsökning av problem med PST-importjobb finns [i Felsöka problem med PST-importjobb.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

Mer information om hur du åtgärdar problem när du importerar PSTs till Outlook finns i Åtgärda problem med att [importera en PST-Outlook (microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)