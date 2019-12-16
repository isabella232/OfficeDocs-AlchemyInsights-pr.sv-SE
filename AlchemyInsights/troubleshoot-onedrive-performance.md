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
ms.openlocfilehash: 5416da63851de8b0b45e1d5c0cef24b03db40e6e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054972"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="a7792-102">Felsöka OneDrive-prestanda</span><span class="sxs-lookup"><span data-stu-id="a7792-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="a7792-103">Om du upplever en långsammare än väntat synkronisering eller liknande prestandaproblem med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="a7792-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="a7792-104">Kontrollera att det finns inga kända problem med hjälp av [instrumentpanelen för tjänstens hälsa](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="a7792-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="a7792-105">[Aktivera filer på begäran](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) så att du kan komma åt alla dina filer i OneDrive utan att behöva hämta dem och använda lagringsutrymme på din enhet.</span><span class="sxs-lookup"><span data-stu-id="a7792-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="a7792-106">[Granska metodtips](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) för nätverksplanering och prestanda.</span><span class="sxs-lookup"><span data-stu-id="a7792-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="a7792-107">[Maximera uppladdnings-och nedladdningshastigheten](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), särskilt om du synkroniserar en enhet för första gången.</span><span class="sxs-lookup"><span data-stu-id="a7792-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="a7792-108">Om du synkroniserar ett bibliotek med fler än 100 000 objekt kan OneDrive-synkronisering verka ha fastnat under en längre tid, eller så visar status för bearbetning av 0KB xMB. "</span><span class="sxs-lookup"><span data-stu-id="a7792-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="a7792-109">[Läs mer om hur du synkroniserar mer än 100 000 filer](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) samt [OneDrive stöds gränsen för 300 000 filer](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="a7792-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="a7792-110">När en användare överskrider användningsgränserna begränsar SharePoint Online alla ytterligare begäranden från det användarkontot under en kort period.</span><span class="sxs-lookup"><span data-stu-id="a7792-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="a7792-111">Alla användaråtgärder Stryp medan begränsningen är i kraft.</span><span class="sxs-lookup"><span data-stu-id="a7792-111">All user actions are throttled while the throttle is in effect.</span></span>
