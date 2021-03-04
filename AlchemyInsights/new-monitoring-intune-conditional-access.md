---
title: Övervaka villkorsstyrd Intune-åtkomst
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428308"
---
# <a name="monitor-intune-conditional-access"></a>Övervaka villkorsstyrd Intune-åtkomst

Användare med villkorsstyrd åtkomst får ett e-postmeddelande om de inte uppfyller organisationens åtkomstkrav. Som lösning på det rekommenderar vi en eller flera av följande lösningar:

1. Om enheten antas vara registrerad kan du be användaren gå till företagsportalappen och kontrollera att den visas i företagsportalen. Om den inte gör det måste användaren registrera enheten.
1. Gå till **Intune-enhetsefterlevnad i**  >  **Azure-portalen.** 
1. Om du vill visa rapporten över enhetsefterlevnad och verifiera att användarens enhet är markerad som kompatibel klickar du **på** Enhetsefterlevnad under **Bildskärm.**
1. Gå till **Intune-enhetsefterlevnad i**  >  **Azure-portalen.** Klicka **på Principer under** **Hantera.** Kontrollera att en profil är tilldelad till användarens enhet i listan över efterlevnadsprinciper. Om ingen profil har tilldelats kan Intune inte bekräfta enhetens efterlevnadsstatus.
1. Redigera användarens tilldelning av villkorsstyrd åtkomst.
1. Gå till Villkorsstyrda åtkomstprinciper för **Intune** i Azure-portalen, välj en princip i listan  >    >  och klicka **på Användare och grupper.**
1. Om du vill att en viss princip ska vara till för någon lägger du till honom eller honom i **listan Med.** Om du vill säkerställa att en person utelämnas från principen lägger du till dem i **listan med uteslutning.**

**Användbara länkar:**

- [Översikt över enhetsefterlevnad](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Felsökning av certifikatutfärdare](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Felsökningsprincip](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Övervaka Intune-enhetsefterlevnad](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> De här stegen är bara användbara när du felsöker Azure Active Directory-funktionen Villkorlig åtkomst. Det går även att sätta en enhet i karantän, så att den inte har tillgång till e-post med Exchange-principen. Mer information om hantering av Exchange-enheter finns [**här.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
