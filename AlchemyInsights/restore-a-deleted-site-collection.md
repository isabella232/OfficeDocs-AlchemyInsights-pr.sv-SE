---
title: Återställa en borttagen webbplatssamling
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: b3c72033dfcc093dd0c2837d2866c6a78d64449c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29491879"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="de064-102">Återställa en borttagen webbplatssamling</span><span class="sxs-lookup"><span data-stu-id="de064-102">Restore a deleted site collection</span></span>

<span data-ttu-id="de064-p101">När en administratör tar bort en klassisk webbplatssamling, placeras den i webbplatssamlingens papperskorg där det hålls för 93 dagar innan den tas bort permanent. Att återställa webbplatssamlingen:</span><span class="sxs-lookup"><span data-stu-id="de064-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="de064-105">Klicka på **Papperskorgen** på menyfliken i klassiska SharePoint administratörscenter.</span><span class="sxs-lookup"><span data-stu-id="de064-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="de064-106">Markera kryssrutan bredvid den webbplatssamling som du vill återställa.</span><span class="sxs-lookup"><span data-stu-id="de064-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="de064-107">Klicka på **Återställ borttagna objekt**.</span><span class="sxs-lookup"><span data-stu-id="de064-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="de064-p102">Du kan använda nya SharePoint admin center förhandsgranskning om du vill återställa ett borttaget meddelande webbplats. I annat fall måste du använda PowerShell. Om du vill återställa en webbplats som tillhör en grupp av Office 365, måste du återställa gruppen i Exchange administratörscenter. Grupper kan återställas i 30 dagar efter att de har tagits bort.</span><span class="sxs-lookup"><span data-stu-id="de064-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  

