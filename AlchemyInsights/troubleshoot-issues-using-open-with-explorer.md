---
title: Felsöka problem med att öppna Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 6e67c2916e0c5739f6126064d45e175a7fd6f8d4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500233"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="10c43-102">Åtgärda problem med att öppna med Explorer</span><span class="sxs-lookup"><span data-stu-id="10c43-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="10c43-103">Åtgärda vanliga problem med att öppna ett dokumentbibliotek i SharePoint eller OneDrive med hjälp av kommandot **Öppna med Utforskaren** :</span><span class="sxs-lookup"><span data-stu-id="10c43-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="10c43-104">Använda Internet Explorer 10 eller 11 för Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="10c43-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="10c43-105">**Öppna med Utforskaren** inte är kompatibel med Microsoft Edge, Google Chrome, Firefox och andra.</span><span class="sxs-lookup"><span data-stu-id="10c43-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="10c43-106">**Öppna med Utforskaren** är inaktiverat i alla webbläsare utom Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="10c43-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="10c43-107">**Öppna med Utforskaren** är inte tillgänglig i den moderna upplevelsen för SharePoint-bibliotek.</span><span class="sxs-lookup"><span data-stu-id="10c43-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="10c43-108">Använd **vyn i File Explorer** istället.</span><span class="sxs-lookup"><span data-stu-id="10c43-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="10c43-109">Välj **Visa alternativ** \> **Visa i File Explorer**.</span><span class="sxs-lookup"><span data-stu-id="10c43-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="10c43-110">Visa i File Explorer är inte kompatibel med Microsoft Edge, Google Chrome, Firefox och andra.</span><span class="sxs-lookup"><span data-stu-id="10c43-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="10c43-111">**Visa i File Explorer** i endast i Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="10c43-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="10c43-112">Kontrollera att WebClient-tjänsten körs.</span><span class="sxs-lookup"><span data-stu-id="10c43-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="10c43-113">Markera appen som kör Fjärrskrivbord i rutan Windows Sök, kör, Skriv, Skriv services.msc och tryck sedan på RETUR.</span><span class="sxs-lookup"><span data-stu-id="10c43-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="10c43-114">Rulla ned till WebClient-tjänsten och kontrollera att kolumnen **Status** visar ”kör”.</span><span class="sxs-lookup"><span data-stu-id="10c43-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="10c43-115">Om den inte dubbelklicka på tjänsten, klicka på **Start**och klicka sedan på **OK**.</span><span class="sxs-lookup"><span data-stu-id="10c43-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="10c43-116">(Du kanske måste först aktivera tjänsten genom att välja **Manuell** eller **automatisk** i rutan **Startmetod** .)</span><span class="sxs-lookup"><span data-stu-id="10c43-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="10c43-117">Öppna ett bibliotek i File Explorer är praktiskt om du vill kopiera eller flytta flera filer och mappar när, men om du regelbundet arbetar i biblioteket, rekommenderar vi synkroniserar den.</span><span class="sxs-lookup"><span data-stu-id="10c43-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="10c43-118">Felsökning av problem med öppna i File Explorer finns i [Öppna i Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="10c43-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="10c43-119">Information om hur du konfigurerar synkronisering finns i [synkronisera SharePoint-filer med den nya OneDrive sync-klienten](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="10c43-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="10c43-120">Se artikel [hur du använder kommandot ”Öppna med Utforskaren” felsökning av problem i SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) för mer information.</span><span class="sxs-lookup"><span data-stu-id="10c43-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

