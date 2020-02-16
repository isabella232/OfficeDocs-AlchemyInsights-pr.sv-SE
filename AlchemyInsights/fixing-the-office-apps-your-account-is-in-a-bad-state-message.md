---
title: Åtgärda Office Apps Ditt konto är i ett meddelande om dåligt tillstånd
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
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969847"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Åtgärda Office-apparna "Ditt konto är i dåligt läge"

Så här åtgärdar du det här felet genom att prova följande alternativ på den berörda datorn:

- Öppna en Office-app, välj > **Utloggning av** > **filkonto**för alla konton . **** Logga in igen med ett användarkonto med en giltig licens. Mer information finns i [Konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Rensa Office-autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med Windows-autentiseringshanteraren.<br>
  **Anm.:** Registersökvägarna för Office 2016 har ändrats till 16.0. Till exempel \Software\Microsoft\Office\16.0\Common\Identity\
- På den berörda datorn anger du EnableADAL = 0 med följande steg:  
     1. Högerklicka på Windows-knappen och välj **Kör**. Skriv **regedit**i rutan **Öppna** och välj sedan **OK**.
     2. Välj **Ja** när du uppmanas att tillåta Registereditorn att göra ändringar på enheten.
    3. Lägg till ett DWORD-värde för EnableADAL i Registereditorn med en inställning på 0 under HKEY_CURRENT_USER\Programvara\Microsoft\Office\16.0\Common\Identity.
- Om felet uppstår när du ansluter till Office 365 med Office 2013 [aktiverar du modern autentisering](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) för Office-klienten.

Mer information finns i Felsöka appar som [inte kan logga in på Office 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

