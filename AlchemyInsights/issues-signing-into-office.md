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
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="8b4d2-102">Problem med att logga in på Office-appar</span><span class="sxs-lookup"><span data-stu-id="8b4d2-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="8b4d2-103">Om du vill åtgärda inloggningsproblem med Office-appar provar du följande:</span><span class="sxs-lookup"><span data-stu-id="8b4d2-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="8b4d2-104">Ta bort alla arbetskonton utom det berörda kontot med Windows-inställningar > **Access-arbete eller skola**.</span><span class="sxs-lookup"><span data-stu-id="8b4d2-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="8b4d2-105">[Rensa Office-autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med Windows-autentiseringshanteraren.</span><span class="sxs-lookup"><span data-stu-id="8b4d2-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="8b4d2-106">**Anm.:** Registersökvägarna för Office 2016 har ändrats till 16.0.</span><span class="sxs-lookup"><span data-stu-id="8b4d2-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="8b4d2-107">(T.ex. \Programvara\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="8b4d2-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="8b4d2-108">Öppna ett Office-program, välj > **Logga ut**för > **filkonto**. **File** Logga sedan in med ett användarkonto med en giltig licens.</span><span class="sxs-lookup"><span data-stu-id="8b4d2-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="8b4d2-109">Mer information finns i [Konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="8b4d2-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="8b4d2-110">För Mac hittar du information i [Det går inte att logga in i ett Office 2016 för Mac-program](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="8b4d2-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="8b4d2-111">Om felen uppstår när du ansluter till Microsoft 365 med Office 2013 aktiverar du modern autentisering för Office-klienten.</span><span class="sxs-lookup"><span data-stu-id="8b4d2-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="8b4d2-112">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="8b4d2-112">For more information, see:</span></span>
- [<span data-ttu-id="8b4d2-113">Du kan inte logga in på Microsoft 365, Azure eller Intune</span><span class="sxs-lookup"><span data-stu-id="8b4d2-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="8b4d2-114">Anslutningsproblem i inloggning efter uppdatering av Office 2016 build 16.0.7967 på Windows 10</span><span class="sxs-lookup"><span data-stu-id="8b4d2-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="8b4d2-115">"Tyvärr, ett annat konto från din organisation är redan inloggad på den här datorn" i Office</span><span class="sxs-lookup"><span data-stu-id="8b4d2-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="8b4d2-116">Felsöka inloggningsproblem med Office-modern autentisering när du använder ADFS</span><span class="sxs-lookup"><span data-stu-id="8b4d2-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)