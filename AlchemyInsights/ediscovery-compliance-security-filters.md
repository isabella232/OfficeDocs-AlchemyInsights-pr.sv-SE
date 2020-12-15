---
title: Inga resultat som returneras under innehålls sökning
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680329"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="8be7a-102">Inga resultat som returneras under innehålls sökning</span><span class="sxs-lookup"><span data-stu-id="8be7a-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="8be7a-103">Om du har problem med följande eDiscovery-scenarier:</span><span class="sxs-lookup"><span data-stu-id="8be7a-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="8be7a-104">Innehålls sökning/export returnerar inga data eller oväntade data</span><span class="sxs-lookup"><span data-stu-id="8be7a-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="8be7a-105">eDiscovery-sökning eller export Miss lyckas</span><span class="sxs-lookup"><span data-stu-id="8be7a-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="8be7a-106">Detta kan bero på att vissa säkerhets filter för efterlevnad har ställts in av en viss administratör och inte har meddelats till alla administratörer.</span><span class="sxs-lookup"><span data-stu-id="8be7a-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="8be7a-107">Lös problemet genom att kontrol lera om det finns några säkerhets filter för efterlevnad som kan orsaka dessa problem:</span><span class="sxs-lookup"><span data-stu-id="8be7a-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="8be7a-108">Ansluta till säkerhets-och Compliance Center PowerShell</span><span class="sxs-lookup"><span data-stu-id="8be7a-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="8be7a-109">Kör följande cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8be7a-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="8be7a-110">Mer information om säkerhets filter för efterlevnad finns i avsnittet [behörigheter för innehålls sökning](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="8be7a-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
