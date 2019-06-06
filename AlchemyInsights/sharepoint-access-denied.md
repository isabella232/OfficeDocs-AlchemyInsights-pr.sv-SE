---
title: 'Felsökning: åtkomst nekad meddelanden'
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 5958ad06ca905f713b5f56aa5c536e95a485f01c
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735755"
---
# <a name="troubleshoot-access-denied-messages"></a>Felsökning: åtkomst nekad meddelanden

Om du får meddelandet åtkomst nekad när du försöker bläddra i en Sharepoint Online-webbplats kan du se den under artiklar.

## <a name="add-and-license-the-user"></a>Lägg till och licensiera användaren

Se till att du [tilldela licenser till användare i Office 365 för företag](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).

Tilldela behörigheter

Om användaren har tilldelats en licens för Sharepoint och ändå får meddelandet åtkomst nekad, kontrollera att de har [tilldelats rätt behörighet](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).

Överväg att använda funktionen begäran

[Åtkomstbegäran](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) funktionen tillåter att begära åtkomst till innehåll som de inte har behörighet att visa för tillfället. 

Tillåt anpassade skript kan orsaka åtkomst nekad problem

Det finns vissa scenarier där funktionen ”Tillåt anpassade skript” kan lyckas förmedla ett åtkomst nekas. För en lista över funktioner som påverkas, säkerhetsaspekter och möjligheten att inaktivera funktionen. Besök, [Tillåt eller förhindra anpassat skript](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)

Anmärkning: Om OneDrive eller SharePoint-webbplatsen inte är tillgänglig för flera användare som tidigare hade åtkomst, kan det finnas en tillfällig service problem. [Kontrollera att tjänsten hälsa instrumentpanelen](https://portal.office.com/adminportal/home#/servicehealth).


  

