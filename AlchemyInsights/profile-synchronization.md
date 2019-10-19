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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>När synkroniseras min profil ändras till SharePoint-användarprofilprogrammet?

SharePoint Online använder det tidsinställda jobbet i Active Directory-import (AD-import) för att importera användare och grupper till användar profils programmet. 
  
1. AD import synkroniserar ändringar från SharePoint Online Directory Store till användarprofilprogrammet. Dessa ändringar bearbetas i batchar.
    
2. Det tidsinställda jobbet körs tills ändringarna synkroniseras.
    
> [!NOTE]
> Den tid det tar att köra jobbet beror på antalet ändringar i processen. Ett stort antal förändringar tar längre tid. Servicenivåavtalet (SLA) anger att en ändring av en användare i SharePoint online-katalogen kommer att återspeglas i användarprofilens program inom 24 timmar. 
  
[Mer information om synkronisering av användarprofil i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

