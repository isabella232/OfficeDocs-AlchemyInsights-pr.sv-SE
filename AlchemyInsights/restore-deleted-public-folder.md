---
title: Återställa en borttagna gemensamma mapp
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
- "3488"
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943393"
---
# <a name="restore-a-deleted-public-folder"></a>Återställa en borttagna gemensamma mapp

**Så här återställer du borttagna objekt från en offentlig mapp:**

- Mer [information finns i Det går inte att återställa borttagna objekt från en offentlig mapp som inte är en e-postmapp i Outlook 2016](https://aka.ms/pfrec).
 
**Återställa en borttagna gemensamma mapp (av alla typer)**: 

- Använd följande EXO PowerShell-kommando:

    Syntax:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Exempel: Följande kommando återställer undermapp1 och placerar det under \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Mer [information finns i Återställa en borttagna](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) gemensamma mapp.
