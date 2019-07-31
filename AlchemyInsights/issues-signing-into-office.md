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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938358"
---
# <a name="issues-signing-in-to-office-apps"></a>Problem att logga in på Office apps

Åtgärda inloggningsproblem med Office-program gör du följande:

- Ta bort alla konton för arbete, utom påverkade kontot med hjälp av inställningar för Windows > **Access arbetet eller i skolan**.
- [Rensa Office autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med hjälp av Windows Referenshanteraren.<br/>
    **Observera:** Registersökvägar 2016 för Office har ändrats till 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Öppna ett Office-program, Välj **filen** > **konto** > **Logga ut**. Logga in med ett användarkonto med en giltig licens. Mer information finns i [konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Mac, finns i [Det går inte att logga in på en 2016 Office för Mac-program](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Aktivera moderna autentisering för Office-klient om fel uppstår vid anslutning till Office 365 med Office 2013.

Mer information finns i:
- [Du kan inte logga in på Office 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Anslutningsproblem i logga in efter uppdatering till Office 2016 bygga 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [”Tyvärr, ett annat konto från din organisation är redan inloggad på den här datorn” i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Felsöka inloggningsproblem med moderna autentisering i Office när du använder AD FS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)