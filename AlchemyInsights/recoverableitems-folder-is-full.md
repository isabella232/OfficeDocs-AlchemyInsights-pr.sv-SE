---
title: 1336 RecoverableItems mappen är full
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 14d46980caf7dac90e73c34482a3aee34382fa1f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389101"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="90802-102">Objekt som kan återskapas mappen är full</span><span class="sxs-lookup"><span data-stu-id="90802-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="90802-103">För Exchange Online-postlådor i Office 365 är standard lagringsgränsen för objekt som kan återskapas mappen 30 GB.</span><span class="sxs-lookup"><span data-stu-id="90802-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="90802-104">Lagringsgränsen för objekt som kan återskapas mappen ökar automatiskt till 100 GB om postlådan placeras på rättstvist håller e-informationsavslöjande Håll eller tilldelas en bevarandeprincip för Office 365.</span><span class="sxs-lookup"><span data-stu-id="90802-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>

<span data-ttu-id="90802-105">När objekt som kan återskapas mappen överskrider lagringsgränsen, påverkas postlåda funktioner på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="90802-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="90802-106">Användaren kan inte ta bort objekt från postlådan.</span><span class="sxs-lookup"><span data-stu-id="90802-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="90802-107">Hanterade Mapphanteraren kan inte radera objekt baserat på kvarhållande tagg eller inställningar för hanterade mappar.</span><span class="sxs-lookup"><span data-stu-id="90802-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="90802-108">Kopiera-on-write sidan skydd processen inte kan upprätthålla versioner av objekt redigeras av användaren för postlådor som har enstaka objekt återställning aktiverat eller har spärrats.</span><span class="sxs-lookup"><span data-stu-id="90802-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="90802-109">För postlådor som har postlådan granskningsloggning aktiverats kan ingen logg granskningsposter postlåda sparas i revisioner undermapp i mappen objekt som kan återskapas.</span><span class="sxs-lookup"><span data-stu-id="90802-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="90802-110">Administratörer kan använda för postlådor som inte är spärrade, de `Search-Mailbox -SearchDumpsterOnly -DeleteContent` i Exchange Online PowerShell för att ta bort objekt i mappen objekt som kan återskapas.</span><span class="sxs-lookup"><span data-stu-id="90802-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="90802-111">Mer information finns i följande avsnitt:</span><span class="sxs-lookup"><span data-stu-id="90802-111">For more information, see the following topics:</span></span> 

- [<span data-ttu-id="90802-112">Söka efter och ta bort meddelanden</span><span class="sxs-lookup"><span data-stu-id="90802-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="90802-113">Sök-postlåda</span><span class="sxs-lookup"><span data-stu-id="90802-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="90802-114">Administratörer måste ta bort spärren innan de kan borttagna objekt från mappen objekt som kan återskapas för postlådor som är spärrade.</span><span class="sxs-lookup"><span data-stu-id="90802-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="90802-115">Mer information finns i [Ta bort objekt i objekt som kan återskapas mappen för molnbaserade postlådor på Håll](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="90802-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="90802-116">För att förhindra att objekt som kan återskapas mappen blir full, kan administratörer öka lagringsgränsen för de objekt som kan återskapas mappen för postlådor på Håll och ställa in en bevarandeprincip för postlådan som flyttar objekt från mappen objekt som kan återskapas till användarens Arkiv e-postlådan.</span><span class="sxs-lookup"><span data-stu-id="90802-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="90802-117">Se [öka objekt som kan återskapas kvoten för postlådor på Håll](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="90802-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
