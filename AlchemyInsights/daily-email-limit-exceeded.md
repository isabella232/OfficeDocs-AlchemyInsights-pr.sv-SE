---
title: Den dagliga e-postgränsen har överskridits. Arbetsflödet är inaktiverat.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914669"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Överskriden daglig e-postgräns. Arbetsflödet är inaktiverat.

Det här felet kan tas emot i följande scenarier:

- Du har ett arbetsflöde i SharePoint Online som använder SharePoint 2010- SharePoint 2013-arbetsflödesplattformtypen.
- Arbetsflödet är konfigurerat för att skicka ett anpassat e-postmeddelande till fler än 200 användare i taget, fler än 10 000 mottagare per dag eller fler än 30 meddelanden per minut.
- När du kör arbetsflödet skickas inte e-postmeddelandet och du märker följande:
    - Om du vill skapa ett arbetsflöde SharePoint 2013-plattformstypen går du till **sidan Arbetsflödesstatus.** På sidan Arbetsflödesstatus är **intern status** inställd på Startad **och** informationsbubblan visar Det går inte att skicka till **en mottagare.**

Du kan komma runt det här problemet genom att konfigurera arbetsflödet så att e-postmeddelanden skickas [utan att Exchange Online gränsen för avsändare](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Du kan till exempel använda en paus i arbetsflödet, skicka e-postmeddelandet till en Microsoft 365-grupp, en distributionsgrupp eller e-postaktiverad säkerhetsgrupp, eller skicka meddelandet till färre än 200 mottagare i taget.


Mer information finns i följande [artikel.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Relaterade ämnen
- [Skapa Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint och Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 