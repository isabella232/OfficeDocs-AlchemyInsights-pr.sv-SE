---
title: Synkronisering av profiler
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768131"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="e0bf4-102">När synkroniseras mina profiländringar i SharePoint-användarprofilprogrammet?</span><span class="sxs-lookup"><span data-stu-id="e0bf4-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="e0bf4-103">SharePoint Online använder AD-importjobbet (AD Import) för att importera användare och grupper till programmet Användarprofil.</span><span class="sxs-lookup"><span data-stu-id="e0bf4-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="e0bf4-104">AD Import synkroniserar ändringar från SharePoint Online Directory Store till användarprofilprogrammet.</span><span class="sxs-lookup"><span data-stu-id="e0bf4-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="e0bf4-105">Dessa ändringar bearbetas i batchar.</span><span class="sxs-lookup"><span data-stu-id="e0bf4-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="e0bf4-106">Timerjobbet körs tills ändringarna synkroniseras.</span><span class="sxs-lookup"><span data-stu-id="e0bf4-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="e0bf4-107">Hur tid det tar för jobbet att köra beror på antalet ändringar som ska bearbetas.</span><span class="sxs-lookup"><span data-stu-id="e0bf4-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="e0bf4-108">Ett stort antal ändringar tar längre tid.</span><span class="sxs-lookup"><span data-stu-id="e0bf4-108">A large number of changes takes longer.</span></span> <span data-ttu-id="e0bf4-109">Service Level Agreement (SLA) anger att en ändring av en användare i SharePoint Online Directory kommer att återspeglas i användarprofilprogrammet om 24 timmar.</span><span class="sxs-lookup"><span data-stu-id="e0bf4-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="e0bf4-110">Mer information om synkronisering av användarprofiler i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="e0bf4-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

