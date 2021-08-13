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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975119"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Övervaka villkorsstyrd åtkomst för Exchange

Användare med villkorsstyrd åtkomst får ett e-postmeddelande om de inte uppfyller organisationens åtkomstkrav. Vi rekommenderar en eller flera av följande lösningar för att lösa problemet:

- Om enheten antas vara registrerad kan du be användaren gå till Företagsportal-appen och kontrollera att den visas i Företagsportal. Om den inte gör det bör användaren registrera enheten.
- Gå till Intune-tjänsten för enhetsefterlevnad > Azure-portalen. Klicka på Enhetsefterlevnad under Bildskärm. Visa rapporten över enhetsefterlevnad för att verifiera att användarens enhet är markerad som kompatibel.
- Gå till Intune-tjänsten för enhetsefterlevnad > Azure-portalen. Klicka på Principer under Hantera. I listan över efterlevnadsprinciper kontrollerar du att en profil är tilldelad till användarens enhet. Om det inte finns någon tilldelad profil kan Intune inte bekräfta enhetens efterlevnadsstatus.
- Redigera användarens tilldelning av villkorsstyrd åtkomst.

1. Gå till Villkorsstyrda **åtkomstprinciper för Intune**  >  **i Azure-portalen.**  >  
2. Välj en princip i listan.
3. Klicka på Användare och grupper.
4. Om du vill att en viss princip ska vara rätt för en person lägger du till honom/honom i ine inkludera-listan. För att säkerställa att en person utelämnas från principen lägger du till dem i exkluderlistan.

Användbara länkar:

[Översikt över enhetsefterlevnad](https://docs.microsoft.com/intune/device-compliance-get-started)

[Felsöknings-CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Felsökningsprincip](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Övervaka enhetsefterlevnad för Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Obs! De här stegen är bara användbara vid felsökning Azure Active Directory villkorsstyrd åtkomst. Det går även att sätta en enhet i karantän som blockerar den för e-poståtkomst Exchange princip. Mer information om Exchange enhetshantering finns [här]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
