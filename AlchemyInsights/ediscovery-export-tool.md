---
title: verktyget för eDiscovery-export
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277936"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="b1fb4-102">Kan du inte installera eller köra verktyget för eDiscovery-export?</span><span class="sxs-lookup"><span data-stu-id="b1fb4-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="b1fb4-103">Om du inte kan installera eller köra verktyget för eDiscovery-export för att hämta Sök resultat kan du kontrol lera följande:</span><span class="sxs-lookup"><span data-stu-id="b1fb4-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="b1fb4-104">Den dator du använder uppfyller dessa krav:</span><span class="sxs-lookup"><span data-stu-id="b1fb4-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="b1fb4-105">32-eller 64-bitars versioner av Windows 7 och senare versioner</span><span class="sxs-lookup"><span data-stu-id="b1fb4-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="b1fb4-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="b1fb4-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="b1fb4-107">En webbläsare som stöds:</span><span class="sxs-lookup"><span data-stu-id="b1fb4-107">A supported browser:</span></span>

  - <span data-ttu-id="b1fb4-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b1fb4-108">Microsoft Edge</span></span>

    <span data-ttu-id="b1fb4-109">Eller</span><span class="sxs-lookup"><span data-stu-id="b1fb4-109">Or</span></span>

  - <span data-ttu-id="b1fb4-110">Internet Explorer 10 och senare versioner</span><span class="sxs-lookup"><span data-stu-id="b1fb4-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="b1fb4-111">Andra webbläsare, till exempel Google Chrome och Mozilla Firefox, stöds inte.</span><span class="sxs-lookup"><span data-stu-id="b1fb4-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="b1fb4-112">Din organisation kan ansluta till slut punkten i Azure, som är \*\* \* . blob.Core.Windows.net\*\* (jokertecknet representerar en unik identifierare för ditt export jobb).</span><span class="sxs-lookup"><span data-stu-id="b1fb4-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="b1fb4-113">Du har tilldelats export rollen i Microsoft 365 Security &amp; Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="b1fb4-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="b1fb4-114">Som standard är den här rollen bara tilldelad till roll gruppen eDiscovery Manager.</span><span class="sxs-lookup"><span data-stu-id="b1fb4-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="b1fb4-115">Se [tilldela eDiscovery-behörigheter](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="b1fb4-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="b1fb4-116">Mer information finns i [Exportera innehålls Sök Resultat](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="b1fb4-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="b1fb4-117">Om du exporterar fler än 100K-postlådor måste du använda följande PowerShell för att ladda ned export resultaten:  [Exportera resultat från fler än 100K-postlådor](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="b1fb4-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>