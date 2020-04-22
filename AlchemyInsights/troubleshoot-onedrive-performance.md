---
title: Felsöka OneDrive-prestanda
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 197a84c5f69f9e58460925049345263743fe78ee
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43733216"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="2a2b2-102">Felsöka OneDrive-prestanda</span><span class="sxs-lookup"><span data-stu-id="2a2b2-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="2a2b2-103">Om du upplever en långsammare synkronisering än förväntat eller liknande prestandaproblem med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="2a2b2-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="2a2b2-104">Bekräfta att det inte finns några kända problem med [instrumentpanelen för tjänstens hälsotillstånd](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="2a2b2-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="2a2b2-105">[Aktivera filer på begäran](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) så att du kan komma åt alla dina filer på OneDrive utan att behöva ladda ned dem alla och använda lagringsutrymme på enheten.</span><span class="sxs-lookup"><span data-stu-id="2a2b2-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="2a2b2-106">[Granska metodtips](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) för nätverksplanering och prestanda.</span><span class="sxs-lookup"><span data-stu-id="2a2b2-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="2a2b2-107">[Maximera uppladdnings- och nedladdningshastigheten](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), särskilt om du synkroniserar en enhet för första gången.</span><span class="sxs-lookup"><span data-stu-id="2a2b2-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="2a2b2-108">Om du synkroniserar ett bibliotek med fler än 100 000 objekt kan OneDrive-synkroniseringen verka ha fastnat under en längre tid, eller så visas bearbetning 0KB xMB."</span><span class="sxs-lookup"><span data-stu-id="2a2b2-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="2a2b2-109">[Läs mer om att synkronisera fler än 100 000 filer](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) samt [OneDrives gräns på 300 000 filer](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)som stöds .</span><span class="sxs-lookup"><span data-stu-id="2a2b2-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="2a2b2-110">När en användare överskrider användningsgränserna begränsar SharePoint Online ytterligare begäranden från det användarkontot under en kort period.</span><span class="sxs-lookup"><span data-stu-id="2a2b2-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="2a2b2-111">Alla användaråtgärder begränsas medan gasreglaget gäller.</span><span class="sxs-lookup"><span data-stu-id="2a2b2-111">All user actions are throttled while the throttle is in effect.</span></span>
