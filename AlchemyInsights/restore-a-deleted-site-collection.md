---
title: Återställa en borttagen webbplats
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692061"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="49752-102">Återställa en borttagen webbplats</span><span class="sxs-lookup"><span data-stu-id="49752-102">Restore a deleted site</span></span>

<span data-ttu-id="49752-103">När en administratör tar bort en SharePoint-webbplats placeras den i pappers korgen för webbplats samlingen, där den bevaras i 93 dagar innan den tas bort permanent.</span><span class="sxs-lookup"><span data-stu-id="49752-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="49752-104">Så här återställer du webbplatsen:</span><span class="sxs-lookup"><span data-stu-id="49752-104">To restore the site:</span></span>
  
1. <span data-ttu-id="49752-105">I det nya administrations centret för SharePoint klickar du på **pappers korgen** i menyfliksområdet.</span><span class="sxs-lookup"><span data-stu-id="49752-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="49752-106">Markera kryss rutan bredvid den webbplats samling du vill återställa.</span><span class="sxs-lookup"><span data-stu-id="49752-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="49752-107">Klicka på **Återställ borttagna objekt**.</span><span class="sxs-lookup"><span data-stu-id="49752-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="49752-108">Om du vill återställa en borttagen kommunikations webbplats kan du använda det nya administrations centret för SharePoint.</span><span class="sxs-lookup"><span data-stu-id="49752-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="49752-109">I annat fall måste du använda Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="49752-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="49752-110">Om du vill återställa en webbplats som tillhör en Microsoft 365-grupp måste du återställa gruppen i administrations centret för Exchange.</span><span class="sxs-lookup"><span data-stu-id="49752-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="49752-111">Grupper kan återställas i 30 dagar efter att de har tagits bort.</span><span class="sxs-lookup"><span data-stu-id="49752-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

