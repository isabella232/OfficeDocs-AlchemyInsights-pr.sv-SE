---
title: Det går inte att skapa en undermapp i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836153"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Det går inte att skapa en undermapp i Outlook

**Det finns ett pågående problem med att ägare av gemensamma mappar skapar undermappar med Outlook. Problemet kommer att åtgärdas inom kort.**

Under tiden kan du använda någon av följande lösningar:

1. Använd Outlook för MAC för att skapa undermappen eftersom problemet bara påverkar Outlook för skrivbordsfönster (alla versioner)
2. Be administratören skapa undermappen med EXO Shell eller EAC
3. Ändra rutan DefaultPublicFolderMailbox/EffectivePublicFolderMailbox för användaren till en annan postlåda än innehållspostlådan för mappen som orsakar problemet  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Vänta en timme, starta om Outlook-klienten