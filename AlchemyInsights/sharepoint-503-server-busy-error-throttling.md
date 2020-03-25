---
title: Begränsning av SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931244"
---
# <a name="sharepoint-online-throttling"></a>Begränsning av SharePoint Online

**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden. Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar. Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.

Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid. Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider. Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.

**503-servern är upptagen fel**

Användare kan få ett 503-server är upptaget när de försöker navigera till SharePoint- eller OneDrive-webbplatser. 

Det här felet kan orsakas av begränsning i SharePoint-tjänsten. SharePoint Online använder begränsning för att upprätthålla optimal prestanda och tillförlitlighet för SharePoint Online-tjänsten. Begränsning begränsar antalet användaråtgärder eller samtidiga anrop (med skript eller kod) för att förhindra överanvändning av resurser. 

Mer information om begränsning finns i [Undvik att bli begränsad eller blockerad i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Om du tror att det här felet inte har något samband med begränsningen kan du kontrollera om det finns aktivt underhåll på din klient genom att navigera till [meddelandecentret](https://portal.office.com/adminportal/home#/MessageCenter).

 Se slutligen till att du besöker sidan [Service Health](https://portal.office.com/adminportal/home#/servicehealth) för att kontrollera eventuella råd/incidenter som kan inträffa.

