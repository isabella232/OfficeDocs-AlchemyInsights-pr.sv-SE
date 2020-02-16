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
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="d28bf-102">Åtgärda Office-apparna "Ditt konto är i dåligt läge"</span><span class="sxs-lookup"><span data-stu-id="d28bf-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="d28bf-103">Så här åtgärdar du det här felet genom att prova följande alternativ på den berörda datorn:</span><span class="sxs-lookup"><span data-stu-id="d28bf-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="d28bf-104">Öppna en Office-app, välj > **Utloggning av** > **filkonto**för alla konton . \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="d28bf-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="d28bf-105">Logga in igen med ett användarkonto med en giltig licens.</span><span class="sxs-lookup"><span data-stu-id="d28bf-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="d28bf-106">Mer information finns i [Konton i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="d28bf-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="d28bf-107">[Rensa Office-autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med Windows-autentiseringshanteraren.</span><span class="sxs-lookup"><span data-stu-id="d28bf-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="d28bf-108">**Anm.:** Registersökvägarna för Office 2016 har ändrats till 16.0.</span><span class="sxs-lookup"><span data-stu-id="d28bf-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d28bf-109">Till exempel \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="d28bf-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="d28bf-110">På den berörda datorn anger du EnableADAL = 0 med följande steg:</span><span class="sxs-lookup"><span data-stu-id="d28bf-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="d28bf-111">Högerklicka på Windows-knappen och välj **Kör**.</span><span class="sxs-lookup"><span data-stu-id="d28bf-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="d28bf-112">Skriv **regedit**i rutan **Öppna** och välj sedan **OK**.</span><span class="sxs-lookup"><span data-stu-id="d28bf-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="d28bf-113">Välj **Ja** när du uppmanas att tillåta Registereditorn att göra ändringar på enheten.</span><span class="sxs-lookup"><span data-stu-id="d28bf-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="d28bf-114">Lägg till ett DWORD-värde för EnableADAL i Registereditorn med en inställning på 0 under HKEY_CURRENT_USER\Programvara\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="d28bf-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="d28bf-115">Om felet uppstår när du ansluter till Office 365 med Office 2013 [aktiverar du modern autentisering](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) för Office-klienten.</span><span class="sxs-lookup"><span data-stu-id="d28bf-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="d28bf-116">Mer information finns i Felsöka appar som [inte kan logga in på Office 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="d28bf-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

