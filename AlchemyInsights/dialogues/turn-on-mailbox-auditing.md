---
title: Aktivera postlådegranskning
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429744"
---
# <a name="turn-on-mailbox-auditing"></a>Aktivera postlådegranskning

Om du vill aktivera postlådegranskning för en enskild användare eller en hel organisation kör du följande cmdlets från Remote PowerShell:

- **Enskild användare:** Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
- **Organisation:** Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Mer information finns i Hantera [granskning av postlådor.](https://go.microsoft.com/fwlink/?linkid=2103668)