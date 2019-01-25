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
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="7ede0-102">Aktivera granskning av postlåda</span><span class="sxs-lookup"><span data-stu-id="7ede0-102">Enable mailbox auditing</span></span>

<span data-ttu-id="7ede0-103">Om du vill aktivera granskning för postlåda för en enskild användare eller en hel organisation måste följande cmdlets köras från Remote Power Shell:</span><span class="sxs-lookup"><span data-stu-id="7ede0-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="7ede0-104">**Enskild användare**</span><span class="sxs-lookup"><span data-stu-id="7ede0-104">**Single User**</span></span>
  
<span data-ttu-id="7ede0-105">Set-postlåda - identitet ”Jane Dow” - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="7ede0-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="7ede0-106">**Organisation**</span><span class="sxs-lookup"><span data-stu-id="7ede0-106">**Organization**</span></span>
  
<span data-ttu-id="7ede0-107">Get-Mailbox - ResultSize obegränsat - filtrera {RecipientTypeDetails - eq ”UserMailbox”} | Set-postlåda - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="7ede0-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
<span data-ttu-id="7ede0-108">Läs mer</span><span class="sxs-lookup"><span data-stu-id="7ede0-108">[Learn more](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)</span></span>
  

