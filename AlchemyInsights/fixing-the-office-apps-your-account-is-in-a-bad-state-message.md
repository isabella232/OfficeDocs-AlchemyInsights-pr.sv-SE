---
title: Åtgärda Microsoft 365-appar Ditt konto är i ett felaktigt tillstånd meddelande
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: 264307f23a349ef4ebf40f48ddbcddd3216a4927
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580135"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Åtgärda microsoft 365-apparna "Ditt konto är i dåligt skick"

Lös det här felet genom att prova följande alternativ på den berörda datorn:

- Öppna ett Office-program, välj **Logga**ut  >  **filkonto**  >  **för alla konton**. Logga in igen med ett användarkonto med en giltig licens. Mer information finns i [Konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Rensa Office-autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med Windows-autentiseringshanteraren.<br>
  **Anm.:** Registersökvägarna för Office 2016 har ändrats till 16.0. Till exempel \Software\Microsoft\Office\16.0\Common\Identity\
- Om felet uppstår när du ansluter till Office 365 med Office 2013 [aktiverar du modern autentisering](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) för Office-klienten.

Mer information finns [i Felsöka appar som inte är webbläsare som inte kan logga in på Microsoft 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

