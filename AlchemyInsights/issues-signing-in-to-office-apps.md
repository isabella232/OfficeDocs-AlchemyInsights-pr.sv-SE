---
title: Problem med att logga in i Microsoft 365-appar
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
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695341"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Att åtgärda Microsoft 365-programmen "ett annat konto från din organisation redan är inloggat"

Lös problemet genom att prova med följande:

- Ta bort alla arbets konton, förutom det berörda kontot, med Windows-inställningar > **Access-eller skol arbete**.
- [Rensa Office-uppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med hjälp av Windows Autentiseringshanteraren Manager.<br/>
    **Obs!** Register Sök vägarna för Office 2016 har ändrats till 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Öppna ett Office-program, Välj **fil**  >  **konto**–  >  **Logga ut**. Logga sedan in med ett användar konto med en giltig licens. Mer information finns i [Konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- För Mac hittar du information i [Det går inte att logga in i ett Office 2016 för Mac-program](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Mer information finns i ["Tyvärr, ett annat konto från din organisation redan är inloggad på den här datorn" i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).