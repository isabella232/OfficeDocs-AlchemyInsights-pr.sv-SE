---
title: Återställa en borttagen webbplats
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: edf851da951e163f30660d524049abe0798a8314
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048814"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="df9e8-102">Återställa en borttagen webbplats</span><span class="sxs-lookup"><span data-stu-id="df9e8-102">Restore a deleted site</span></span>

<span data-ttu-id="df9e8-103">När en administratör tar bort en SharePoint-webbplats placeras den i papperskorgen för webbplatssamlingen, där den sparas i 93 dagar innan den tas bort permanent.</span><span class="sxs-lookup"><span data-stu-id="df9e8-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="df9e8-104">Så här återställer du webbplatsen:</span><span class="sxs-lookup"><span data-stu-id="df9e8-104">To restore the site:</span></span>
  
1. <span data-ttu-id="df9e8-105">I det nya administrationscentret för SharePoint klickar du på **papperskorgen** i menyfliksområdet.</span><span class="sxs-lookup"><span data-stu-id="df9e8-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="df9e8-106">Markera kryssrutan bredvid den webbplatssamling som du vill återställa.</span><span class="sxs-lookup"><span data-stu-id="df9e8-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="df9e8-107">Klicka på **Återställ borttagna objekt**.</span><span class="sxs-lookup"><span data-stu-id="df9e8-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="df9e8-108">Om du vill återställa en borttagen kommunikations plats kan du använda det nya administrationscentret för SharePoint.</span><span class="sxs-lookup"><span data-stu-id="df9e8-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="df9e8-109">I annat fall måste du använda Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="df9e8-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="df9e8-110">Om du vill återställa en webbplats som tillhör en Office 365-grupp måste du återställa gruppen i Exchange administratörscenter.</span><span class="sxs-lookup"><span data-stu-id="df9e8-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="df9e8-111">Grupper kan återställas i 30 dagar efter att de har raderats.</span><span class="sxs-lookup"><span data-stu-id="df9e8-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

