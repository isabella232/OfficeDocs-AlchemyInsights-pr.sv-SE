---
title: Villkor för villkorlig åtkomst
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015003"
---
# <a name="conditional-access-issues"></a>Villkor för villkorlig åtkomst

**Lösa problem med inloggnings diagnosen**

Du kan snabbt ta reda på vad som har hänt eller diagnostisera problem med inloggning med hjälp av [inloggnings diagnosen](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Starta inloggnings diagnosen.
1. Hitta den händelse du vill analysera genom att ange informationen du har om användaren, programmet, tiden för inloggning, begärande-ID eller korrelations-ID.
1. Granska de diagnostiska resultaten som visar information om vad som hände och vilka åtgärder du kan vidta för att göra ändringar (om ändringar behövs).

**Steg för att felsöka en inloggning** 

1. Gå till inloggnings sidan för Azure AD.
1. Filtrera inloggnings program efter användare, tidsintervall, program, status, klient program och så vidare.
1. Välj en inloggnings händelse och Visa fliken villkorsstyrd åtkomst för att se vilka principer som utvärderades.
1. Klicka på raden för en princip för att Visa princip detaljerna och förstå varför den tillämpas.

**Verktyg för att felsöka en princip för villkorsstyrd åtkomst**

- I läget endast rapport kan du utvärdera en princip utan att påverka användare.
- Vad händer om du kan simulera inloggnings händelser och se vilka principer som gäller.
- Arbets boken insikter och rapportering visar real tids påverkan för varje princip.

**Principer för rikt linjer**

Principer för rikt linjer är inaktuella. De tillämpas inte längre och kommer snart att tas bort från Azure Portal. Vi rekommenderar att du aktiverar [säkerhets standarder](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Mer information om villkorlig åtkomst finns i:

[Metod tips för villkorlig åtkomst i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Villkor i villkorlig åtkomst](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontroller i villkorlig åtkomst](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Platser i villkorlig åtkomst](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
