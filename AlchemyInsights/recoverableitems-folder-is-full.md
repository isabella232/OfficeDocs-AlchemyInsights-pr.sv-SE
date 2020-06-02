---
title: 1336 Mappen RecoverableItems är full
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510770"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="06332-102">Mappen Återställningsbara objekt är full</span><span class="sxs-lookup"><span data-stu-id="06332-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="06332-103">För Exchange Online-postlådor är standardlagringsgränsen för mappen Återställningsbara objekt 30 GB.</span><span class="sxs-lookup"><span data-stu-id="06332-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="06332-104">Lagringsgränsen för mappen Återställningsbara objekt ökas automatiskt till 100 GB om postlådan placeras på bevarande av juridiska skäl, spärr för eDiscovery eller tilldelas en bevarandeprincip.</span><span class="sxs-lookup"><span data-stu-id="06332-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="06332-105">När mappen Återställningsbara objekt når lagringsgränsen påverkas postlådefunktionen på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="06332-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="06332-106">Användaren kan inte ta bort objekt från postlådan.</span><span class="sxs-lookup"><span data-stu-id="06332-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="06332-107">Assistenten för hanterad mapp kan inte ta bort objekt baserat på kvarhållningstagg eller hanterade mappinställningar.</span><span class="sxs-lookup"><span data-stu-id="06332-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="06332-108">För postlådor som har ensidig återställning av ett objekt aktiverat eller har spärrats kan sidskyddsprocessen för copy-on-write inte underhålla versioner av objekt som redigerats av användaren.</span><span class="sxs-lookup"><span data-stu-id="06332-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="06332-109">För postlådor som har loggning av postlådegranskning aktiverat kan inga loggposter för postlådagranskning sparas i undermappen Granskningar i mappen Återställningsbara objekt.</span><span class="sxs-lookup"><span data-stu-id="06332-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="06332-110">För postlådor som inte är spärrade kan administratörer använda `Search-Mailbox -SearchDumpsterOnly -DeleteContent` kommandot i Exchange Online PowerShell för att ta bort objekt i mappen Återställningsbara objekt.</span><span class="sxs-lookup"><span data-stu-id="06332-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="06332-111">Mer information finns i följande avsnitt:</span><span class="sxs-lookup"><span data-stu-id="06332-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="06332-112">Söka efter och ta bort meddelanden</span><span class="sxs-lookup"><span data-stu-id="06332-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="06332-113">Sök-brevlåda</span><span class="sxs-lookup"><span data-stu-id="06332-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="06332-114">För postlådor som är spärrade måste administratörer ta bort spärren innan de kan ta bort objekt från mappen Återställningsbara objekt.</span><span class="sxs-lookup"><span data-stu-id="06332-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="06332-115">Mer information finns [i Ta bort objekt i mappen Återställningsbara objekt för molnbaserade postlådor som är spärrade](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="06332-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="06332-116">För att förhindra att mappen Återställningsbara objekt blir fullständig kan administratörer öka lagringsgränsen för mappen Återställningsbara objekt för spärrade postlådor och ställa in en bevarandeprincip för postlådan som flyttar objekt från mappen Återställningsbara objekt till användarens arkivpostlåda.</span><span class="sxs-lookup"><span data-stu-id="06332-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="06332-117">Se [Öka kvoten För återställningsbara objekt för spärrade postlådor](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="06332-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
