---
title: Prestanda problem-SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771262"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive långsamt, otillgängligt eller inte tillgängligt för flera användare

Om en OneDrive-eller SharePoint-webbplats inte är tillgänglig för flera användare som tidigare hade åtkomst kan det finnas ett tillfälligt tjänst problem. [Kontrol lera instrument panelen för tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth).

**Lägga till och licensiera användaren**

Se till att [tilldela licenser till användare i Microsoft 365 för företag](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Tilldela behörigheter**

Om användaren har tilldelats en SharePoint-licens och fortfarande får ett meddelande om nekad åtkomst bör du kontrol lera att de har [rätt behörighets nivå](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .

**Överväg att använda funktionen för åtkomstbegäran**

Med [funktionen](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) åtkomstbegäran kan användarna begära åtkomst till innehåll som de inte har behörighet att se.

**Tillåt anpassat skript kan orsaka problem med åtkomst nekande**

Det finns vissa scenarier där funktionen för *att tillåta anpassade skript* kan visa upp en åtkomst nekad. En lista över de funktioner som påverkas finns i säkerhets aspekter och möjligheten att inaktivera funktionen. Gå till [Tillåt eller förhindra anpassat skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

