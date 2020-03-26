---
title: Prestanda för SharePoint-migrering
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932406"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="e3c83-102">Prestanda för SharePoint-migrering</span><span class="sxs-lookup"><span data-stu-id="e3c83-102">SharePoint migration performance</span></span>

<span data-ttu-id="e3c83-103">**Viktigt**: många SharePoint Online- och OneDrive-kunder kör företagskritiska applikationer mot den tjänst som körs i bakgrunden.</span><span class="sxs-lookup"><span data-stu-id="e3c83-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e3c83-104">Här ingår lösningar för migrering av innehåll, DLP (skydd mot dataförlust) och säkerhetskopiering.</span><span class="sxs-lookup"><span data-stu-id="e3c83-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e3c83-105">Under dessa tider som saknar motstycke tar vi stegen för att se till att SharePoint Online- och OneDrive-tjänsterna är mycket tillgängliga och tillförlitliga för dina användare som är beroende av tjänsten mer än någonsin i scenarier med distansarbete.</span><span class="sxs-lookup"><span data-stu-id="e3c83-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e3c83-106">För att stödja det målet har vi genomfört strängare begränsningar för bakgrundsprogram (lösningar för migrering, DLP och säkerhetskopiering) under dagtid på veckodagar.</span><span class="sxs-lookup"><span data-stu-id="e3c83-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e3c83-107">Du bör förvänta dig att programmen kommer att uppnå mycket begränsad genomströmning under dessa tider.</span><span class="sxs-lookup"><span data-stu-id="e3c83-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e3c83-108">Under kvällstid och de dagar som anses som helger i regionen står tjänster redo att ta hand om avsevärt högre volymer med förfrågningar från bakgrundsprogram.</span><span class="sxs-lookup"><span data-stu-id="e3c83-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="e3c83-109">**Prestanda för migrering**</span><span class="sxs-lookup"><span data-stu-id="e3c83-109">**Migration performance**</span></span>

<span data-ttu-id="e3c83-110">Prestanda för migrering kan påverkas av nätverksinfrastrukturen, filstorlek, migreringstid och begränsning.</span><span class="sxs-lookup"><span data-stu-id="e3c83-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="e3c83-111">Att förstå dem hjälper dig att planera och maximera effektiviteten i migreringen.</span><span class="sxs-lookup"><span data-stu-id="e3c83-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="e3c83-112">Besök länkarna nedan om du vill ha mer information.</span><span class="sxs-lookup"><span data-stu-id="e3c83-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="e3c83-113">Migreringshastighet för SharePoint Online och ODB</span><span class="sxs-lookup"><span data-stu-id="e3c83-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="e3c83-114">Undvika begränsningar och blockeringar i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="e3c83-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="e3c83-115">Ladda ned och installera migreringsverktyget för SharePoint</span><span class="sxs-lookup"><span data-stu-id="e3c83-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
