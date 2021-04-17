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
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="0e332-102">Åtgärda meddelandet "Tyvärr, ett annat konto från din organisation är redan inloggad" i Microsoft 365-programmen</span><span class="sxs-lookup"><span data-stu-id="0e332-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="0e332-103">Lös problemet genom att prova med följande:</span><span class="sxs-lookup"><span data-stu-id="0e332-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="0e332-104">Ta bort alla arbetskonton, förutom det aktuella kontot, med hjälp av Windows-> **Åtkomst till arbete eller skola.**</span><span class="sxs-lookup"><span data-stu-id="0e332-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="0e332-105">[Ta bort Office-autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med Windows Autentiseringshanteraren.</span><span class="sxs-lookup"><span data-stu-id="0e332-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="0e332-106">**Obs!** Registersökvägarna för Office 2016 har ändrats till 16.0.</span><span class="sxs-lookup"><span data-stu-id="0e332-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="0e332-107">(Exempel: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="0e332-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="0e332-108">Öppna ett Office-program och välj **Logga**  >  **ut från**  >  **konto.** Logga sedan in med ett användarkonto med en giltig licens.</span><span class="sxs-lookup"><span data-stu-id="0e332-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="0e332-109">Mer information finns i [Konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="0e332-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="0e332-110">För Mac hittar du information i [Det går inte att logga in i ett Office 2016 för Mac-program](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="0e332-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="0e332-111">Mer information finns i "Tyvärr är ett annat konto från organisationen redan inloggad [på den här datorn" i Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)</span><span class="sxs-lookup"><span data-stu-id="0e332-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>