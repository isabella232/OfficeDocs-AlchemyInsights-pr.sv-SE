---
title: Begränsning av SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931244"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="77284-102">Begränsning av SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="77284-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="77284-103">**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden.</span><span class="sxs-lookup"><span data-stu-id="77284-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="77284-104">Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar.</span><span class="sxs-lookup"><span data-stu-id="77284-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="77284-105">Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.</span><span class="sxs-lookup"><span data-stu-id="77284-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="77284-106">Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid.</span><span class="sxs-lookup"><span data-stu-id="77284-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="77284-107">Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider.</span><span class="sxs-lookup"><span data-stu-id="77284-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="77284-108">Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.</span><span class="sxs-lookup"><span data-stu-id="77284-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="77284-109">**503-servern är upptagen fel**</span><span class="sxs-lookup"><span data-stu-id="77284-109">**503 server is busy error**</span></span>

<span data-ttu-id="77284-110">Användare kan få ett 503-server är upptaget när de försöker navigera till SharePoint- eller OneDrive-webbplatser.</span><span class="sxs-lookup"><span data-stu-id="77284-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="77284-111">Det här felet kan orsakas av begränsning i SharePoint-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="77284-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="77284-112">SharePoint Online använder begränsning för att upprätthålla optimal prestanda och tillförlitlighet för SharePoint Online-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="77284-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="77284-113">Begränsning begränsar antalet användaråtgärder eller samtidiga anrop (med skript eller kod) för att förhindra överanvändning av resurser.</span><span class="sxs-lookup"><span data-stu-id="77284-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="77284-114">Mer information om begränsning finns i [Undvik att bli begränsad eller blockerad i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="77284-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="77284-115">Om du tror att det här felet inte har något samband med begränsningen kan du kontrollera om det finns aktivt underhåll på din klient genom att navigera till [meddelandecentret](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="77284-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="77284-116">Se slutligen till att du besöker sidan [Service Health](https://portal.office.com/adminportal/home#/servicehealth) för att kontrollera eventuella råd/incidenter som kan inträffa.</span><span class="sxs-lookup"><span data-stu-id="77284-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

