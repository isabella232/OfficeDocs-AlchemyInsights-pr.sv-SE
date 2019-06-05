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
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719534"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint- eller OneDrive långsam, inte tillgänglig eller inte tillgänglig för flera användare

Om en OneDrive eller SharePoint-webbplatsen inte är tillgänglig för flera användare som tidigare har haft åtkomst kan det finnas en tillfällig service-problem. [Kontrollera att tjänsten hälsa instrumentpanelen](https://portal.office.com/adminportal/home#/servicehealth).

## <a name="add-and-license-the-user"></a>Lägg till och licensiera användaren

Se till att du [tilldela licenser till användare i Office 365 för företag](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


## <a name="assign-permissions"></a>Tilldela behörigheter

Om användaren har tilldelats en licens för Sharepoint och ändå får meddelandet åtkomst nekad, kontrollera att de har [rätt behörighetsnivå](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) tilldelad.

## <a name="consider-using-the-access-request-feature"></a>Överväg att använda funktionen begäran

[Begäran funktionen](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) tillåter att begära åtkomst till innehåll som de inte har behörighet att visa för tillfället.

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>Tillåt anpassade skript kan orsaka åtkomst nekad problem

Det finns vissa scenarier där funktionen *Tillåt anpassade skript* kan lyckas förmedla ett åtkomst nekas. För en lista över funktioner som påverkas, säkerhetsaspekter och möjligheten att inaktivera funktionen. Besök [Tillåt eller förhindra att skriptet](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).

