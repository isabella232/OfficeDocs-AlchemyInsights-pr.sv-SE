---
title: Aktivera postlådegranskning
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: c04f27edc1e22e0e4269758827d5468767967be8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814210"
---
# <a name="enable-mailbox-auditing"></a>Aktivera postlådegranskning

Om du vill aktivera postlådegranskning för en enskild användare eller en hel organisation måste du köra följande cmdlets från Remote Power Shell:
  
 **En enskild användare**
  
Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
  
 **Organisation**
  
Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true
  
[Läs mer](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

