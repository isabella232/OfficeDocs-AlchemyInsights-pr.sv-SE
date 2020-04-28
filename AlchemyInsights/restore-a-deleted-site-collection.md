---
title: Återställa en borttagen plats
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
ms.openlocfilehash: d37fd903c91c8cd6ac6137e815cb253f7edb4494
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912693"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="fed5f-102">Återställa en borttagen plats</span><span class="sxs-lookup"><span data-stu-id="fed5f-102">Restore a deleted site</span></span>

<span data-ttu-id="fed5f-103">När en administratör tar bort en SharePoint-webbplats placeras den i webbplatssamlingen Papperskorgen, där den sparas i 93 dagar innan den tas bort permanent.</span><span class="sxs-lookup"><span data-stu-id="fed5f-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="fed5f-104">Så här återställer du webbplatsen:</span><span class="sxs-lookup"><span data-stu-id="fed5f-104">To restore the site:</span></span>
  
1. <span data-ttu-id="fed5f-105">Klicka på Papperskorgen i menyfliksområdet i det nya **administrationscentret** för SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fed5f-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="fed5f-106">Markera kryssrutan bredvid den webbplatssamling som du vill återställa.</span><span class="sxs-lookup"><span data-stu-id="fed5f-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="fed5f-107">Klicka på **Återställ borttagna objekt**.</span><span class="sxs-lookup"><span data-stu-id="fed5f-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="fed5f-108">Om du vill återställa en borttagen kommunikationswebbplats kan du använda det nya Administrationscentret för SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fed5f-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="fed5f-109">Annars måste du använda Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fed5f-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="fed5f-110">Om du vill återställa en webbplats som tillhör en Microsoft 365-grupp måste du återställa gruppen i administrationscentret för Exchange.</span><span class="sxs-lookup"><span data-stu-id="fed5f-110">To restore a site that belongs to an Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="fed5f-111">Grupper kan återställas i 30 dagar efter att de har tagits bort.</span><span class="sxs-lookup"><span data-stu-id="fed5f-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

