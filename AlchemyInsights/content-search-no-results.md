---
title: Innehålls sökning inga resultat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680665"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="8dcb4-102">Inga resultat från innehålls sökning/export</span><span class="sxs-lookup"><span data-stu-id="8dcb4-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="8dcb4-103">Problem med innehålls sökning/exporterar inte några data kan bero på vissa säkerhets filter för efterlevnad som konfigurerades av en viss administratör och inte kommunicerar med alla administratörer.</span><span class="sxs-lookup"><span data-stu-id="8dcb4-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="8dcb4-104">Lös problemet genom att kontrol lera om det finns några säkerhets filter för efterlevnad som kan orsaka detta:</span><span class="sxs-lookup"><span data-stu-id="8dcb4-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="8dcb4-105">Ansluta till säkerhets-och Compliance Center PowerShell</span><span class="sxs-lookup"><span data-stu-id="8dcb4-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="8dcb4-106">Kör följande cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8dcb4-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="8dcb4-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="8dcb4-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="8dcb4-108">Skaffa-ComplianceSecurityFilter-organisation $org</span><span class="sxs-lookup"><span data-stu-id="8dcb4-108">Get-ComplianceSecurityFilter -Organization $org</span></span>