---
title: Aktivera granskning av postlåda
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29500300"
---
# <a name="enable-mailbox-auditing"></a>Aktivera granskning av postlåda

Om du vill aktivera granskning för postlåda för en enskild användare eller en hel organisation måste följande cmdlets köras från Remote Power Shell:
  
 **Enskild användare**
  
Set-postlåda - identitet ”Jane Dow” - AuditEnabled $true
  
 **Organisation**
  
Get-Mailbox - ResultSize obegränsat - filtrera {RecipientTypeDetails - eq ”UserMailbox”} | Set-postlåda - AuditEnabled $true
  
Läs mer
  

