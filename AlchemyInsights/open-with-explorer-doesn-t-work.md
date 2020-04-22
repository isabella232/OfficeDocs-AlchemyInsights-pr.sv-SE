---
title: Öppna med Explorer fungerar inte
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713052"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="19eba-102">Öppna med Explorer fungerar inte</span><span class="sxs-lookup"><span data-stu-id="19eba-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="19eba-103">Om **Öppna med Utforskaren** eller **Visa i Utforskaren** inte fungerar kontrollerar du att WebClient-tjänsten är inställd **på Kör** genom att följa stegen nedan.</span><span class="sxs-lookup"><span data-stu-id="19eba-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="19eba-104">Det kan till exempel ta lång tid att öppna ett SharePoint- eller OneDrive-bibliotek när tjänsten inte körs.</span><span class="sxs-lookup"><span data-stu-id="19eba-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="19eba-105">Skriv kör i sökrutan i Windows, välj appen Kör skrivbord, skriv services.msc och välj sedan **Retur**.</span><span class="sxs-lookup"><span data-stu-id="19eba-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="19eba-106">Bläddra ned till WebClient-tjänsten och kontrollera kolumnen **Status.**</span><span class="sxs-lookup"><span data-stu-id="19eba-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="19eba-107">Om WebClient-tjänstens status inte **körs**dubbelklickar du på Tjänsten, klickar på **Start**och sedan på **OK**.</span><span class="sxs-lookup"><span data-stu-id="19eba-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="19eba-108">Aktivera tjänsten om det behövs genom att välja **manuell** eller **automatisk** i rutan **Starttyp.**</span><span class="sxs-lookup"><span data-stu-id="19eba-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="19eba-109">Mer om du vill felsöka problem som öppnas i Utforskaren finns [i Öppna i Utforskaren](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="19eba-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="19eba-110">Utforska synkronisering som ett bättre alternativ: [Synkronisera SharePoint-filer med den nya OneDrive-synkroniseringsklienten](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="19eba-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

