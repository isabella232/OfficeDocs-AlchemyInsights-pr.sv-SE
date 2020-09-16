---
title: 1336 RecoverableItems-mappen är full
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741285"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="64208-102">Mappen för återställnings bara objekt är full</span><span class="sxs-lookup"><span data-stu-id="64208-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="64208-103">För Exchange Online-postlådor är standard lagrings gränsen 30 GB för mappen för återställnings bara objekt.</span><span class="sxs-lookup"><span data-stu-id="64208-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="64208-104">Gränsen för lagrings utrymmet för mappen för återställnings bara objekt höjs automatiskt till 100 GB om post lådan är placerad i en begränsnings spärr, eDiscovery-undantag eller är kopplad till en bevarande princip.</span><span class="sxs-lookup"><span data-stu-id="64208-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="64208-105">När mappen för återställnings bara objekt når lagrings gränsen påverkas funktionen för post lådor på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="64208-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="64208-106">Användaren kan inte ta bort objekt från post lådan.</span><span class="sxs-lookup"><span data-stu-id="64208-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="64208-107">Assistenten för hanterade mappar kan inte ta bort objekt baserat på bevarande kod eller inställningar för hanterade mappar.</span><span class="sxs-lookup"><span data-stu-id="64208-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="64208-108">För att post lådor med återställning av enskilt objekt är aktiverat eller parkerade kan inte kopierings skydds processen hantera de objekt som redigerats av användaren.</span><span class="sxs-lookup"><span data-stu-id="64208-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="64208-109">För post lådor som har post lådans gransknings loggning aktive rad kan inga gransknings poster för post lådor sparas i undermappen revisioner i mappen återställnings bara objekt.</span><span class="sxs-lookup"><span data-stu-id="64208-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="64208-110">För brev lådor som inte är parkerade kan administratörer använda `Search-Mailbox -SearchDumpsterOnly -DeleteContent` kommandot i Exchange Online PowerShell för att ta bort objekt i mappen för återställnings bara objekt.</span><span class="sxs-lookup"><span data-stu-id="64208-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="64208-111">Mer information finns i följande avsnitt:</span><span class="sxs-lookup"><span data-stu-id="64208-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="64208-112">Söka efter och ta bort meddelanden</span><span class="sxs-lookup"><span data-stu-id="64208-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="64208-113">Sök-post låda</span><span class="sxs-lookup"><span data-stu-id="64208-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="64208-114">För att post lådor ska blockeras måste administratörer ta bort spärren innan de kan ta bort objekt från mappen för återställnings bara objekt.</span><span class="sxs-lookup"><span data-stu-id="64208-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="64208-115">Mer information finns i [ta bort objekt i mappen för återställnings bara objekt i molnbaserade post lådor](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="64208-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="64208-116">För att förhindra att mappen återställnings bara objekt blir full kan administratörerna öka lagrings gränsen för mappen för återställnings bara objekt för post lådor med undantag och konfigurera en bevarande princip för post lådor som flyttar objekt från mappen för återställnings bara objekt till användarens arkiv post låda.</span><span class="sxs-lookup"><span data-stu-id="64208-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="64208-117">Se [öka kvoten för återställnings bara objekt för post lådor](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="64208-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
