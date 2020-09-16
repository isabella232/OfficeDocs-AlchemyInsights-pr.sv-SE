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
# <a name="calendar-permissions"></a><span data-ttu-id="609b0-102">Kalender behörigheter</span><span class="sxs-lookup"><span data-stu-id="609b0-102">Calendar Permissions</span></span>

<span data-ttu-id="609b0-103">Användare kan ändra sina egna kalender behörigheter med Outlook på webben eller andra klienter, men som administratör kan du även behöva undersöka det.</span><span class="sxs-lookup"><span data-stu-id="609b0-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="609b0-104">Med Exchange PowerShell cmdlet kan du Visa behörigheten för en användares kalender:</span><span class="sxs-lookup"><span data-stu-id="609b0-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="609b0-105">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="609b0-105">To see more information see the following:</span></span>

- [<span data-ttu-id="609b0-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="609b0-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="609b0-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="609b0-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="609b0-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="609b0-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="609b0-109">Kalender behörigheter används för att dela kalendrar, för att få mer information om att dela en Outlook-kalender, se dessa artiklar:</span><span class="sxs-lookup"><span data-stu-id="609b0-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="609b0-110">Dela en Outlook-kalender med andra</span><span class="sxs-lookup"><span data-stu-id="609b0-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="609b0-111">Dela din kalender i Outlook på webben för företag</span><span class="sxs-lookup"><span data-stu-id="609b0-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="609b0-112">Om du vill felsöka kalender behörighet kan du använda verktyget för [support och återställning](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .</span><span class="sxs-lookup"><span data-stu-id="609b0-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>