---
title: Återställa en borttagen gemensam mapp
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
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063760"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="f102c-102">Återställa en borttagen gemensam mapp</span><span class="sxs-lookup"><span data-stu-id="f102c-102">Restore a deleted public folder</span></span>

<span data-ttu-id="f102c-103">**Så här återställer du borttagna objekt från en gemensam mapp:**</span><span class="sxs-lookup"><span data-stu-id="f102c-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="f102c-104">Se [Du kan inte återställa borttagna objekt från en gemensam mapp som inte skickas i Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="f102c-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="f102c-105">**Så här återställer du en borttagen gemensam mapp (av vilken typ som helst)**:</span><span class="sxs-lookup"><span data-stu-id="f102c-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="f102c-106">Använd följande KOMMANDOT EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="f102c-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="f102c-107">Syntax:</span><span class="sxs-lookup"><span data-stu-id="f102c-107">Syntax:</span></span>

    ><span data-ttu-id="f102c-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Namn -eq\<" name_of_deleted_public_Folder"}; \<Sökväg$pf-identitetssökväg för digital mapp där mappen återställs></span><span class="sxs-lookup"><span data-stu-id="f102c-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="f102c-109">Exempel: Följande kommando återställer undermapp1 och placerar den under \Parent1:</span><span class="sxs-lookup"><span data-stu-id="f102c-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="f102c-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Namn -eq "Underfolder1"}; Set-PublicFolder $pf.identity -Path \Parent1</span><span class="sxs-lookup"><span data-stu-id="f102c-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="f102c-111">Mer information finns i [Återställa en borttagen gemensam mapp.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)</span><span class="sxs-lookup"><span data-stu-id="f102c-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
