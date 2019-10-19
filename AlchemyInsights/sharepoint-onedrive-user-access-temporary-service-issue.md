---
title: Prestandaproblem-SharePoint eller OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 7e218cfff81274cd16d55dec2c5243eb8b74a3b7
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750574"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive är långsam, otillgänglig eller otillgänglig för flera användare

Om en OneDrive eller SharePoint-webbplats inte är tillgänglig för flera användare som tidigare hade åtkomst, kan det finnas ett tillfälligt problem med tjänsten. [Kontrollera den service Health instrumentpanelen](https://portal.office.com/adminportal/home#/servicehealth).

**Lägg till och licensiera användaren**

Se till att du [tilldelar licenser till användare i Office 365 för företag](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


**Tilldela behörigheter**

Om användaren har tilldelats en SharePoint-licens och fortfarande får ett meddelande om nekad åtkomst, kontrollera att de har [rätt behörighetsnivå](https://docs.microsoft.com/sharepoint/understanding-permission-levels) tilldelad.

**Överväg att använda funktionen för åtkomstbegäran**

Med [funktionen för åtkomstbegäran](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) kan personer begära åtkomst till innehåll som de för närvarande inte har behörighet att se.

**Tillåt anpassade skript kan orsaka åtkomst nekad problem**

Det finns vissa scenarier där funktionen *Tillåt anpassade skript* kan utgöra en åtkomst nekad. En lista över funktioner som berörs, säkerhetsöverväganden och möjligheten att inaktivera funktionen. Besök [Tillåt eller förhindra anpassade skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

