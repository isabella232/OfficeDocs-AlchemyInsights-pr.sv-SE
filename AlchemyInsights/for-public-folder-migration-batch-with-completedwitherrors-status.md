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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043623"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>För batch för flyttning av delad mapp med CompletedWithErrors-status

Använd följande steg för att slutföra batchen och hoppa över de stora/dåliga objekten: 
1. Godkänn de överhoppade objekten på migreringsbatchen:

    Batchnamn för \<set-migrationbatchnamn> -GodkännSkippedItems 
2. Använd följande kommando för att godkänna de överhoppade objekten på migreringsbegäranden som är "Synkroniserade" men inte slutförda:

    $pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -includeReport; ForEach ($i i $pf) {om ($i.LargeItemsEncountered -gt 0 -eller $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}
3. Migreringsbatchen och begäranden ska återupptas och slutföras på några minuter.

