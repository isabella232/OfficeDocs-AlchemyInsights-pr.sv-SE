---
title: Återställa en borttagen gemensam mapp
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
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774549"
---
# <a name="restore-a-deleted-public-folder"></a>Återställa en borttagen gemensam mapp

**Så här återställer du borttagna objekt från en gemensam mapp**:

- Se [att du inte kan återställa borttagna objekt från en gemensam mapp utan e-post i Outlook 2016](https://aka.ms/pfrec).
 
**Så här återställer du en borttagen gemensam mapp (av valfri typ)**: 

- Använd följande EXO PowerShell-kommando:

    Frågesyntaxen

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Exempel: följande kommando återställer Subfolder1 och placerar den under \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Mer information finns i [återställa en borttagen gemensam mapp](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
