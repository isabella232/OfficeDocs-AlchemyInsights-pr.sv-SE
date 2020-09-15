---
title: Profilsynkronisering
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801787"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="5dc46-102">När synkroniserar profil ändringarna till användar profil programmet för SharePoint?</span><span class="sxs-lookup"><span data-stu-id="5dc46-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="5dc46-103">SharePoint Online använder det tidsinställda Active Directory import-jobbet (AD-import) för att importera användare och grupper till användar profil programmet.</span><span class="sxs-lookup"><span data-stu-id="5dc46-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="5dc46-104">AD import-synkroniseringar ändras från SharePoint online-katalogen till användar profil programmet.</span><span class="sxs-lookup"><span data-stu-id="5dc46-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="5dc46-105">Dessa ändringar bearbetas i batchar.</span><span class="sxs-lookup"><span data-stu-id="5dc46-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="5dc46-106">Det tidsinställda jobbet körs tills ändringarna synkroniseras.</span><span class="sxs-lookup"><span data-stu-id="5dc46-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="5dc46-107">Hur lång tid det tar att köra jobbet beror på antalet ändringar i processen.</span><span class="sxs-lookup"><span data-stu-id="5dc46-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="5dc46-108">Ett stort antal ändringar tar längre tid.</span><span class="sxs-lookup"><span data-stu-id="5dc46-108">A large number of changes takes longer.</span></span> <span data-ttu-id="5dc46-109">Service nivå avtalet (SLA) anger att en ändring av en användare i SharePoint online-katalogen återspeglas i användar profil programmet inom 24 timmar.</span><span class="sxs-lookup"><span data-stu-id="5dc46-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="5dc46-110">Mer information om synkronisering av användar profiler i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5dc46-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

