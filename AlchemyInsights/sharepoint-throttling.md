---
title: Begränsning av SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931460"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="035ee-102">Begränsning av SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="035ee-102">SharePoint Online throttling</span></span>

<span data-ttu-id="035ee-103">**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden.</span><span class="sxs-lookup"><span data-stu-id="035ee-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="035ee-104">Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar.</span><span class="sxs-lookup"><span data-stu-id="035ee-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="035ee-105">Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.</span><span class="sxs-lookup"><span data-stu-id="035ee-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="035ee-106">Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid.</span><span class="sxs-lookup"><span data-stu-id="035ee-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="035ee-107">Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider.</span><span class="sxs-lookup"><span data-stu-id="035ee-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="035ee-108">Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.</span><span class="sxs-lookup"><span data-stu-id="035ee-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="035ee-109">**Begränsning av SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="035ee-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="035ee-110">SharePoint Online använder begränsning för att upprätthålla optimal prestanda och tillförlitlighet för SharePoint Online-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="035ee-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="035ee-111">Begränsning begränsar antalet användaråtgärder eller samtidiga anrop (med skript eller kod) för att förhindra överanvändning av resurser.</span><span class="sxs-lookup"><span data-stu-id="035ee-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="035ee-112">För mer information, besök länkarna nedan.</span><span class="sxs-lookup"><span data-stu-id="035ee-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="035ee-113">Undvik att bli begränsad eller blockerad i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="035ee-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="035ee-114">Datamigrering och SPO-begränsning</span><span class="sxs-lookup"><span data-stu-id="035ee-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="035ee-115">Flyttningshastighet för SharePoint Online och OneDrive</span><span class="sxs-lookup"><span data-stu-id="035ee-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="035ee-116">Hantera Begränsning av SharePoint Online med hjälp av exponentiell back off</span><span class="sxs-lookup"><span data-stu-id="035ee-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="035ee-117">Kapacitetsplanering och belastningstestning av SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="035ee-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

