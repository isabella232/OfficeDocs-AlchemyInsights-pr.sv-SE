---
title: Arbetsflödet startar inte
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403761"
---
# <a name="workflow-is-not-starting"></a>Arbetsflödet startar inte

- SharePoint 2010- och SharePoint 2013-arbetsflödena startar inte.

    - Om arbetsflödet inte startar kan det finnas ett tillfälligt tjänstproblem där användarna kan uppleva oregelbundna fördröjningar av arbetsflödets förlopp. Titta på [instrumentpanelen för](https://admin.microsoft.com/AdminPortal/Home/servicehealth) tjänstens hälsa för att se om din organisation påverkas.

    - Om det har gått mer än 24 timmar sedan problemet sågs för första gången ska du logga ett supportmeddelande. I många fall arbetar vi redan på en lösning. Ge oss minst 24 timmar för att slutföra en lösning.

- SharePoint 2010-arbetsflöden fördröjs vid start.

    - Detta inträffar om arbetsflödet utlöses i stora batchar. (Till exempel när flera objekt läggs till samtidigt).

    - Arbetsflöden är inte utformade för att köras i realtid, så en fördröjning beror på designbeteendet.

   -  Om arbetsflödet är komplext XMOL (Extensible Object Markup Language) kan kompileringen vara långsam. Läs [den här](https://support.microsoft.com//kb/3043697) artikeln.

    - Du bör förenkla arbetsflödet eller omarbeta det med microsoft SharePoint 2013-arbetsflödesplattformtypen.

    - Om arbetsflödeshistoriken har blivit stor kanske du vill rensa objekten eller skapa en ny historiklista.

        Mer information: [Rensa arbetsflödeshistorik](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Relaterade ämnen
Vill du prova Microsoft Flow i SharePoint Online?
- [Skapa flöde](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint och Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
