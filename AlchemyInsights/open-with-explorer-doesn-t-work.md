---
title: Öppna i Explorer fungerar inte
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29491817"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="f47e2-102">Öppna i Explorer fungerar inte</span><span class="sxs-lookup"><span data-stu-id="f47e2-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="f47e2-p101">Om **Öppna med Utforskaren** eller **Visa i File Explorer** inte fungerar kontrollerar du att WebClient-tjänsten är inställd på **Kör** genom att följa stegen nedan. Till exempel kan det ta lång tid att öppna ett bibliotek i SharePoint eller OneDrive när tjänsten inte körs.</span><span class="sxs-lookup"><span data-stu-id="f47e2-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="f47e2-105">I rutan Sök i Windows typ kör, Välj Kör stationär app, typ services.msc och välj sedan **RETUR**.</span><span class="sxs-lookup"><span data-stu-id="f47e2-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="f47e2-p102">Rulla ned till WebClient-tjänsten och kontrollera kolumnen **Status** . Om **status för WebClient-tjänsten inte körs,** Dubbelklicka på tjänsten, klicka på **Start**och klicka sedan på **OK**. Aktivera tjänsten, vid behov genom att välja **Manuell** eller **automatisk** i rutan **Startmetod** .</span><span class="sxs-lookup"><span data-stu-id="f47e2-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="f47e2-p103">Felsökning av problem med öppna i File Explorer finns i [Öppna i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Utforska synkronisering som ett bättre alternativ: [synkronisera SharePoint-filer med den nya OneDrive sync-klienten](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="f47e2-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

