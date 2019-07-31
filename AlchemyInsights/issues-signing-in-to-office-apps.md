---
title: Problem att logga in på Office apps
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
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938357"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Fastställande av Office apps ”tyvärr, ett annat konto från din organisation är redan inloggad” meddelande

Försök med följande om du vill åtgärda det här felet:

- Ta bort alla konton för arbete, utom påverkade kontot med hjälp av inställningar för Windows > **Access arbetet eller i skolan**.
- [Rensa Office autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med hjälp av Windows Referenshanteraren.<br/>
    **Observera:** Registersökvägar 2016 för Office har ändrats till 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Öppna ett Office-program, Välj **filen** > **konto** > **Logga ut**. Logga in med ett användarkonto med en giltig licens. Mer information finns i [konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Mac, finns i [Det går inte att logga in på en 2016 Office för Mac-program](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Mer information finns i [”tyvärr, ett annat konto från din organisation är redan inloggad på den här datorn” i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).