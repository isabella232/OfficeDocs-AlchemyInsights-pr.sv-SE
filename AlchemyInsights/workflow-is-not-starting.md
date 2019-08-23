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
ms.openlocfilehash: d4bfdb44c04eb6838f4a265e55a4873d14c78f6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558005"
---
# <a name="workflow-is-not-starting"></a>Arbetsflödet startar inte

- Arbetsflöden för SharePoint 2010 och SharePoint 2013 startar inte.

    - Om arbetsflödet inte startar, kan det finnas en tillfällig service problem där användare kan drabbas av återkommande förseningar med arbetsflödet. Kontrollera att [Tjänsten hälsa instrumentpanelen](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) för att se om din organisation påverkas.

    - Om mer än 24 timmar har gått sedan du först såg problemet, logga en biljett stöd. I många fall kan arbetar vi redan på en lösning. Ge oss minst 24 timmar att slutföra en lösning.

- SharePoint 2010 arbetsflöden fördröjda på start.

    - Detta inträffar om arbetsflödet ska utlösas i stora grupper. (till exempel när flera artiklar läggs till på en gång).

    - Arbetsflöden är inte avsett att köras i realtid, så att en fördröjning är avsiktlig beteende.

   -  Om arbetsflödet är komplexa Extensible Object Markup Language (XMOL), kan kompilering vara långsam. Kontrollera [den här](https://support.microsoft.com/en-us/kb/3043697) artikeln.

    - Du bör förenkla arbetsflödet eller modifiera den med hjälp av Microsoft SharePoint 2013 arbetsflöde-plattformstyp.

    - Om din arbetsflödeshistorik har blivit stort, kanske du vill rensa objekten eller skapa en ny historiklista.

        Mer Information: [Rensa arbetsflödeshistorik](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Relaterade ämnen
Vill du prova Microsoft Flow i SharePoint Online?
- [Skapa flöde](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint och flöde](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


