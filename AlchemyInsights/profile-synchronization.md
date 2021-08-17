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
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320727"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>När synkroniseras mina profiländringar till SharePoint-profilprogrammet?

SharePoint Online använder det tidsinställda jobbet för import av Active Directory (AD Import) för att importera användare och grupper till användarprofilprogrammet. 
  
1. AD-import synkroniserar ändringar från SharePoint Online Directory Store till användarprofilprogrammet. Dessa ändringar bearbetas i grupper.
    
2. Tidsinställt jobb körs tills ändringarna har synkroniserats.
    
**Obs!** Den tid det tar att köra jobbet beror på antalet ändringar som ska bearbetas. Ett stort antal ändringar tar längre tid. Tjänstnivåavtalet (SLA) innebär att en ändring av en användare i SharePoint Online-katalogen återspeglas i användarprofilprogrammet inom 24 timmar. 
  
[Mer information om synkronisering av användarprofiler i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

