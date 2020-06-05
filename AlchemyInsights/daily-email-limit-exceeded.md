---
title: Den dagliga e-postgränsen har överskridits. Arbetsflödet är pausat.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580351"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Den dagliga e-postgränsen har överskridits. Arbetsflödet är pausat.

Det här felet kan tas emot i följande scenarier:

- Du har ett arbetsflöde i SharePoint Online som använder typen SharePoint 2010 eller SharePoint 2013.You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform platform type.
- Arbetsflödet är konfigurerat för att skicka ett anpassat e-postmeddelande till fler än 200 användare åt gången, fler än 10 000 mottagare per dag eller fler än 30 meddelanden per minut.
- När du kör arbetsflödet skickas inte e-postmeddelandet och du märker följande:
    - Om du vill ha ett arbetsflöde med typen SharePoint 2013-plattform bläddrar du till sidan **Arbetsflödesstatus.** På sidan Arbetsflödesstatus är den **interna statusen** inställd på **Startad**och informationsbubblan visar **det inte går att skicka till en mottagare**.

Du kan lösa problemet genom att konfigurera arbetsflödet så att det skickar e-postmeddelanden utan att [överskrida exchange online-avsändningsgränserna](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Använd till exempel en paus i arbetsflödet, skicka e-postmeddelandet till en Microsoft 365-grupp, en distributionsgrupp eller en e-postaktiverad säkerhetsgrupp eller skicka meddelandet till färre än 200 mottagare åt gången.


Mer information finns i följande [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Relaterade ämnen
- [Skapa flöde](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint och flöde](https://flow.microsoft.com/blog/sharepoint-and-flow/) 