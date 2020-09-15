---
title: Felsöka problem med öppna med Utforskaren
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659076"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="fd4e4-102">Åtgärda problem med öppna med Utforskaren</span><span class="sxs-lookup"><span data-stu-id="fd4e4-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="fd4e4-103">Åtgärda vanliga problem med att öppna ett dokument bibliotek i SharePoint eller OneDrive med kommandot **Öppna med Utforskaren** :</span><span class="sxs-lookup"><span data-stu-id="fd4e4-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="fd4e4-104">Använd Internet Explorer 10 eller Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="fd4e4-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="fd4e4-105">**Öppna med Utforskaren** är inte kompatibelt med Microsoft Edge, Google Chrome, Firefox och andra.</span><span class="sxs-lookup"><span data-stu-id="fd4e4-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="fd4e4-106">**Öppna med Utforskaren** är inaktiverat i alla webbläsare utom Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="fd4e4-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="fd4e4-107">**Öppna med Utforskaren** är inte tillgängligt i den moderna versionen för SharePoint-bibliotek.</span><span class="sxs-lookup"><span data-stu-id="fd4e4-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="fd4e4-108">Använd **Visa i Utforskaren** i stället.</span><span class="sxs-lookup"><span data-stu-id="fd4e4-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="fd4e4-109">Välj vyn **visnings alternativ** \> **i Utforskaren**.</span><span class="sxs-lookup"><span data-stu-id="fd4e4-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="fd4e4-110">Visa i Utforskaren är inte kompatibelt med Microsoft Edge, Google Chrome, Firefox och andra.</span><span class="sxs-lookup"><span data-stu-id="fd4e4-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="fd4e4-111">**Visa i Utforskaren** i endast tillgänglig i Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="fd4e4-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="fd4e4-112">Kontrol lera att WebClient-tjänsten körs.</span><span class="sxs-lookup"><span data-stu-id="fd4e4-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="fd4e4-113">Skriv kör i sökrutan i Windows, välj Kör Skriv bords programmet, Skriv Services. msc och tryck sedan på RETUR.</span><span class="sxs-lookup"><span data-stu-id="fd4e4-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="fd4e4-114">Bläddra ned till WebClient-tjänsten och kontrol lera att kolumnen **status** visar "kör".</span><span class="sxs-lookup"><span data-stu-id="fd4e4-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="fd4e4-115">Om det inte gör det dubbelklickar du på tjänsten, klickar på **Start**och sedan på **OK**.</span><span class="sxs-lookup"><span data-stu-id="fd4e4-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="fd4e4-116">(Du kanske måste aktivera tjänsten först genom att välja antingen **manuell** eller **Automatisk** i rutan **Start metod** .)</span><span class="sxs-lookup"><span data-stu-id="fd4e4-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="fd4e4-117">Det är praktiskt att öppna ett bibliotek i Utforskaren om du behöver kopiera eller flytta flera filer och mappar en gång, men om du ofta vill arbeta i biblioteket rekommenderar vi att du synkroniserar det.</span><span class="sxs-lookup"><span data-stu-id="fd4e4-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="fd4e4-118">Information om hur du felsöker problem med öppning i Utforskaren finns i [Öppna i Utforskaren](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="fd4e4-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="fd4e4-119">Information om hur du konfigurerar synkronisering finns i [Synkronisera SharePoint-filer med den nya synkroniseringsklienten för OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="fd4e4-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="fd4e4-120">Mer information finns i artikeln om [hur du använder kommandot "öppna med Utforskaren" för att felsöka problem i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) .</span><span class="sxs-lookup"><span data-stu-id="fd4e4-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

