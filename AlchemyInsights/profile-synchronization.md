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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>När synkroniseras mina profiländringar i SharePoint-användarprofilprogrammet?

SharePoint Online använder AD-importjobbet (AD Import) för att importera användare och grupper till programmet Användarprofil. 
  
1. AD Import synkroniserar ändringar från SharePoint Online Directory Store till användarprofilprogrammet. Dessa ändringar bearbetas i batchar.
    
2. Timerjobbet körs tills ändringarna synkroniseras.
    
> [!NOTE]
> Hur tid det tar för jobbet att köra beror på antalet ändringar som ska bearbetas. Ett stort antal ändringar tar längre tid. Service Level Agreement (SLA) anger att en ändring av en användare i SharePoint Online Directory kommer att återspeglas i användarprofilprogrammet om 24 timmar. 
  
[Mer information om synkronisering av användarprofiler i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

