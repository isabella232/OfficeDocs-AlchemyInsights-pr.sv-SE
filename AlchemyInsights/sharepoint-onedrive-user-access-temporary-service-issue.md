---
title: Prestandaproblem-SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511166"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive långsamt, otillgängligt eller inte tillgängligt för flera användare

Om en OneDrive- eller SharePoint-webbplats inte är tillgänglig för flera användare som tidigare hade åtkomst kan det bero på ett tillfälligt serviceproblem. [Kontrollera instrumentpanelen för tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth).

**Lägga till och licensiera användaren**

Kontrollera att du [tilldelar licenser till användare i Microsoft 365 för företag](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Tilldela behörigheter**

Om användaren har tilldelats en Sharepoint-licens och fortfarande får ett meddelande om nekad åtkomst, se till att de har [rätt behörighetsnivå](https://docs.microsoft.com/sharepoint/understanding-permission-levels) tilldelad.

**Överväg att använda funktionen för åtkomstbegäran**

[Funktionen för åtkomstbegäran](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) gör det möjligt för personer att begära åtkomst till innehåll som de för närvarande inte har behörighet att se.

**Tillåt anpassade skript kan orsaka åtkomst nekade problem**

Det finns vissa scenarier där funktionen *Tillåt anpassat skript* kan presentera en åtkomst nekad. För en lista över funktioner som påverkas, säkerhetsöverväganden och möjligheten att inaktivera funktionen. Besök [Tillåt eller förhindra anpassat skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

