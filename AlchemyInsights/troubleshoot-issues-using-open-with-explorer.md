---
title: Felsöka problem med Öppna med Utforskaren
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759710"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="50f64-102">Åtgärda problem med Öppna med Utforskaren</span><span class="sxs-lookup"><span data-stu-id="50f64-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="50f64-103">Åtgärda vanliga problem med att öppna ett dokumentbibliotek i SharePoint eller OneDrive med kommandot **Öppna med Utforskaren:**</span><span class="sxs-lookup"><span data-stu-id="50f64-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="50f64-104">Använda Internet Explorer 10 eller Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="50f64-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="50f64-105">**Öppna med Explorer** är inte kompatibelt med Microsoft Edge, Google Chrome, Firefox och andra.</span><span class="sxs-lookup"><span data-stu-id="50f64-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="50f64-106">**Öppna med Explorer** är inaktiverat i alla webbläsare utom Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="50f64-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="50f64-107">Det går inte att **öppna med Utforskaren** i den moderna upplevelsen för SharePoint-bibliotek.</span><span class="sxs-lookup"><span data-stu-id="50f64-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="50f64-108">Använd **Visa i Utforskaren i** stället.</span><span class="sxs-lookup"><span data-stu-id="50f64-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="50f64-109">Välj **Visa alternativ** \> **Visa i Utforskaren**.</span><span class="sxs-lookup"><span data-stu-id="50f64-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="50f64-110">Visa i Utforskaren är inte kompatibel med Microsoft Edge, Google Chrome, Firefox och andra.</span><span class="sxs-lookup"><span data-stu-id="50f64-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="50f64-111">**Visa i Utforskaren** endast tillgängligt i Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="50f64-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="50f64-112">Kontrollera att WebClient-tjänsten körs.</span><span class="sxs-lookup"><span data-stu-id="50f64-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="50f64-113">Skriv kör i sökrutan i Windows, välj appen Kör skrivbord, skriv services.msc och tryck sedan på Retur.</span><span class="sxs-lookup"><span data-stu-id="50f64-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="50f64-114">Bläddra ned till WebClient-tjänsten och se till att **kolumnen Status** visar "Körs".</span><span class="sxs-lookup"><span data-stu-id="50f64-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="50f64-115">Om den inte gör det dubbelklickar du på tjänsten, klickar på **Start**och sedan på **OK**.</span><span class="sxs-lookup"><span data-stu-id="50f64-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="50f64-116">(Du kan behöva aktivera tjänsten först genom att välja **Manuell** eller **Automatisk** i rutan **Starttyp.)**</span><span class="sxs-lookup"><span data-stu-id="50f64-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="50f64-117">Det är praktiskt att öppna ett bibliotek i Utforskaren om du behöver kopiera eller flytta flera filer och mappar en gång, men om du vill arbeta regelbundet i biblioteket rekommenderar vi att du synkroniserar det.</span><span class="sxs-lookup"><span data-stu-id="50f64-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="50f64-118">Mer om du vill felsöka problem som öppnas i Utforskaren finns [i Öppna i Utforskaren](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="50f64-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="50f64-119">Information om hur du konfigurerar synkronisering finns i [Synkronisera SharePoint-filer med den nya OneDrive-synkroniseringsklienten](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="50f64-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="50f64-120">Mer information finns i artikeln [Så här använder du kommandot "Öppna med Utforskaren" för att felsöka problem i SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)</span><span class="sxs-lookup"><span data-stu-id="50f64-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

