---
title: Problem med att logga in på Microsoft 365-appar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579955"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Åtgärda meddelandet "Tyvärr, ett annat konto från organisationen är redan inloggad"

Lös problemet genom att prova med följande:

- Ta bort alla arbetskonton utom det berörda kontot med Windows-inställningar > **Access-arbete eller skola**.
- [Rensa Office-autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med Windows-autentiseringshanteraren.<br/>
    **Anm.:** Registersökvägarna för Office 2016 har ändrats till 16.0. (T.ex. \Programvara\Microsoft\Office\16.0\Common\Identity\)
- Öppna ett Office-program, välj Logga ut **för**  >  **filkonto**  >  **Sign Out**. Logga sedan in med ett användarkonto med en giltig licens. Mer information finns i [Konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- För Mac hittar du information i [Det går inte att logga in i ett Office 2016 för Mac-program](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Mer information finns i ["Tyvärr, ett annat konto från din organisation är redan inloggad på den här datorn" i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).