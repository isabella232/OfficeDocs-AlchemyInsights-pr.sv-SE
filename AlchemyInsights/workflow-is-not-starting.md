---
title: Arbetsflödet startar inte
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738107"
---
# <a name="workflow-is-not-starting"></a>Arbetsflödet startar inte

- SharePoint 2010 och SharePoint 2013 arbetsflöden startar inte.

    - Om ditt arbetsflöde inte startar kan det finnas ett tillfälligt tjänstproblem där användare kan drabbas av återkommande fördröjningar med arbetsflödes förloppet. Kontrollera den [service Health instrumentpanelen](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) för att se om din organisation påverkas.

    - Om mer än 24 timmar har gått sedan du först såg detta problem, vänligen logga ett supportärende. I många fall arbetar vi redan på en lösning. Vänligen ge oss minst 24 timmar för att slutföra en lösning.

- SharePoint 2010 arbetsflöden fördröjs på Start.

    - Detta inträffar om arbetsflödet utlöses i stora partier. (till exempel när flera objekt läggs till på en gång).

    - Arbetsflöden är inte utformade för att köras i realtid, så en fördröjning är avsiktligt beteende.

   -  Om arbetsflödet är komplext Extensible Object Markup Language (XMOL), kan kompilering vara långsam. Kontrollera [den här](https://support.microsoft.com//kb/3043697) artikeln.

    - Du bör förenkla arbetsflödet eller omforma det med hjälp av Microsoft SharePoint 2013 arbetsflödestypen plattform.

    - Om arbetsflödeshistoriken har blivit stor kanske du vill rensa objekten eller skapa en ny historiklista.

        Mer information: [Rensa arbetsflödeshistoriken](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Relaterade ämnen
Vill du prova Microsoft Flow i SharePoint Online?
- [Skapa flöde](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint och Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


