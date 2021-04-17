---
title: Åtgärda meddelandet om att Microsoft 365-appar inte kunde hitta associerade Office-licenser
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816506"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="a06ce-102">Åtgärdar meddelandet "Det gick inte att hitta associerade Office-licenser" för Microsoft 365-programmen</span><span class="sxs-lookup"><span data-stu-id="a06ce-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="a06ce-103">Om du får det här meddelandet kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="a06ce-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="a06ce-104">Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att kontrollera att de inte blockerar Internetåtkomsten till Microsoft 365-appar.</span><span class="sxs-lookup"><span data-stu-id="a06ce-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="a06ce-105">Se [URL-adresser och IP-adressintervall för Microsoft 365.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="a06ce-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="a06ce-106">Ta bort [och omtilldela Office-licensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) för den aktuella användaren.</span><span class="sxs-lookup"><span data-stu-id="a06ce-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="a06ce-107">Öppna ett Office-program [och logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användarkonton.</span><span class="sxs-lookup"><span data-stu-id="a06ce-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="a06ce-108">Gå till Windows Inställningar >  >  **e-&-postkonton** och ta bort alla arbetskonton utom det aktuella kontot.</span><span class="sxs-lookup"><span data-stu-id="a06ce-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="a06ce-109">Gå till Windows Inställningar > **Konton Åtkomst till** arbete eller skola  >  **och** koppla bort alla arbetskonton utom det aktuella kontot.</span><span class="sxs-lookup"><span data-stu-id="a06ce-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="a06ce-110">Återställ Office-aktiveringsstatusen.</span><span class="sxs-lookup"><span data-stu-id="a06ce-110">Reset the Office activation state.</span></span> <span data-ttu-id="a06ce-111">[Läs mer](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="a06ce-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="a06ce-112">[Logga in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med det aktuella användarkontot.</span><span class="sxs-lookup"><span data-stu-id="a06ce-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="a06ce-113">Ytterligare felsökningslösningar finns i [Office-felmeddelanden om olicensierad produkt och aktivering.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="a06ce-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>