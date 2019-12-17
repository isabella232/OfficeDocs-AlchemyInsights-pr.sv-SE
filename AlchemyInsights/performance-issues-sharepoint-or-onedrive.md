---
title: Prestandaproblem-SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068438"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive är långsam, otillgänglig eller otillgänglig för flera användare

SharePoint eller OneDrive kan vara långsam, otillgänglig eller otillgänglig, eller kan visa tjänsten otillgänglig eller 503 fel, av flera anledningar:
  
- Om din SharePoint-eller OneDrive-webbplats är långsam eller försenad för flera användare kan det finnas ett tillfälligt tjänstproblem där användare drabbas av återkommande fördröjningar eller navigeringsfel vid åtkomst till SharePoint-webbplatser eller OneDrive-innehåll. Kontrollera den [service Health instrumentpanelen](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) för att se om din organisation påverkas.
  
- Användare kan få en *503 Server är upptagen* fel när du försöker navigera till SharePoint eller OneDrive webbplatser. Det här felet kan orsakas av begränsning i SharePoint-tjänsten. SharePoint Online använder begränsning för att bibehålla optimala prestanda och tillförlitlighet för SharePoint Online-tjänsten. Begränsning begränsar antalet användaråtgärder eller samtidiga anrop (med skript eller kod) för att förhindra överanvändning av resurser. Mer information om begränsning se, [undvika att få begränsas eller blockeras i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Om du upplever långsamma prestanda med en **klassisk** eller **modern** SharePoint-webbplats eller-sida använder du [diagnostikverktyget](https://aka.ms/perftool) för sidor för att analysera sidorna.
  
- Om du fortfarande upplever allmänt långsamma prestanda, granska resurserna längst ned i den här artikeln: [Introduktion till prestandajustering för SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  