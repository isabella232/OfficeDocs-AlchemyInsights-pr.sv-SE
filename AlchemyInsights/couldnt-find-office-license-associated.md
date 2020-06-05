---
title: Åtgärda Microsoft 365-appar Kunde inte hitta associerat meddelande om office-licenser
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580459"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="1dd6d-102">Åtgärda meddelandet "Det gick inte att hitta associerade office-licenser" i Microsoft 365-apparna</span><span class="sxs-lookup"><span data-stu-id="1dd6d-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="1dd6d-103">Om du får det här meddelandet kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="1dd6d-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="1dd6d-104">Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att bekräfta att de inte blockerar Internetåtkomst till Microsoft 365-appar.</span><span class="sxs-lookup"><span data-stu-id="1dd6d-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="1dd6d-105">Se [Microsoft 365-URL:er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="1dd6d-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="1dd6d-106">Ta bort och [tilldela office-licensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) för den berörda användaren.</span><span class="sxs-lookup"><span data-stu-id="1dd6d-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="1dd6d-107">Öppna ett Office-program och [logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användarkonton.</span><span class="sxs-lookup"><span data-stu-id="1dd6d-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="1dd6d-108">Gå till Windows-inställningar **Accounts**>  >  **Konton e-& konton**och ta bort alla arbetskonton utom det berörda kontot.</span><span class="sxs-lookup"><span data-stu-id="1dd6d-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="1dd6d-109">Gå till Windows-inställningar > **Konton**  >  **Access-arbete eller skola**och koppla från alla arbetskonton utom det berörda kontot.</span><span class="sxs-lookup"><span data-stu-id="1dd6d-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="1dd6d-110">Återställ Office-aktiveringsstatusen.</span><span class="sxs-lookup"><span data-stu-id="1dd6d-110">Reset the Office activation state.</span></span> <span data-ttu-id="1dd6d-111">[Läs mer](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="1dd6d-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="1dd6d-112">[Logga in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med det berörda användarkontot.</span><span class="sxs-lookup"><span data-stu-id="1dd6d-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="1dd6d-113">Ytterligare felsökningslösningar finns [i Olicensierade produkt- och aktiveringsfel i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="1dd6d-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>