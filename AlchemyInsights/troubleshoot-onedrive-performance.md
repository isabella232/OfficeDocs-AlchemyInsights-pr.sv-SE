---
title: Felsöka OneDrive-prestanda
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757903"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="d0998-102">Felsöka OneDrive-prestanda</span><span class="sxs-lookup"><span data-stu-id="d0998-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="d0998-103">Om du har problem med att synkronisera eller liknande prestanda problem med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="d0998-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="d0998-104">Bekräfta att det inte finns några kända problem med [instrument panelen för tjänste hälsa](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="d0998-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="d0998-105">[Aktivera filer på begäran](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) så att du kan komma åt alla filer på OneDrive utan att behöva ladda ned dem och använda lagrings utrymme på din enhet.</span><span class="sxs-lookup"><span data-stu-id="d0998-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="d0998-106">[Läs metod tips](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) för nätverks planering och prestanda.</span><span class="sxs-lookup"><span data-stu-id="d0998-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="d0998-107">[Maximera uppladdnings-och nedladdnings hastighet](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), särskilt om du synkroniserar en enhet för första gången.</span><span class="sxs-lookup"><span data-stu-id="d0998-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="d0998-108">Om du synkroniserar ett bibliotek med fler än 100 000 objekt kan synkronisering med OneDrive verka vara en längre tid eller statusen visar 0KB för xMB. "</span><span class="sxs-lookup"><span data-stu-id="d0998-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="d0998-109">[Läs mer om hur du synkroniserar fler än 100 000-filer](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) samt OneDrive-funktioner som [stöds för 300 000-filer](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="d0998-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="d0998-110">När en användare överskrider användnings gränserna begränsas eventuella fler förfrågningar från det användar kontot under en kort period.</span><span class="sxs-lookup"><span data-stu-id="d0998-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="d0998-111">Alla användar åtgärder begränsas medan begränsningen gäller.</span><span class="sxs-lookup"><span data-stu-id="d0998-111">All user actions are throttled while the throttle is in effect.</span></span>
