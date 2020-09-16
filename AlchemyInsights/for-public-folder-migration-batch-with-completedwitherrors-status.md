---
title: För gruppmigrering med CompletedWithErrors status
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
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744131"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>För gruppmigrering med CompletedWithErrors status

Följ de här stegen för att slutföra gruppen och hoppa över de stora/dåliga objekten: 
1. Godkänn de objekt som hoppats över i en migreringstabell:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Använd följande kommando för att godkänna överhoppade objekt på begäran om migrering som "synkroniserats" men inte slutförts:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Migreringen och förfrågningarna bör återupptas och slutföras inom några minuter.

