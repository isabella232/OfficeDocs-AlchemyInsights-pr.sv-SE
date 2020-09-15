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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>När synkroniserar profil ändringarna till användar profil programmet för SharePoint?

SharePoint Online använder det tidsinställda Active Directory import-jobbet (AD-import) för att importera användare och grupper till användar profil programmet. 
  
1. AD import-synkroniseringar ändras från SharePoint online-katalogen till användar profil programmet. Dessa ändringar bearbetas i batchar.
    
2. Det tidsinställda jobbet körs tills ändringarna synkroniseras.
    
> [!NOTE]
> Hur lång tid det tar att köra jobbet beror på antalet ändringar i processen. Ett stort antal ändringar tar längre tid. Service nivå avtalet (SLA) anger att en ändring av en användare i SharePoint online-katalogen återspeglas i användar profil programmet inom 24 timmar. 
  
[Mer information om synkronisering av användar profiler i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

