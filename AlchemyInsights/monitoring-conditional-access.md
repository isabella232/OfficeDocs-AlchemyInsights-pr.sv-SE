---
title: Övervaka villkorlig åtkomst
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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366446"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Övervaka villkorlig åtkomst för Exchange

Användare riktade mot villkorsstyrd åtkomst får ett e-postmeddelande om de inte uppfyller åtkomst kraven för organisationen. För att lösa problemet rekommenderar vi en eller flera av följande lösningar:

- Om enheten är registrerad kan du uppmana användaren att gå till företagsportalsappen och kontrol lera att den visas i företags portalen. Om det inte gör det bör användaren registrera enheten.
- I Azure-portalen går du till Intune > enhets efterlevnad. Klicka på enhets överensstämmelse under bildskärm. Visa din enhets kompatibilitetsstatus för att kontrol lera att användarens enhet är markerad som kompatibel.
- I Azure-portalen går du till Intune > enhets efterlevnad. Under hantera klickar du på principer. I listan över efterlevnadsprinciper kontrollerar du att en profil har tilldelats till din användares enhet. Om ingen profil är tilldelad kan Intune inte bekräfta status för enhetens efterlevnad.
- Redigera användarens villkorliga åtkomst tilldelning.

1. I Azure-portalen går du till **Intune**  >  policy för**villkorlig åtkomst**  >  **Policies**.
2. Välj en princip i listan.
3. Klicka på användare och grupper.
4. Om du vill rikta en viss princip till någon kan du lägga till dem i listan ta med. Om du vill se till att en person utelämnas från policyn lägger du till den i listan undantag.

Användbara länkar:

[Översikt över enhetens efterlevnad](https://docs.microsoft.com/intune/device-compliance-get-started)

[Felsöka CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Fel söknings princip](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Övervaka efterlevnad av Intune-enheter](https://docs.microsoft.com/intune/compliance-policy-monitor)

Obs! de här stegen är bara till hjälp när du ska felsöka villkorlig åtkomst för Azure Active Directory-funktionen. Det går också att använda karantän en enhet för att blockera e-poståtkomst med Exchange-princip. Mer information om Exchange Device Management finns [här](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
