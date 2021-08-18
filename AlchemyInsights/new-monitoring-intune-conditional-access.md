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
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327575"
---
# <a name="monitor-intune-conditional-access"></a>Övervaka villkorsstyrd Intune-åtkomst

Användare med villkorsstyrd åtkomst får ett e-postmeddelande om de inte uppfyller organisationens åtkomstkrav. Vi rekommenderar en eller flera av följande lösningar för att lösa problemet:

1. Om enheten antas vara registrerad kan du be användaren gå till Företagsportal-appen och kontrollera att den visas i Företagsportal. Om den inte gör det måste användaren registrera enheten.
1. Gå till **Intune** Enhetsefterlevnad i  >  **Azure-portalen.** 
1. Om du vill visa rapporten över enhetsefterlevnad och verifiera att användarens enhet är markerad som kompatibel klickar du **på** Enhetsefterlevnad under **Bildskärm.**
1. Gå till **Intune** Enhetsefterlevnad i  >  **Azure-portalen.** Klicka **på Principer** under **Hantera.** I listan över efterlevnadsprinciper kontrollerar du att en profil är tilldelad till användarens enhet. Om det inte finns någon tilldelad profil kan Intune inte bekräfta enhetens efterlevnadsstatus.
1. Redigera användarens tilldelning av villkorsstyrd åtkomst.
1. Gå till Villkorsstyrda **åtkomstprinciper för Intune** i Azure-portalen , välj en princip i listan  >    >  och klicka **på Användare och grupper.**
1. Om du vill att en viss princip ska vara mål för en person lägger du till honom/honom i **ine- listan**. För att säkerställa att en person utelämnas från principen lägger du till dem i **exkluderlistan.**

**Användbara länkar:**

- [Översikt över enhetsefterlevnad](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Felsöknings-CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Felsökningsprincip](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Övervaka enhetsefterlevnad för Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Obs!** De här stegen är bara användbara vid felsökning Azure Active Directory villkorsstyrd åtkomst. Det går även att sätta en enhet i karantän som blockerar den för e-poståtkomst Exchange princip. Mer information Exchange om enhetshantering finns [**här.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
