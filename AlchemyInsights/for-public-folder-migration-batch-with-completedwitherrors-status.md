---
title: För batch för flyttning av delad mapp med CompletedWithErrors-status
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158641"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>För batch för flyttning av delad mapp med CompletedWithErrors-status

Använd följande steg för att slutföra batchen och hoppa över de stora/dåliga objekten: 
1. Godkänn de överhoppade objekten på migreringsbatchen:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Använd följande kommando för att godkänna de överhoppade objekten på migreringsbegäranden som är "Synkroniserade" men inte slutförda:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Migreringsbatchen och begäranden ska återupptas och slutföras på några minuter.

