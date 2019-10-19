---
title: Profilsynkronisering
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554351"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="86289-102">När synkroniseras min profil ändras till SharePoint-användarprofilprogrammet?</span><span class="sxs-lookup"><span data-stu-id="86289-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="86289-103">SharePoint Online använder det tidsinställda jobbet i Active Directory-import (AD-import) för att importera användare och grupper till användar profils programmet.</span><span class="sxs-lookup"><span data-stu-id="86289-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="86289-104">AD import synkroniserar ändringar från SharePoint Online Directory Store till användarprofilprogrammet.</span><span class="sxs-lookup"><span data-stu-id="86289-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="86289-105">Dessa ändringar bearbetas i batchar.</span><span class="sxs-lookup"><span data-stu-id="86289-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="86289-106">Det tidsinställda jobbet körs tills ändringarna synkroniseras.</span><span class="sxs-lookup"><span data-stu-id="86289-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="86289-107">Den tid det tar att köra jobbet beror på antalet ändringar i processen.</span><span class="sxs-lookup"><span data-stu-id="86289-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="86289-108">Ett stort antal förändringar tar längre tid.</span><span class="sxs-lookup"><span data-stu-id="86289-108">A large number of changes takes longer.</span></span> <span data-ttu-id="86289-109">Servicenivåavtalet (SLA) anger att en ändring av en användare i SharePoint online-katalogen kommer att återspeglas i användarprofilens program inom 24 timmar.</span><span class="sxs-lookup"><span data-stu-id="86289-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="86289-110">Mer information om synkronisering av användarprofil i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="86289-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

