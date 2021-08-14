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
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923662"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>När synkroniseras mina profiländringar till SharePoint-profilprogrammet?

SharePoint Online använder det tidsinställda jobbet för import av Active Directory (AD Import) för att importera användare och grupper till användarprofilprogrammet. 
  
1. AD-import synkroniserar ändringar från SharePoint Online Directory Store till användarprofilprogrammet. Dessa ändringar bearbetas i grupper.
    
2. Tidsinställt jobb körs tills ändringarna har synkroniserats.
    
> [!NOTE]
> Hur lång tid det tar att köra jobbet beror på antalet ändringar som ska bearbetas. Ett stort antal ändringar tar längre tid. SLA (Service Level Agreement) innebär att en ändring av en användare i SharePoint Online-katalogen återspeglas i användarprofilprogrammet inom 24 timmar. 
  
[Mer information om synkronisering av användarprofiler i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

