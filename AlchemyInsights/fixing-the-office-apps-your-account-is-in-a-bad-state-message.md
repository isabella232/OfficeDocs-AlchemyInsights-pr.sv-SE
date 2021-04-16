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
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="d76c0-102">Åtgärda felmeddelandet "Ditt konto är i ett dåligt tillstånd" för Microsoft 365-programmen</span><span class="sxs-lookup"><span data-stu-id="d76c0-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="d76c0-103">Prova följande alternativ på den aktuella datorn för att åtgärda felet:</span><span class="sxs-lookup"><span data-stu-id="d76c0-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="d76c0-104">Öppna ett Office-program och **välj**  >  **Logga ut** från alla  >  **konton.**</span><span class="sxs-lookup"><span data-stu-id="d76c0-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="d76c0-105">Logga in igen med ett användarkonto med en giltig licens.</span><span class="sxs-lookup"><span data-stu-id="d76c0-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="d76c0-106">Mer information finns i [Konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="d76c0-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="d76c0-107">[Ta bort Office-autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med Windows Autentiseringshanteraren.</span><span class="sxs-lookup"><span data-stu-id="d76c0-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="d76c0-108">**Obs!** Registersökvägarna för Office 2016 har ändrats till 16.0.</span><span class="sxs-lookup"><span data-stu-id="d76c0-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d76c0-109">Exempel: \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="d76c0-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="d76c0-110">Om felet uppstår när du ansluter till Office 365 med Hjälp av Office 2013 kan du [aktivera modern autentisering](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) för Office-klienten.</span><span class="sxs-lookup"><span data-stu-id="d76c0-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="d76c0-111">Mer information finns i Felsöka appar som inte är webbläsarbaserade och som inte kan logga in på [Microsoft 365, Azure eller Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)</span><span class="sxs-lookup"><span data-stu-id="d76c0-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

