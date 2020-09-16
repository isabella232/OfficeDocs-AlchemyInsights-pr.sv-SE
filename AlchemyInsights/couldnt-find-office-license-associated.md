---
title: Reparera Microsoft 365-appar det gick inte att hitta det kopplade meddelandet för Office-licenser
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747713"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="9325a-102">Åtgärda meddelande om att Microsoft 365-apparna inte hittade Office-licenser</span><span class="sxs-lookup"><span data-stu-id="9325a-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="9325a-103">Om du får det här meddelandet kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="9325a-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="9325a-104">Kontrol lera brand vägg, antivirus program och proxyinställningar för att bekräfta att de inte blockerar Internet åtkomst till Microsoft 365-appar.</span><span class="sxs-lookup"><span data-stu-id="9325a-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="9325a-105">Se [Microsoft 365 URL: er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="9325a-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="9325a-106">Ta bort och [tilldela om Office-licensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) för den aktuella användaren.</span><span class="sxs-lookup"><span data-stu-id="9325a-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="9325a-107">Öppna ett Office-program och [Logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användar konton.</span><span class="sxs-lookup"><span data-stu-id="9325a-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="9325a-108">Gå till Windows-inställningar > **konton**  >  **& konton**och ta bort alla arbets konton förutom det berörda kontot.</span><span class="sxs-lookup"><span data-stu-id="9325a-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="9325a-109">Gå till Windows-inställningar > **konton**  >  **åtkomst till arbets-eller skol arbete**och koppla från alla arbets konton förutom det berörda kontot.</span><span class="sxs-lookup"><span data-stu-id="9325a-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="9325a-110">Återställ Office-aktiveringsstatusen.</span><span class="sxs-lookup"><span data-stu-id="9325a-110">Reset the Office activation state.</span></span> <span data-ttu-id="9325a-111">[Läs mer](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="9325a-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="9325a-112">[Logga](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) in med det användar konto som påverkas.</span><span class="sxs-lookup"><span data-stu-id="9325a-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="9325a-113">Ytterligare lösningar för fel sökning finns i [olicensierad produkt och aktiverings fel i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="9325a-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>