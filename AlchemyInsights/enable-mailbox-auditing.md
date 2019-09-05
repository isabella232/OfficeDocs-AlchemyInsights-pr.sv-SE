---
title: Aktivera granskning av postlåda
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736271"
---
# <a name="enable-mailbox-auditing"></a>Aktivera granskning av postlåda

Om du vill aktivera granskning av postlådan för antingen en enskild användare eller en hel organisation följande cmdlets måste köras från Remote Power Shell:
  
 **Enda användare**
  
Set-postlåda-identitet "Jane Dow"-AuditEnabled $true
  
 **Organisation**
  
Get-Mailbox-ResultSize obegränsat-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-postlåda-AuditEnabled $true
  
[Lära sig mer](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

