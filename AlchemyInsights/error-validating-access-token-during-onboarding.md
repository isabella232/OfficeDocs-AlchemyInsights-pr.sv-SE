---
title: Ett fel uppstod vid validering av åtkomsttoken under skrivbordsanalys på boarding
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946633"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Felet "Ett fel uppstod vid validering av åtkomsttoken" under registrering av Skrivbordsanalys

Det här felet observeras normalt när autentiseringstoken upphör att gälla. Vanligtvis uppdateras token när sidan uppdateras. Men det här problemet kan kvarstå om det finns några villkorsstyrda åtkomstprinciper som tillämpas på det konto som används för skrivbordsanalys. Du kan granska Azure AD-inloggningsloggarna i Azure Portal för att se om det uppstår något inloggningsfel för det konto som används för registrering av Skrivbordsanalys.

Mer information om villkorsstyrd åtkomst finns i [Planera villkorsstyrd åtkomstdistribution.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)