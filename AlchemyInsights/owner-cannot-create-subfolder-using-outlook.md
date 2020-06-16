---
title: Ägaren kan inte skapa undermapp med Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749146"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Ägaren kan inte skapa undermapp med Outlook

**Det finns ett pågående problem med att ägare av gemensamma mappar skapar undermappar med Outlook. Problemet kommer att åtgärdas snart.**

Under tiden använder du någon av följande lösningar:

1. Använd Outlook för MAC för att skapa undermappen eftersom problemet endast påverkar Outlook för skrivbordsfönster (alla versioner)
2. Låt administratören skapa undermappen med EXO Shell eller EAC
3. Ändra DefaultPublicFolderMailbox/EffectivePublicFolderMailbox på användaren till annan postlåda än innehållspostlådan för mappen som orsakar problem  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Vänta i en timme, starta om Outlook-klienten