---
title: Prestanda problem-SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771919"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="55f98-102">SharePoint eller OneDrive långsamt, otillgängligt eller otillgängligt för flera användare</span><span class="sxs-lookup"><span data-stu-id="55f98-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="55f98-103">SharePoint eller OneDrive kan vara långsamt, otillgängliga eller otillgängliga eller kanske Visa tjänsten ej tillgänglig eller 503 fel, av olika anledningar:</span><span class="sxs-lookup"><span data-stu-id="55f98-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="55f98-104">Om din SharePoint-eller OneDrive-webbplats är långsam eller fördröjd för flera användare kan det finnas ett tillfälligt tjänst problem där användarna upplever fördröjningar eller navigerings fel vid åtkomst till SharePoint-webbplatser eller OneDrive-innehåll.</span><span class="sxs-lookup"><span data-stu-id="55f98-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="55f98-105">Kontrol lera [instrument panelen för tjänstens hälsa](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) för att se om din organisation påverkas.</span><span class="sxs-lookup"><span data-stu-id="55f98-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="55f98-106">Användare kan få en *503-server att vara upptagen* när du försöker navigera till SharePoint-eller OneDrive-webbplatser.</span><span class="sxs-lookup"><span data-stu-id="55f98-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="55f98-107">Det här felet kan orsakas av begränsning i SharePoint-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="55f98-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="55f98-108">SharePoint Online använder begränsning för att bibehålla optimala prestanda och tillförlitlighet i SharePoint Online-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="55f98-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="55f98-109">Begränsningen begränsar antalet användaråtgärder och samtidiga anrop (med skript eller kod) för att förhindra att resurserna utnyttjas för mycket.</span><span class="sxs-lookup"><span data-stu-id="55f98-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="55f98-110">Mer information om begränsning finns i [undvika begränsning eller blockering i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="55f98-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="55f98-111">Om du upplever låga prestanda med en **klassisk** eller **modern** SharePoint-webbplats eller-sida kan du använda [verktyget](https://aka.ms/perftool) för att analysera sidorna.</span><span class="sxs-lookup"><span data-stu-id="55f98-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="55f98-112">Om du fortfarande upplever allmän långsam prestanda kan du gå igenom resurserna längst ned i den här artikeln: [Introduktion till prestanda justering för SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="55f98-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  