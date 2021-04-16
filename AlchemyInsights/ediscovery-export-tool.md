---
title: eDiscovery-exportverktyg
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814606"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="30784-102">Kan du inte installera eller köra eDiscovery-exportverktyget?</span><span class="sxs-lookup"><span data-stu-id="30784-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="30784-103">Om du inte kan installera eller köra eDiscovery-exportverktyget för att ladda ned sökresultat kontrollerar du följande:</span><span class="sxs-lookup"><span data-stu-id="30784-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="30784-104">Datorn du använder uppfyller dessa krav:</span><span class="sxs-lookup"><span data-stu-id="30784-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="30784-105">32- eller 64-bitarsversioner av Windows 7 och senare versioner</span><span class="sxs-lookup"><span data-stu-id="30784-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="30784-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="30784-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="30784-107">En webbläsare som stöds:</span><span class="sxs-lookup"><span data-stu-id="30784-107">A supported browser:</span></span>

  - <span data-ttu-id="30784-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="30784-108">Microsoft Edge</span></span>

    <span data-ttu-id="30784-109">Eller</span><span class="sxs-lookup"><span data-stu-id="30784-109">Or</span></span>

  - <span data-ttu-id="30784-110">Internet Explorer 10 och senare versioner</span><span class="sxs-lookup"><span data-stu-id="30784-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="30784-111">Andra webbläsare, till exempel Google Chrome och Mozilla Firefox, stöds inte.</span><span class="sxs-lookup"><span data-stu-id="30784-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="30784-112">Din organisation kan ansluta till slutpunkten i Azure, som är **\* .blob.core.windows.net** (jokertecknet representerar en unik identifierare för exportjobbet).</span><span class="sxs-lookup"><span data-stu-id="30784-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="30784-113">Du har tilldelats exportrollen i Säkerhetsefterlevnadscenter för Microsoft 365. &amp;</span><span class="sxs-lookup"><span data-stu-id="30784-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="30784-114">Som standard är den här rollen endast tilldelad rollgruppen för eDiscovery-hanteraren.</span><span class="sxs-lookup"><span data-stu-id="30784-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="30784-115">Se [Tilldela eDiscovery-behörigheter](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="30784-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="30784-116">Mer information finns i [Exportera resultat för innehållssökning.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="30784-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="30784-117">Om du exporterar fler än 100 000 postlådor måste du använda följande Powershell för att ladda ned exportresultatet: Exportera resultat från fler än [100 000 postlådor.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="30784-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>