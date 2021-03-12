---
title: Övervaka villkorsstyrd åtkomst
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708692"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Övervaka villkorsstyrd åtkomst för Exchange

Användare med villkorsstyrd åtkomst får ett e-postmeddelande om de inte uppfyller organisationens åtkomstkrav. Som lösning på det rekommenderar vi en eller flera av följande lösningar:

- Om enheten antas vara registrerad kan du be användaren gå till företagsportalappen och kontrollera att den visas i företagsportalen. Om den inte gör det bör användaren registrera enheten.
- I Azure-portalen går du till Intune > Enhetsefterlevnad. Klicka på Enhetsefterlevnad under Övervaka. Visa rapporten över enhetsefterlevnad för att verifiera att användarens enhet är markerad som kompatibel.
- I Azure-portalen går du till Intune > Enhetsefterlevnad. Klicka på Principer under Hantera. Kontrollera att en profil är tilldelad till användarens enhet i listan över efterlevnadsprinciper. Om ingen profil har tilldelats kan Intune inte bekräfta enhetens efterlevnadsstatus.
- Redigera användarens tilldelning av villkorsstyrd åtkomst.

1. Gå till Villkorsstyrda **åtkomstprinciper för Intune** i Azure  >  **Portal.**  >  
2. Välj en princip i listan.
3. Klicka på Användare och grupper.
4. Om du vill att en viss princip ska vara till för någon lägger du till honom eller honom i listan Med. För att säkerställa att en person utelämnas från principen lägger du till dem i listan med uteslutning.

Användbara länkar:

[Översikt över enhetsefterlevnad](https://docs.microsoft.com/intune/device-compliance-get-started)

[Felsökning av certifikatutfärdare](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Felsökningsprincip](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Övervaka Intune-enhetsefterlevnad](https://docs.microsoft.com/intune/compliance-policy-monitor)

Obs! De här stegen är bara användbara vid felsökning av villkorsstyrd åtkomst i Azure Active Directory-funktionen. Det går även att sätta en enhet i karantän, så att den inte får åtkomst till e-post med Exchange-principen. Mer information om hantering av Exchange-enheter finns [här]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
