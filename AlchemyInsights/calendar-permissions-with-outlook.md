---
title: Kalenderbehörigheter
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862166"
---
# <a name="calendar-permissions"></a>Kalenderbehörigheter

Användare kan ändra sina egna kalenderbehörigheter med Outlook på webben eller andra klienter, men som administratör kan du också behöva undersöka.  
Med Exchange PowerShell cmdlet visar du behörigheten för en användares kalender:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Så här ser du mer information:

- [Hämta-mailboxfolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-mailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [TilläggspostlådaMapparBehörighet](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalenderbehörigheter används vid delning av kalendrar, för att se mer information om hur du delar en Outlook-kalender, se följande artiklar:

- [Dela en Outlook-kalender med andra](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Dela kalendern i Outlook på webben för företag](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Om du vill felsöka kalenderbehörighet kan du använda verktyget [Support- och återställningsassistent.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)