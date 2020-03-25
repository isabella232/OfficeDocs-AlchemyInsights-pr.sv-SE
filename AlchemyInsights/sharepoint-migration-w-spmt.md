---
title: SharePoint-migrering med SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931568"
---
# <a name="sharepoint-migration-with-spmt"></a>SharePoint-migrering med SPMT

**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden. Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar. Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.

Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid. Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider. Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.

**Migreringsverktyget för SharePoint**

SharePoint Migration Tool är utformat för migreringar som sträcker sig från den minsta uppsättningen filer till en storskalig företagsmigrering och gör att du kan överföra din information till molnet och dra nytta av det senaste samarbetet, intelligensen och säkerhetslösningar med Office 365.

- [Hämta och installera Verktyget för migrering i SharePoint](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [Felsöka vanliga SPMT-problem och fel](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [Felsöka problem med SPMT-installation](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
