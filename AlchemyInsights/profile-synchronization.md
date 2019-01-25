---
title: Synkronisering av användarprofil
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492698"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="223c4-102">När min profil ändringar synkroniseras med SharePoint användarprofilprogrammet?</span><span class="sxs-lookup"><span data-stu-id="223c4-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="223c4-103">SharePoint Online använder Active Directory Import tidsinställt jobb (AD-Import) för att importera användare och grupper till användarprofilprogrammet.</span><span class="sxs-lookup"><span data-stu-id="223c4-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="223c4-p101">AD-Import synkroniserar ändringar från SharePoint Online-katalogdatabasen användarprofilprogrammet. Ändringarna bearbetas i batchar.</span><span class="sxs-lookup"><span data-stu-id="223c4-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="223c4-106">Det tidsinställda jobbet körs tills ändringarna synkroniseras.</span><span class="sxs-lookup"><span data-stu-id="223c4-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="223c4-p102">Den tid det tar att jobbet ska köras beror på antalet ändringar att bearbeta. Ett stort antal ändringar tar längre tid. Service Level (SLA) anger att en ändring till en användare i en SharePoint Online-katalogen kommer att återspeglas i användarprofilprogrammet i 24 timmar.</span><span class="sxs-lookup"><span data-stu-id="223c4-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="223c4-110">Mer information om synkronisering av användarprofiler i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="223c4-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

