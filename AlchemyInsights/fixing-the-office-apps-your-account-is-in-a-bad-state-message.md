---
title: Åtgärda Microsoft 365-appar Ditt konto har ett meddelande om felaktig status
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
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812554"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Åtgärda felmeddelandet "Ditt konto är i ett dåligt tillstånd" för Microsoft 365-programmen

Prova följande alternativ på den aktuella datorn för att åtgärda felet:

- Öppna ett Office-program och **välj**  >  **Logga ut** från alla  >  **konton.** Logga in igen med ett användarkonto med en giltig licens. Mer information finns i [Konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Ta bort Office-autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med Windows Autentiseringshanteraren.<br>
  **Obs!** Registersökvägarna för Office 2016 har ändrats till 16.0. Exempel: \Software\Microsoft\Office\16.0\Common\Identity\
- Om felet uppstår när du ansluter till Office 365 med Hjälp av Office 2013 kan du [aktivera modern autentisering](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) för Office-klienten.

Mer information finns i Felsöka appar som inte är webbläsarbaserade och som inte kan logga in på [Microsoft 365, Azure eller Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

