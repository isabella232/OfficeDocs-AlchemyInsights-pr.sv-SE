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
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="617b0-102">Problem att logga in på Office apps</span><span class="sxs-lookup"><span data-stu-id="617b0-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="617b0-103">Åtgärda inloggningsproblem med Office-program gör du följande:</span><span class="sxs-lookup"><span data-stu-id="617b0-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="617b0-104">Ta bort alla konton för arbete, utom påverkade kontot med hjälp av inställningar för Windows > **Access arbetet eller i skolan**.</span><span class="sxs-lookup"><span data-stu-id="617b0-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="617b0-105">[Rensa Office autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med hjälp av Windows Referenshanteraren.</span><span class="sxs-lookup"><span data-stu-id="617b0-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="617b0-106">**Observera:** Registersökvägar 2016 för Office har ändrats till 16,0.</span><span class="sxs-lookup"><span data-stu-id="617b0-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="617b0-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="617b0-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="617b0-108">Öppna ett Office-program, Välj **filen** > **konto** > **Logga ut**. Logga in med ett användarkonto med en giltig licens.</span><span class="sxs-lookup"><span data-stu-id="617b0-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="617b0-109">Mer information finns i [konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="617b0-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="617b0-110">Mac, finns i [Det går inte att logga in på en 2016 Office för Mac-program](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="617b0-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="617b0-111">Aktivera moderna autentisering för Office-klient om fel uppstår vid anslutning till Office 365 med Office 2013.</span><span class="sxs-lookup"><span data-stu-id="617b0-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="617b0-112">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="617b0-112">For more information, see:</span></span>
- [<span data-ttu-id="617b0-113">Du kan inte logga in på Office 365, Azure eller Intune</span><span class="sxs-lookup"><span data-stu-id="617b0-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="617b0-114">Anslutningsproblem i logga in efter uppdatering till Office 2016 bygga 16.0.7967 på Windows 10</span><span class="sxs-lookup"><span data-stu-id="617b0-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="617b0-115">”Tyvärr, ett annat konto från din organisation är redan inloggad på den här datorn” i Office</span><span class="sxs-lookup"><span data-stu-id="617b0-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="617b0-116">Felsöka inloggningsproblem med moderna autentisering i Office när du använder AD FS</span><span class="sxs-lookup"><span data-stu-id="617b0-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)