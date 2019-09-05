---
title: Felsöka problem med öppna med Utforskaren
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
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742751"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="5636b-102">Åtgärda problem med öppna med Utforskaren</span><span class="sxs-lookup"><span data-stu-id="5636b-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="5636b-103">Åtgärda vanliga problem med att öppna ett dokumentbibliotek i SharePoint eller OneDrive med kommandot **Öppna med Utforskaren** :</span><span class="sxs-lookup"><span data-stu-id="5636b-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="5636b-104">Använd Internet Explorer 10 eller 11 i Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="5636b-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="5636b-105">**Öppna med Utforskaren** är inte kompatibel med Microsoft Edge, Google Chrome, Firefox och andra.</span><span class="sxs-lookup"><span data-stu-id="5636b-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="5636b-106">**Öppna med Utforskaren** är inaktiverat i alla webbläsare utom Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="5636b-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="5636b-107">**Öppna med Utforskaren** är inte tillgänglig i den moderna upplevelsen för SharePoint-bibliotek.</span><span class="sxs-lookup"><span data-stu-id="5636b-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="5636b-108">Använd **Visa i Utforskaren** i stället.</span><span class="sxs-lookup"><span data-stu-id="5636b-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="5636b-109">Välj **Visa alternativ** \> **i Utforskaren**.</span><span class="sxs-lookup"><span data-stu-id="5636b-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="5636b-110">Visa i Utforskaren är inte kompatibel med Microsoft Edge, Google Chrome, Firefox och andra.</span><span class="sxs-lookup"><span data-stu-id="5636b-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="5636b-111">**Visa i Utforskaren** i endast tillgänglig i Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="5636b-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="5636b-112">Kontrollera att WebClient-tjänsten körs.</span><span class="sxs-lookup"><span data-stu-id="5636b-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="5636b-113">I Windows-sökrutan skriver du kör, väljer Kör skrivbordsapp, skriver Services. msc och trycker på RETUR.</span><span class="sxs-lookup"><span data-stu-id="5636b-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="5636b-114">Rulla ned till WebClient-tjänsten och kontrollera att kolumnen **status** visar "löpning".</span><span class="sxs-lookup"><span data-stu-id="5636b-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="5636b-115">Om den inte gör det dubbelklickar du på tjänsten, klickar på **Start**och sedan på **OK**.</span><span class="sxs-lookup"><span data-stu-id="5636b-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="5636b-116">(Du måste kanske först aktivera tjänsten genom att välja antingen **manuell** eller **Automatisk** i rutan **Startmetod** .)</span><span class="sxs-lookup"><span data-stu-id="5636b-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="5636b-117">Att öppna ett bibliotek i Utforskaren är praktiskt om du behöver kopiera eller flytta flera filer och mappar en gång, men om du vill arbeta regelbundet i biblioteket rekommenderar vi att du synkroniserar den.</span><span class="sxs-lookup"><span data-stu-id="5636b-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="5636b-118">Om du vill felsöka problem med att öppna i Utforskaren, se [Öppna i Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="5636b-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="5636b-119">Information om hur du konfigurerar synkronisering finns [i Synka SharePoint-filer med den nya OneDrive-synkroniseringsklienten](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="5636b-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="5636b-120">Se artikeln [hur du använder kommandot "öppna med Utforskaren" för att felsöka problem i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) för mer information.</span><span class="sxs-lookup"><span data-stu-id="5636b-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

