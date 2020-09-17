---
title: Arbets flödet startar inte
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794785"
---
# <a name="workflow-is-not-starting"></a>Arbets flödet startar inte

- SharePoint 2010-och SharePoint 2013-arbets flöden startas inte.

    - Om arbets flödet inte startas kan det finnas ett tillfälligt tjänst problem där användarna kan uppleva fördröjningar med arbets flödes status. Kontrol lera [instrument panelen för tjänstens hälsa](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) för att se om din organisation påverkas.

    - Om det inte finns mer än 24 timmar sedan du först såg det här problemet, logga in ett support ärende. I många fall jobbar vi redan med en lösning. Ange minst 24 timmar för att slutföra en lösning.

- SharePoint 2010-arbets flöden fördröjs vid start.

    - Detta inträffar om arbets flödet utlöses i stora grupper. (när flera objekt läggs till samtidigt).

    - Arbets flöden är inte avsedda att köras i real tid, så en fördröjning är by-design.

   -  Om arbets flödet är ett komplext Extensible Object Markup Language (XMOL) kan kompileringen bli långsam. Kontrol lera [den här](https://support.microsoft.com//kb/3043697) artikeln.

    - Du bör förenkla arbets flödet eller omkonstruera det med hjälp av plattforms typen Microsoft SharePoint 2013 Workflow.

    - Om arbets flödes historiken är stor kanske du vill ta bort objekten eller skapa en ny historik lista.

        Mer information: [ta bort arbets flödes historik](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Relaterade ämnen
Vill du prova Microsoft Flow i SharePoint Online?
- [Skapa flöde](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint och flöde](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


