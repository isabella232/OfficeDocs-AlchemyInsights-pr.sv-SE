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
# <a name="calendar-permissions"></a><span data-ttu-id="1a1ee-102">Kalenderbehörigheter</span><span class="sxs-lookup"><span data-stu-id="1a1ee-102">Calendar Permissions</span></span>

<span data-ttu-id="1a1ee-103">Användare kan ändra sina egna kalenderbehörigheter med Outlook på webben eller andra klienter, men som administratör kan du också behöva undersöka.</span><span class="sxs-lookup"><span data-stu-id="1a1ee-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="1a1ee-104">Med Exchange PowerShell cmdlet visar du behörigheten för en användares kalender:</span><span class="sxs-lookup"><span data-stu-id="1a1ee-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="1a1ee-105">Så här ser du mer information:</span><span class="sxs-lookup"><span data-stu-id="1a1ee-105">To see more information see the following:</span></span>

- [<span data-ttu-id="1a1ee-106">Hämta-mailboxfolderPermission</span><span class="sxs-lookup"><span data-stu-id="1a1ee-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="1a1ee-107">Set-mailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="1a1ee-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="1a1ee-108">TilläggspostlådaMapparBehörighet</span><span class="sxs-lookup"><span data-stu-id="1a1ee-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="1a1ee-109">Kalenderbehörigheter används vid delning av kalendrar, för att se mer information om hur du delar en Outlook-kalender, se följande artiklar:</span><span class="sxs-lookup"><span data-stu-id="1a1ee-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="1a1ee-110">Dela en Outlook-kalender med andra</span><span class="sxs-lookup"><span data-stu-id="1a1ee-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="1a1ee-111">Dela kalendern i Outlook på webben för företag</span><span class="sxs-lookup"><span data-stu-id="1a1ee-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="1a1ee-112">Om du vill felsöka kalenderbehörighet kan du använda verktyget [Support- och återställningsassistent.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)</span><span class="sxs-lookup"><span data-stu-id="1a1ee-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>