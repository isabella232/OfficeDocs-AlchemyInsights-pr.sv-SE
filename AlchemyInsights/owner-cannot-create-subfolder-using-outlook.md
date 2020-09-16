---
title: Ägaren kan inte skapa undermappen med Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665736"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Ägaren kan inte skapa undermappen med Outlook

**Det finns ett pågående problem med privata ägarnoder som skapar undermappar med Outlook. Problemet åtgärdas snart.**

Under tiden kan du använda någon av följande lösningar:

1. Använda Outlook för MAC för att skapa undermappen eftersom problemet endast påverkar Outlook för Skriv bords fönster (alla versioner)
2. Be administratören skapa undermappen med EXO skal eller UK
3. Ändra DefaultPublicFolderMailbox/EffectivePublicFolderMailbox för användaren till en annan post låda än innehålls post lådan för mappen som orsakar problemet  
    - *Set-post låda Användare1 DefaultPublicFolderMailbox PubMBX3*
4. Vänta i en timme, starta om Outlook-klient