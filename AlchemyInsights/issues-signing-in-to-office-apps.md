---
title: Problem med inloggning på Microsoft 365-appar
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
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833093"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Åtgärda meddelandet "Tyvärr, ett annat konto från din organisation är redan inloggad" i Microsoft 365-programmen

Lös problemet genom att prova med följande:

- Ta bort alla arbetskonton, förutom det aktuella kontot, med hjälp av Windows-> **Åtkomst till arbete eller skola.**
- [Ta bort Office-autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med Windows Autentiseringshanteraren.<br/>
    **Obs!** Registersökvägarna för Office 2016 har ändrats till 16.0. (Exempel: \Software\Microsoft\Office\16.0\Common\Identity\)
- Öppna ett Office-program och välj **Logga**  >  **ut från**  >  **konto.** Logga sedan in med ett användarkonto med en giltig licens. Mer information finns i [Konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- För Mac hittar du information i [Det går inte att logga in i ett Office 2016 för Mac-program](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Mer information finns i "Tyvärr är ett annat konto från organisationen redan inloggad [på den här datorn" i Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)