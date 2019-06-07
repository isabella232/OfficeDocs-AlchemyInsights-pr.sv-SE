---
title: Prestanda problem-SharePoint eller OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 745a62c917c0b94501843332d70609261c6d3b76
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759168"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint- eller OneDrive långsam, inte tillgänglig eller inte tillgänglig för flera användare

Om en OneDrive eller SharePoint-webbplatsen inte är tillgänglig för flera användare som tidigare har haft åtkomst kan det finnas en tillfällig service-problem. [Kontrollera att tjänsten hälsa instrumentpanelen](https://portal.office.com/adminportal/home#/servicehealth).

Lägg till och licensiera användaren

Se till att du [tilldela licenser till användare i Office 365 för företag](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


**Tilldela behörigheter**

Om användaren har tilldelats en licens för Sharepoint och ändå får meddelandet åtkomst nekad, kontrollera att de har [rätt behörighetsnivå](https://docs.microsoft.com/sharepoint/understanding-permission-levels) tilldelad.

**Överväg att använda funktionen begäran**

[Begäran funktionen](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) tillåter att begära åtkomst till innehåll som de inte har behörighet att visa för tillfället.

**Tillåt anpassade skript kan orsaka åtkomst nekad problem**

Det finns vissa scenarier där funktionen *Tillåt anpassade skript* kan lyckas förmedla ett åtkomst nekas. För en lista över funktioner som påverkas, säkerhetsaspekter och möjligheten att inaktivera funktionen. Besök [Tillåt eller förhindra att skriptet](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

