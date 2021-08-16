---
title: Problem med att logga in Microsoft 365 appar
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
- "9000571"
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028058"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Åtgärda meddelandet "Microsoft 365, ett annat konto från din organisation är redan inloggad" när du åtgärdar problem med appen

Lös problemet genom att prova med följande:

- Ta bort alla arbetskonton, förutom det aktuella kontot, med hjälp Windows Inställningar > **Åtkomst till arbete eller skola.**
- [Ta Office autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med Windows Autentiseringshanteraren.<br/>
    **Obs!** Registersökvägarna för Office 2016 har ändrats till 16.0. (Exempel: \Software\Microsoft\Office\16.0\Common\Identity\)
- Öppna en Office-appen väljer du **Logga**  >  **ut från**  >  **filkonto.** Logga sedan in med ett användarkonto med en giltig licens. Mer information finns i [Konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- För Mac hittar du information i [Det går inte att logga in i ett Office 2016 för Mac-program](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Mer information finns i ["Tyvärr är ett annat konto från](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)din organisation redan inloggad på den här datorn" i Office .