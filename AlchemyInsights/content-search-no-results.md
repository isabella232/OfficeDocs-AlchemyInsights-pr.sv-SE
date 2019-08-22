---
title: Innehåll Sök inga resultat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516797"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="33856-102">Inga resultat från innehåll Sök/export</span><span class="sxs-lookup"><span data-stu-id="33856-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="33856-103">Problem med innehåll Sök/export inte returnerar några data kan bero på att vissa krav säkerhetsfilter som installerades av en viss Admin och kommunicerar inte till alla administratörer.</span><span class="sxs-lookup"><span data-stu-id="33856-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="33856-104">Kontrollera om det finns några efterföljande säkerhetsfilter som kan orsaka det här problemet:</span><span class="sxs-lookup"><span data-stu-id="33856-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="33856-105">Ansluta till säkerhet och regelefterlevnadscentret Powershell</span><span class="sxs-lookup"><span data-stu-id="33856-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="33856-106">Kör följande kommandon:</span><span class="sxs-lookup"><span data-stu-id="33856-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="33856-107">$org = ”yourdomain.com”</span><span class="sxs-lookup"><span data-stu-id="33856-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="33856-108">Get-ComplianceSecurityFilter-organisation $org</span><span class="sxs-lookup"><span data-stu-id="33856-108">Get-ComplianceSecurityFilter -Organization $org</span></span>