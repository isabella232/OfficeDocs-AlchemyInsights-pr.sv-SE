---
title: Kalender behörigheter
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748811"
---
# <a name="calendar-permissions"></a>Kalender behörigheter

Användare kan ändra sina egna kalender behörigheter med Outlook på webben eller andra klienter, men som administratör kan du även behöva undersöka det.  
Med Exchange PowerShell cmdlet kan du Visa behörigheten för en användares kalender:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Mer information finns i:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalender behörigheter används för att dela kalendrar, för att få mer information om att dela en Outlook-kalender, se dessa artiklar:

- [Dela en Outlook-kalender med andra](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Dela din kalender i Outlook på webben för företag](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Om du vill felsöka kalender behörighet kan du använda verktyget för [support och återställning](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .