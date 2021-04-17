---
title: Innehållssökning inga resultat
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816866"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="e64b5-102">Inga resultat från innehållssökning/-exporter</span><span class="sxs-lookup"><span data-stu-id="e64b5-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="e64b5-103">Problem med innehållssökning/exporter som inte returnerar några data kan bero på vissa säkerhetsfilter för efterlevnad som har ställts in av en viss administratör och inte meddelar dem till alla administratörer.</span><span class="sxs-lookup"><span data-stu-id="e64b5-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="e64b5-104">Lös problemet genom att kontrollera om det finns säkerhetsfilter för efterlevnad som kan orsaka följande:</span><span class="sxs-lookup"><span data-stu-id="e64b5-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="e64b5-105">Ansluta till Säkerhets- och efterlevnadscenter Powershell</span><span class="sxs-lookup"><span data-stu-id="e64b5-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="e64b5-106">Kör följande kommando:</span><span class="sxs-lookup"><span data-stu-id="e64b5-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="e64b5-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="e64b5-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="e64b5-108">Get-ComplianceSecurityFilter - $org</span><span class="sxs-lookup"><span data-stu-id="e64b5-108">Get-ComplianceSecurityFilter -Organization $org</span></span>