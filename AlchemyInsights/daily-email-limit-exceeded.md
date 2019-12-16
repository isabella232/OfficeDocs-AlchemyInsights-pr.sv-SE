---
title: Daglig email gräns överskridat. Arbetsflödet är avstängt.
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
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053135"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Daglig email gräns överskridat. Arbetsflödet är avstängt.

Det här felet kan tas emot i följande scenarier:

- Du har ett arbetsflöde i SharePoint Online som använder den SharePoint 2010 eller SharePoint 2013 arbetsflödestyp plattform.
- Arbetsflödet har konfigurerats för att skicka ett anpassat e-postmeddelande till mer än 200 användare i taget, mer än 10 000 mottagare per dag eller mer än 30 meddelanden per minut.
- När du kör arbetsflödet e-postmeddelandet skickas inte och du märker följande beteende:
    - För ett arbetsflöde med plattforms typen SharePoint 2013 bläddrar du till sidan **arbetsflödes status** . På SidanArbetsflödesstatus är **intern status** inställd på **startad**och informationsbubblan **kan inte skickas till en mottagare**.

Undvik det här problemet genom att konfigurera arbetsflödet för att skicka e-postmeddelanden utan att överskrida [Exchange Online avsändar gränser](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Till exempel använda en paus i arbetsflödet, skicka e-postmeddelandet till en grupp för Office 365, en distributionsgrupp eller e-postaktiverade säkerhetsgruppen eller skicka meddelandet till färre än 200 mottagare i taget.


Mer information finns i följande [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Relaterade ämnen
- [Skapa flöde](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint och Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 