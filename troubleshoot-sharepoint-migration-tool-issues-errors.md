---
title: Felsöka problem och fel i SharePoint Migration Tool
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931136"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="48c40-102">Felsöka problem och fel i SharePoint Migration Tool</span><span class="sxs-lookup"><span data-stu-id="48c40-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="48c40-103">**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden.</span><span class="sxs-lookup"><span data-stu-id="48c40-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="48c40-104">Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar.</span><span class="sxs-lookup"><span data-stu-id="48c40-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="48c40-105">Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.</span><span class="sxs-lookup"><span data-stu-id="48c40-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="48c40-106">Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid.</span><span class="sxs-lookup"><span data-stu-id="48c40-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="48c40-107">Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider.</span><span class="sxs-lookup"><span data-stu-id="48c40-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="48c40-108">Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.</span><span class="sxs-lookup"><span data-stu-id="48c40-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="48c40-109">**Vanliga problem och fel**</span><span class="sxs-lookup"><span data-stu-id="48c40-109">**Common issues and errors**</span></span>

<span data-ttu-id="48c40-110">Du kan stöta på några vanliga problem och fel när du använder SharePoint Migration Tool (SPMT).</span><span class="sxs-lookup"><span data-stu-id="48c40-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="48c40-111">Vänligen hänvisa till länkarna nedan för mer information.</span><span class="sxs-lookup"><span data-stu-id="48c40-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="48c40-112">Felsöka vanliga SPMT-problem och fel</span><span class="sxs-lookup"><span data-stu-id="48c40-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="48c40-113">Felsöka problem med SPMT-installation</span><span class="sxs-lookup"><span data-stu-id="48c40-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)