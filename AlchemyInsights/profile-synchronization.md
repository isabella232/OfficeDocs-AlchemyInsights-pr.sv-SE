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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>När min profil ändringar synkroniseras med SharePoint användarprofilprogrammet?

SharePoint Online använder Active Directory Import tidsinställt jobb (AD-Import) för att importera användare och grupper till användarprofilprogrammet. 
  
1. AD-Import synkroniserar ändringar från SharePoint Online-katalogdatabasen användarprofilprogrammet. Ändringarna bearbetas i batchar.
    
2. Det tidsinställda jobbet körs tills ändringarna synkroniseras.
    
> [!NOTE]
> Den tid det tar att jobbet ska köras beror på antalet ändringar att bearbeta. Ett stort antal ändringar tar längre tid. Service Level (SLA) anger att en ändring till en användare i en SharePoint Online-katalogen kommer att återspeglas i användarprofilprogrammet i 24 timmar. 
  
[Mer information om synkronisering av användarprofiler i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

