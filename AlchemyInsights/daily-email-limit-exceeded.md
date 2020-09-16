---
title: Daglig e-postgräns har överskridits. Arbets flödet är inaktiverat.
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
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731581"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Daglig e-postgräns har överskridits. Arbets flödet är inaktiverat.

Det här felet kan tas emot i följande fall:

- Du har ett arbets flöde i SharePoint Online som använder plattforms typen SharePoint 2010 eller SharePoint 2013 Workflow Platform.
- Arbets flödet är konfigurerat för att skicka ett anpassat e-postmeddelande till fler än 200 användare åt gången, mer än 10 000 mottagare per dag eller mer än 30 meddelanden per minut.
- När du kör arbets flödet skickas inte e-postmeddelandet och du märker följande:
    - För ett arbets flöde som använder SharePoint 2013-plattforms typen bläddrar du till sidan **arbets flödes status** . På sidan arbets flödes status är den **interna statusen** inaktive rad och informations ballongen **visar att** **det inte går att skicka till en mottagare**.

Undvik det här problemet genom att konfigurera arbets flödet för att skicka e-postmeddelanden utan att överskrida [avsändarenas gränser för Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Du kan till exempel använda en paus i arbets flödet och skicka e-postmeddelandet till en Microsoft 365-grupp, en distributions grupp eller en e-postaktive rad säkerhets grupp eller skicka meddelandet till färre än 200 mottagare åt gången.


Mer information finns i följande [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Relaterade ämnen
- [Skapa flöde](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint och flöde](https://flow.microsoft.com/blog/sharepoint-and-flow/) 