---
title: För migreringsbatch för offentlig mapp med CompletedWithErrors-status
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
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812482"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>För migreringsbatch för offentlig mapp med CompletedWithErrors-status

Gör så här för att slutföra batchen och hoppa över de stora/dåliga objekten: 
1. Godkänn de överhoppade objekten i migreringsbatchen:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Använd följande kommando för att godkänna de överhoppade objekten på migreringsförfrågningar som är "synkroniserade" men inte slutförda:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Migreringsbatchen och förfrågningar bör återupptas och slutföras om några minuter.

