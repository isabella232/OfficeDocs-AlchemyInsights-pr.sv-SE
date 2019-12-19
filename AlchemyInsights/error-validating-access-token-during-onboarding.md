---
title: Ett fel uppstod vid validering av åtkomsttokenfel vid skrivbords analys vid ombordstigning
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741286"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"Det uppstod ett fel vid validering av åtkomsttoken" fel vid registrering av skrivbords analys

Det här felet observeras normalt när autentiseringstoken upphör att gälla. Vanligtvis uppdatera sidan uppdaterar token. Det här problemet kan dock kvarstå om det finns några principer för villkorlig åtkomst tillämpas på kontot som används för att ombord Desktop Analytics. Du kan granska den Azure AD loggar in loggar i Azure-portalen för att se om det finns några Inloggningsfel för det konto som används för Desktop Analytics onboarding.

Mer information om villkorlig åtkomst finns i [Planera distributionen av villkorlig åtkomst](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).