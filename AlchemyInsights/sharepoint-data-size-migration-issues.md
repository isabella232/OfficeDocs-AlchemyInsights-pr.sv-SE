---
title: Problem när du migrerar data till SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931712"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="21784-102">Problem när du migrerar data till SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="21784-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="21784-103">**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden.</span><span class="sxs-lookup"><span data-stu-id="21784-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="21784-104">Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar.</span><span class="sxs-lookup"><span data-stu-id="21784-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="21784-105">Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.</span><span class="sxs-lookup"><span data-stu-id="21784-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="21784-106">Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid.</span><span class="sxs-lookup"><span data-stu-id="21784-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="21784-107">Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider.</span><span class="sxs-lookup"><span data-stu-id="21784-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="21784-108">Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.</span><span class="sxs-lookup"><span data-stu-id="21784-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="21784-109">**Migrera över 100 TB data**</span><span class="sxs-lookup"><span data-stu-id="21784-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="21784-110">Det verkar som om du migrerar över 100 TB data till SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="21784-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="21784-111">Följ stegen nedan så att vi kan hjälpa dig så snart som möjligt.</span><span class="sxs-lookup"><span data-stu-id="21784-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="21784-112">Välj **Ny tjänstbegäran**och sedan **ny servicebegäran**.</span><span class="sxs-lookup"><span data-stu-id="21784-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="21784-113">Lämna rubriken och beskrivningen som **SharePoint-migrering över 100 TB**.</span><span class="sxs-lookup"><span data-stu-id="21784-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="21784-114">När biljetten har skickats, vänligen uppdatera den med följande information:</span><span class="sxs-lookup"><span data-stu-id="21784-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="21784-115">Uppskattad storlek på din migrering.</span><span class="sxs-lookup"><span data-stu-id="21784-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="21784-116">En uppskattning av när du vill starta och slutföra migreringen.</span><span class="sxs-lookup"><span data-stu-id="21784-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="21784-117">Beskriv var du migrerar ditt innehåll från, till exempel SharePoint Server, Box, GDrive, Filresurser osv..</span><span class="sxs-lookup"><span data-stu-id="21784-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

