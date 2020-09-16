---
title: Reparera Microsoft 365-appar ditt konto är i ett felaktigt tillstånd
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744563"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Åtgärda felet för Microsoft 365-apparna "ditt konto är i ett dåligt tillstånd"

För att åtgärda det här felet kan du försöka med följande alternativ på den påverkade datorn:

- Öppna ett Office-program, Välj **fil**  >  **konto**  >  **Logga ut från alla konton**. Logga in igen med ett användar konto med en giltig licens. Mer information finns i [Konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Rensa Office-uppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med hjälp av Windows Autentiseringshanteraren Manager.<br>
  **Obs!** Register Sök vägarna för Office 2016 har ändrats till 16,0. Till exempel \Software\Microsoft\Office\16.0\Common\Identity\
- Om felet uppstår när du ansluter till Office 365 med Office 2013 [aktiverar du modern auktorisering](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) för Office-klienten.

Mer information finns i [så här felsöker du icke-webbläsarbaserade program som inte kan logga in på Microsoft 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

