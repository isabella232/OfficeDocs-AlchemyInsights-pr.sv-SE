---
title: Diagrammet visar olika antal poster i rutnätet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439961"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="ad9db-102">Diagrammet visar olika antal poster i rutnätet</span><span class="sxs-lookup"><span data-stu-id="ad9db-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="ad9db-103">**Symptom**</span><span class="sxs-lookup"><span data-stu-id="ad9db-103">**Symptom**</span></span>

<span data-ttu-id="ad9db-104">För diagram på instrumentpanelssidan, när du klickar på diagrammet "..." och klicka på "Visa poster", navigerar du till rutnätssidan för att se alla poster. Ibland ändras antalet poster.</span><span class="sxs-lookup"><span data-stu-id="ad9db-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="ad9db-105">**Orsak**</span><span class="sxs-lookup"><span data-stu-id="ad9db-105">**Cause**</span></span>

<span data-ttu-id="ad9db-106">Detta beror på skillnaden mellan vyerna mellan diagrammet på den ursprungliga instrumentpanelssidan och diagrammet på rutnätets startsida.</span><span class="sxs-lookup"><span data-stu-id="ad9db-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="ad9db-107">**Lösning**</span><span class="sxs-lookup"><span data-stu-id="ad9db-107">**Solution**</span></span>

1. <span data-ttu-id="ad9db-108">Kontrollera vyn från den ursprungliga sidan och vyn i rutnätet för att se om de är annorlunda.</span><span class="sxs-lookup"><span data-stu-id="ad9db-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="ad9db-109">Ändra vyn i rutnätet så att den matchar vyn på den ursprungliga sidan.</span><span class="sxs-lookup"><span data-stu-id="ad9db-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="ad9db-110">Om rätt vy inte kan hittas betyder det vanligtvis att vyn inte är aktiverad i appdesignern.</span><span class="sxs-lookup"><span data-stu-id="ad9db-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="ad9db-111">Gå till appdesignern för den specifika appen, välj entiteten och dess vyer, kontrollera den vy som du vill aktivera, spara, publicera och stänga.</span><span class="sxs-lookup"><span data-stu-id="ad9db-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="ad9db-112">Uppdatera sidan.</span><span class="sxs-lookup"><span data-stu-id="ad9db-112">Refresh the page.</span></span>