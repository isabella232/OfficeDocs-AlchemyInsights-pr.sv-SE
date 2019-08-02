---
title: Dagliga e-gränsen har överskridits. Arbetsflödet avbryts.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059656"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Dagliga e-gränsen har överskridits. Arbetsflödet avbryts.

Det här felet kan tas emot i följande scenarier:

- Du har ett arbetsflöde i SharePoint Online som använder SharePoint 2010 eller SharePoint 2013 arbetsflödestypen plattform.
- Arbetsflödet har konfigurerats för att skicka ett anpassat e-postmeddelande till mer än 200 användare i taget, mer än 10 000 mottagare per dag eller mer än 30 meddelanden per minut.
- När du kör arbetsflödet skickas inget e-postmeddelandet och följande inträffa:
    - För ett arbetsflöde som använder SharePoint 2013-plattformstyp, bläddra till sidan **Arbetsflödesstatus** . **Interna Status** har värdet **startad**och information pratbubbla visas **Det går inte att skicka till en mottagare**på sidan Arbetsflödesstatus.

Undvik det här problemet genom att konfigurera arbetsflödet om du vill skicka e-postmeddelanden utan att överskrida [gränserna för Exchange Online avsändaren](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Till exempel använder en paus i arbetsflödet, skicka e-postmeddelandet till en Office 365-grupp, en distributionsgrupp eller grupp med säkerhet aktiverat mail eller skicka meddelandet till färre än 200 mottagare samtidigt.


Mer information finns i följande [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Relaterade ämnen
- [Skapa flöde](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint och flöde](https://flow.microsoft.com/blog/sharepoint-and-flow/) 