---
title: Arbetsflödet startar inte
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766115"
---
# <a name="workflow-is-not-starting"></a>Arbetsflödet startar inte

- SharePoint 2010- och SharePoint 2013-arbetsflöden startar inte.

    - Om arbetsflödet inte startar kan det finnas ett tillfälligt serviceproblem där användare kan uppleva återkommande fördröjningar med arbetsflödesförloppet. Kontrollera [instrumentpanelen](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) för tjänsthälsa för att se om din organisation påverkas.

    - Om det har gått mer än 24 timmar sedan du först såg det här problemet, vänligen logga en supportbiljett. I många fall arbetar vi redan på en lösning. Vänligen ge oss minst 24 timmar att slutföra en lösning.

- SharePoint 2010-arbetsflöden försenades vid start.

    - Detta inträffar om arbetsflödet utlöses i stora batchar. (till exempel när flera objekt läggs till samtidigt).

    - Arbetsflöden är inte utformade för att köras i realtid, så en fördröjning är avsiktligt beteende.

   -  Om arbetsflödet är komplext utökningsbart objektmarkeringsspråk (XMOL) kan kompileringen vara långsam. Läs [den här](https://support.microsoft.com//kb/3043697) artikeln.

    - Du bör förenkla arbetsflödet eller omforma det med hjälp av plattformstypen Microsoft SharePoint 2013 Workflow.

    - Om arbetsflödeshistoriken har blivit stor kanske du vill rensa objekten eller skapa en ny historiklista.

        Mer information : [Rensa arbetsflödeshistorik](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Relaterade ämnen
Vill du prova Microsoft Flow i SharePoint Online?
- [Skapa flöde](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint och flöde](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


