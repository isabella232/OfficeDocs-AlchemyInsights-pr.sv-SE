---
title: MC210173 – SharePoint Designer nytt anpassat formulär funktion utfasning
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831824"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 – SharePoint Designer nytt anpassat formulär funktion utfasning

Vi har identifierat ett problem som påverkar SharePoint Designer-funktionerna för [att skapa anpassade formulär](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) i SharePoint Online. Efter noggrann undersökning har vi fastställt att det inte finns någon känd lösning på problemet och valt att inaktivera funktionen för att skapa anpassade formulär effektivt fr. 3:00 AM UTC på lördag, 25 april 2020. Den här ändringen påverkar inte möjligheten att redigera tidigare skapade formulär och andra befintliga funktioner i SharePoint Online Designer.

När du har gjort det kan användarna få följande felmeddelande: "Det gick inte att spara liständringarna på servern" när du skapar nya formulär.

Användare som tidigare har använt SharePoint Designer för att skapa egna formulär kan i stället använda [PowerApps-](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) för det ändamålet.

PowerApps är ett enkelt och kraftfullt verktyg som gör det möjligt för användare i SharePoint Online Modern Experience att skapa och redigera anpassade formulär för SharePoint-listor och dokumentbibliotek direkt i ett webbläsarfönster. PowerApps kräver inte traditionella koder eller att kunna koda eller några andra nedladdningar av appar som InfoPath.

**Obs**: användare av SharePoint Online Classic kommer tillfälligt att behöva gå över till den moderna miljön för att få tillgång till och använda PowerApps; alla anpassade formulär som skapas i PowerApps är dock tillgängliga för användare av SharePoint Online Classic Experience.
