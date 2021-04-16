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
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813706"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Felet "Ett fel uppstod vid validering av åtkomsttoken" under registrering av Skrivbordsanalys

Det här felet observeras normalt när autentiseringstoken upphör att gälla. Vanligtvis uppdateras token när sidan uppdateras. Men det här problemet kan kvarstå om det finns några villkorsstyrda åtkomstprinciper som tillämpas på det konto som används för skrivbordsanalys. Du kan granska Azure AD-inloggningsloggarna i Azure Portal för att se om det uppstår något inloggningsfel för det konto som används för registrering av Skrivbordsanalys.

Mer information om villkorsstyrd åtkomst finns i [Planera villkorsstyrd åtkomstdistribution.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)