---
title: Öppna med Utforskaren fungerar inte
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694474"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="6d646-102">Öppna med Utforskaren fungerar inte</span><span class="sxs-lookup"><span data-stu-id="6d646-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="6d646-103">Om **Öppna med Utforskaren** eller **vyn i Utforskaren** inte fungerar kontrollerar du att WebClient-tjänsten är inställd på att **köras** genom att följa stegen nedan.</span><span class="sxs-lookup"><span data-stu-id="6d646-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="6d646-104">Det kan ta lång tid att öppna ett SharePoint-eller OneDrive-bibliotek när tjänsten inte körs.</span><span class="sxs-lookup"><span data-stu-id="6d646-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="6d646-105">Skriv kör i sökrutan i Windows, välj Kör Skriv bords programmet, Skriv Services. msc och välj sedan **RETUR**.</span><span class="sxs-lookup"><span data-stu-id="6d646-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="6d646-106">Bläddra ned till WebClient-tjänsten och kontrol lera kolumnen **status** .</span><span class="sxs-lookup"><span data-stu-id="6d646-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="6d646-107">Om WebClient-tjänstens status inte **körs**dubbelklickar du på tjänsten, klickar på **Start**och sedan på **OK**.</span><span class="sxs-lookup"><span data-stu-id="6d646-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="6d646-108">Aktivera tjänsten, om det behövs genom att välja **manuellt** eller **automatiskt** i rutan **Start** .</span><span class="sxs-lookup"><span data-stu-id="6d646-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="6d646-109">Information om hur du felsöker problem med öppning i Utforskaren finns i [Öppna i Utforskaren](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="6d646-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="6d646-110">Utforska synkroniseringen som ett bättre alternativ: [Synkronisera SharePoint-filer med den nya synkroniseringsklienten för OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="6d646-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

