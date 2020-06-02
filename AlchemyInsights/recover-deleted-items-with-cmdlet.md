---
title: Återställa borttagna objekt med cmdlet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 86744d92a44096991079d1da3bdf4e95e58c55b7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493428"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="1c685-102">Återställa borttagna objekt med cmdlet</span><span class="sxs-lookup"><span data-stu-id="1c685-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="1c685-103">Använd cmdleten [Get-RecoverItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) om du vill visa borttagna objekt i postlådor.</span><span class="sxs-lookup"><span data-stu-id="1c685-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="1c685-104">När du har hittat de borttagna objekten använder du cmdleten [Restore-RecoverItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) för att återställa dem.</span><span class="sxs-lookup"><span data-stu-id="1c685-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="1c685-105">Se fullständig information i [Get-RecoverAbleItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="1c685-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="1c685-106">Du måste tilldelas rollen Exportera postlådan importera export innan du kan köra den här cmdleten.</span><span class="sxs-lookup"><span data-stu-id="1c685-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="1c685-107">Mer information finns [i Get-RecoverItems.](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="1c685-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
