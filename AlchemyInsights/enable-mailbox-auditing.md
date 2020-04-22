---
title: Aktivera granskning av postlådor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703589"
---
# <a name="enable-mailbox-auditing"></a>Aktivera granskning av postlådor

Om du vill aktivera postlådegranskning för antingen en enskild användare eller en hel organisation måste följande cmdlets köras från Remote Power Shell:
  
 **En användare**
  
Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
  
 **Organisation**
  
Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-mailbox -AuditEnabled $true
  
[Läs mer](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

