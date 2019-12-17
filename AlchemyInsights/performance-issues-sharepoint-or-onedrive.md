---
title: Prestandaproblem-SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068438"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="b1398-102">SharePoint eller OneDrive är långsam, otillgänglig eller otillgänglig för flera användare</span><span class="sxs-lookup"><span data-stu-id="b1398-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="b1398-103">SharePoint eller OneDrive kan vara långsam, otillgänglig eller otillgänglig, eller kan visa tjänsten otillgänglig eller 503 fel, av flera anledningar:</span><span class="sxs-lookup"><span data-stu-id="b1398-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="b1398-104">Om din SharePoint-eller OneDrive-webbplats är långsam eller försenad för flera användare kan det finnas ett tillfälligt tjänstproblem där användare drabbas av återkommande fördröjningar eller navigeringsfel vid åtkomst till SharePoint-webbplatser eller OneDrive-innehåll.</span><span class="sxs-lookup"><span data-stu-id="b1398-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="b1398-105">Kontrollera den [service Health instrumentpanelen](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) för att se om din organisation påverkas.</span><span class="sxs-lookup"><span data-stu-id="b1398-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="b1398-106">Användare kan få en *503 Server är upptagen* fel när du försöker navigera till SharePoint eller OneDrive webbplatser.</span><span class="sxs-lookup"><span data-stu-id="b1398-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="b1398-107">Det här felet kan orsakas av begränsning i SharePoint-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="b1398-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="b1398-108">SharePoint Online använder begränsning för att bibehålla optimala prestanda och tillförlitlighet för SharePoint Online-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="b1398-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="b1398-109">Begränsning begränsar antalet användaråtgärder eller samtidiga anrop (med skript eller kod) för att förhindra överanvändning av resurser.</span><span class="sxs-lookup"><span data-stu-id="b1398-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="b1398-110">Mer information om begränsning se, [undvika att få begränsas eller blockeras i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="b1398-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="b1398-111">Om du upplever långsamma prestanda med en **klassisk** eller **modern** SharePoint-webbplats eller-sida använder du [diagnostikverktyget](https://aka.ms/perftool) för sidor för att analysera sidorna.</span><span class="sxs-lookup"><span data-stu-id="b1398-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="b1398-112">Om du fortfarande upplever allmänt långsamma prestanda, granska resurserna längst ned i den här artikeln: [Introduktion till prestandajustering för SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="b1398-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  