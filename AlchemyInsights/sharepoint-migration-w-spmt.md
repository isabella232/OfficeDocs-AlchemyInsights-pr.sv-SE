---
title: SharePoint-migrering med SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931568"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="27b75-102">SharePoint-migrering med SPMT</span><span class="sxs-lookup"><span data-stu-id="27b75-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="27b75-103">**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden.</span><span class="sxs-lookup"><span data-stu-id="27b75-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="27b75-104">Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar.</span><span class="sxs-lookup"><span data-stu-id="27b75-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="27b75-105">Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.</span><span class="sxs-lookup"><span data-stu-id="27b75-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="27b75-106">Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid.</span><span class="sxs-lookup"><span data-stu-id="27b75-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="27b75-107">Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider.</span><span class="sxs-lookup"><span data-stu-id="27b75-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="27b75-108">Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.</span><span class="sxs-lookup"><span data-stu-id="27b75-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="27b75-109">**Migreringsverktyget för SharePoint**</span><span class="sxs-lookup"><span data-stu-id="27b75-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="27b75-110">SharePoint Migration Tool är utformat för migreringar som sträcker sig från den minsta uppsättningen filer till en storskalig företagsmigrering och gör att du kan överföra din information till molnet och dra nytta av det senaste samarbetet, intelligensen och säkerhetslösningar med Office 365.</span><span class="sxs-lookup"><span data-stu-id="27b75-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="27b75-111">Hämta och installera Verktyget för migrering i SharePoint</span><span class="sxs-lookup"><span data-stu-id="27b75-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="27b75-112">Felsöka vanliga SPMT-problem och fel</span><span class="sxs-lookup"><span data-stu-id="27b75-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="27b75-113">Felsöka problem med SPMT-installation</span><span class="sxs-lookup"><span data-stu-id="27b75-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
