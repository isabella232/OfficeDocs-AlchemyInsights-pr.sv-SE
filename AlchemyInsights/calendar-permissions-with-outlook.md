---
title: Kalenderbehörigheter
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819926"
---
# <a name="calendar-permissions"></a>Kalenderbehörigheter

Användare kan ändra sina egna kalenderbehörigheter med Outlook på webben eller andra klienter, men som administratör kan du behöva undersöka också.  
Med Exchange PowerShell-cmdleten får du behörighet för en användares kalender:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Mer information finns i följande avsnitt:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalenderbehörigheter används vid delning av kalendrar. Mer information om hur du delar en Outlook-kalender finns i följande artiklar:

- [Dela en Outlook-kalender med andra](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Dela din kalender i Outlook på webben för företag](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Om du vill felsöka kalenderbehörighet kan du använda [verktyget Support- och återställningsassistenten.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)