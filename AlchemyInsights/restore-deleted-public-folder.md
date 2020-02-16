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
# <a name="restore-a-deleted-public-folder"></a>Återställa en borttagen gemensam mapp

**Så här återställer du borttagna objekt från en gemensam mapp:**

- Se [Du kan inte återställa borttagna objekt från en gemensam mapp som inte skickas i Outlook 2016](https://aka.ms/pfrec).
 
**Så här återställer du en borttagen gemensam mapp (av vilken typ som helst)**: 

- Använd följande KOMMANDOT EXO PowerShell:

    Syntax:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Namn -eq\<" name_of_deleted_public_Folder"}; \<Sökväg$pf-identitetssökväg för digital mapp där mappen återställs>

    Exempel: Följande kommando återställer undermapp1 och placerar den under \Parent1:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Namn -eq "Underfolder1"}; Set-PublicFolder $pf.identity -Path \Parent1

Mer information finns i [Återställa en borttagen gemensam mapp.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)
