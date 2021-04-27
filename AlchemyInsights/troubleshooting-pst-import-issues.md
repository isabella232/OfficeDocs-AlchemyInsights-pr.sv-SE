---
title: Felsöka problem med PST-import
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
- "1800027"
- "1225"
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059833"
---
# <a name="troubleshooting-pst-import-issues"></a>Felsöka problem med PST-import

- Om du importerar inom Outlook-klienten kan du gå till [Åtgärda problem med att importera en Outlook.pst-fil.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Om du använder importtjänsten och den har fastnat bör du observera att varje PST-fil som du laddar upp till Azure Storage-platsen inte ska vara större än 20 GB. PST-filer som är större än 20 GB kan påverka prestandan för PST-importen. Mer information om felsökning av jobb som fastnat finns i [Problem som påverkar PST-importjobb.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

- Om du vill verifiera statusen för ett visst importjobb använder du [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Fullständig information om importtjänsten finns i [Översikt över hur du importerar organisationens PST-filer.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
