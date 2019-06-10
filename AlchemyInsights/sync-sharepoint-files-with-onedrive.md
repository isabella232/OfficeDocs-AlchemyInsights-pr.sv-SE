---
title: Synkronisera SharePoint-filer med den nya OneDrive-synkroniseringsklienten
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 74b79efeb7e46d03dc55f46252d152cd13e66c84
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757837"
---
# <a name="sync-sharepoint-files-with-the-new-onedrive-sync-client"></a><span data-ttu-id="5b3cd-102">Synkronisera SharePoint-filer med den nya OneDrive-synkroniseringsklienten</span><span class="sxs-lookup"><span data-stu-id="5b3cd-102">Sync SharePoint files with the new OneDrive sync client</span></span>

<span data-ttu-id="5b3cd-103">Kommandot Öppna med Utforskaren öppnar en lokal instans av Utforskaren som visar mappstrukturen på den server som är värd för SharePoint-webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="5b3cd-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="5b3cd-104">Vi rekommenderar att du [synkroniserar SharePoint-filer med den nya OneDrive-synkroniseringsklienten](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> som tillhandahåller [filer på begäran](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), eftersom det ger lokal åtkomst till dina filer och ger bästa möjliga prestanda.</span><span class="sxs-lookup"><span data-stu-id="5b3cd-104">This being said , we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="5b3cd-105">Om du väljer att använda Utforskarvyn i stället för den nya synkroniseringsklienten ska du vara noga med att följa anvisningarna och metodtipsen i artiklarna nedan.</span><span class="sxs-lookup"><span data-stu-id="5b3cd-105">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span>

- [<span data-ttu-id="5b3cd-106">Använda kommandot "Öppna med Utforskaren" för felsökning av problem i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5b3cd-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- <span data-ttu-id="5b3cd-107">[Kopiera eller flytta biblioteksfiler med hjälp av Öppna med Utforskaren](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)</span><span class="sxs-lookup"><span data-stu-id="5b3cd-107">See [Video: Copy or move library files by using Open with Explorer](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2).</span></span>

<span data-ttu-id="5b3cd-108">Obs! Knappen Öppna med Utforskaren visas inte i den nya biblioteksvyn.</span><span class="sxs-lookup"><span data-stu-id="5b3cd-108">Note:  The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="5b3cd-109">Klicka på listrutan Visa i det övre högra hörnet (namnet på listrutan ändras beroende på aktuell vy) och klicka sedan på Visa i Utforskaren.</span><span class="sxs-lookup"><span data-stu-id="5b3cd-109">Click the View drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click View in File Explorer.</span></span>

 <span data-ttu-id="5b3cd-110">Öppna med Utforskaren i SharePoint använder ActiveX-kontroller, så det stöds endast i Internet Explorer 10 eller 11.</span><span class="sxs-lookup"><span data-stu-id="5b3cd-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="5b3cd-111">Öppna med Utforskaren fungerar inte i Windows med Microsoft Edge, Google Chrome, Mozilla Firefox eller på Mac-plattformen.</span><span class="sxs-lookup"><span data-stu-id="5b3cd-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="5b3cd-112">På grund av detta kan alternativet Utforskarvy vara nedtonat.</span><span class="sxs-lookup"><span data-stu-id="5b3cd-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

- <span data-ttu-id="5b3cd-113">[Varför knappar på SharePoints menyflikar inte är tillgängliga](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="5b3cd-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

