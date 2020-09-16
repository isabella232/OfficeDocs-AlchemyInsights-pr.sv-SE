---
title: Prestanda problem-SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771919"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive långsamt, otillgängligt eller otillgängligt för flera användare

SharePoint eller OneDrive kan vara långsamt, otillgängliga eller otillgängliga eller kanske Visa tjänsten ej tillgänglig eller 503 fel, av olika anledningar:
  
- Om din SharePoint-eller OneDrive-webbplats är långsam eller fördröjd för flera användare kan det finnas ett tillfälligt tjänst problem där användarna upplever fördröjningar eller navigerings fel vid åtkomst till SharePoint-webbplatser eller OneDrive-innehåll. Kontrol lera [instrument panelen för tjänstens hälsa](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) för att se om din organisation påverkas.
  
- Användare kan få en *503-server att vara upptagen* när du försöker navigera till SharePoint-eller OneDrive-webbplatser. Det här felet kan orsakas av begränsning i SharePoint-tjänsten. SharePoint Online använder begränsning för att bibehålla optimala prestanda och tillförlitlighet i SharePoint Online-tjänsten. Begränsningen begränsar antalet användaråtgärder och samtidiga anrop (med skript eller kod) för att förhindra att resurserna utnyttjas för mycket. Mer information om begränsning finns i [undvika begränsning eller blockering i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Om du upplever låga prestanda med en **klassisk** eller **modern** SharePoint-webbplats eller-sida kan du använda [verktyget](https://aka.ms/perftool) för att analysera sidorna.
  
- Om du fortfarande upplever allmän långsam prestanda kan du gå igenom resurserna längst ned i den här artikeln: [Introduktion till prestanda justering för SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  