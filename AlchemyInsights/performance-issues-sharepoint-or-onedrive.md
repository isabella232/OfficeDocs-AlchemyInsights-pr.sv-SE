---
title: Prestandaproblem-SharePoint eller OneDrive
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
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911860"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive långsamt, otillgängligt eller otillgängligt för flera användare

SharePoint eller OneDrive vara långsamt, otillgängligt eller otillgängligt, eller kan visa fel om tjänsten inte är tillgänglig eller 503 av flera orsaker:
  
- Om din SharePoint- eller OneDrive-webbplats är långsam eller försenad för flera användare kan det finnas ett tillfälligt tjänstproblem där användarna upplever oregelbundna fördröjningar eller navigeringsfel när de öppnar SharePoint webbplatser eller OneDrive innehåll. Titta på [instrumentpanelen för](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) tjänstens hälsa för att se om din organisation påverkas.
  
- Användarna kan få *felmeddelandet 503 om att servern* är upptagen när de försöker SharePoint eller OneDrive webbplatser. Det här felet kan orsakas av begränsning inom SharePoint tjänsten. SharePoint Online använder begränsning för att bibehålla optimala prestanda och tillförlitlighet i SharePoint Online-tjänsten. Begränsningen begränsar antalet användaråtgärder och samtidiga anrop (med skript eller kod) för att förhindra att resurserna utnyttjas för mycket. Mer information om begränsning finns i Undvik [att begränsas eller blockeras i SharePoint Online.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Om du upplever långsam prestanda med en **klassisk** eller **modern** SharePoint webbplats eller sida använder du verktyget [Siddiagnostik för](https://aka.ms/perftool) att analysera sidorna.
  
- Om du fortfarande upplever generellt långsam prestanda kan du läsa resurserna längst ned i den här artikeln: Introduktion till [prestandajustering för SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  