---
title: Problem med att logga in på Office-appar
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
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763019"
---
# <a name="issues-signing-in-to-office-apps"></a>Problem med att logga in på Office-appar

Om du vill åtgärda inloggningsproblem med Office-appar provar du följande:

- Ta bort alla arbetskonton utom det berörda kontot med Windows-inställningar > **Access-arbete eller skola**.
- [Rensa Office-autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med Windows-autentiseringshanteraren.<br/>
    **Anm.:** Registersökvägarna för Office 2016 har ändrats till 16.0. (T.ex. \Programvara\Microsoft\Office\16.0\Common\Identity\)
- Öppna ett Office-program, välj > **Logga ut**för > **filkonto**. **File** Logga sedan in med ett användarkonto med en giltig licens. Mer information finns i [Konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- För Mac hittar du information i [Det går inte att logga in i ett Office 2016 för Mac-program](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Om felen uppstår när du ansluter till Microsoft 365 med Office 2013 aktiverar du modern autentisering för Office-klienten.

Mer information finns i:
- [Du kan inte logga in på Microsoft 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Anslutningsproblem i inloggning efter uppdatering av Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Tyvärr, ett annat konto från din organisation är redan inloggad på den här datorn" i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Felsöka inloggningsproblem med Office-modern autentisering när du använder ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)