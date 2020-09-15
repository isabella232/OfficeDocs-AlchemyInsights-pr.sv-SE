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
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="e7581-102">Att åtgärda Microsoft 365-programmen "ett annat konto från din organisation redan är inloggat"</span><span class="sxs-lookup"><span data-stu-id="e7581-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="e7581-103">Lös problemet genom att prova med följande:</span><span class="sxs-lookup"><span data-stu-id="e7581-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="e7581-104">Ta bort alla arbets konton, förutom det berörda kontot, med Windows-inställningar > **Access-eller skol arbete**.</span><span class="sxs-lookup"><span data-stu-id="e7581-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="e7581-105">[Rensa Office-uppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med hjälp av Windows Autentiseringshanteraren Manager.</span><span class="sxs-lookup"><span data-stu-id="e7581-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="e7581-106">**Obs!** Register Sök vägarna för Office 2016 har ändrats till 16,0.</span><span class="sxs-lookup"><span data-stu-id="e7581-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e7581-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="e7581-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="e7581-108">Öppna ett Office-program, Välj **fil**  >  **konto**–  >  **Logga ut**. Logga sedan in med ett användar konto med en giltig licens.</span><span class="sxs-lookup"><span data-stu-id="e7581-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="e7581-109">Mer information finns i [Konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="e7581-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="e7581-110">För Mac hittar du information i [Det går inte att logga in i ett Office 2016 för Mac-program](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="e7581-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="e7581-111">Mer information finns i ["Tyvärr, ett annat konto från din organisation redan är inloggad på den här datorn" i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="e7581-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>