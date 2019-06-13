---
title: Åtkomst nekad när du visar ett arbetsflöde
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: b7a3805d30cac44781adbbb00c0f0ed3496ff17b
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/12/2019
ms.locfileid: "34883609"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Åtkomst nekad när du visar ett arbetsflöde

Arbetsflöden för SharePoint 2013 som försöker skicka ett e-postmeddelande till en SharePoint-grupp kan misslyckas med felmeddelandet ”åtkomst nekad” om medlemskap i SharePoint-gruppen inte har angetts för alla.
  
 **Lös problemet genom att utföra de här stegen:**
  
 1. Kan alla se medlemmarna i SharePoint-gruppen.
  
 2. Ta bort SharePoint-gruppen från rutan till eller kopia raden i e-postmeddelandet.
  
 3. Lägga till användare i till eller kopia uttryckligen rad om medlemskap synligheten inte kan ändras för SharePoint-grupp.
  
Om du vill visa finns mer information i [Http-obehörig till /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  