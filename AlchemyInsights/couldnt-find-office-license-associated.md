---
title: Fastställande Office apps kunde inte hitta Office-licenser associerade meddelande
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
ms.openlocfilehash: 1820cdb83a1adf36b4e7d0898ecdf8097eb6f0f3
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627936"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="cc28b-102">Åtgärda Office-appar "Det gick inte att hitta Office-licenser associerade" meddelande</span><span class="sxs-lookup"><span data-stu-id="cc28b-102">Fixing the Office apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="cc28b-103">Om det här meddelandet visas provar du följande:</span><span class="sxs-lookup"><span data-stu-id="cc28b-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="cc28b-104">Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att bekräfta att de inte blockerar Internet-åtkomst till Office-appar.</span><span class="sxs-lookup"><span data-stu-id="cc28b-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="cc28b-105">Se [Office 365-URL: er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="cc28b-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="cc28b-106">Ta bort och [omtilldela Office-licensen](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) för den berörda användaren.</span><span class="sxs-lookup"><span data-stu-id="cc28b-106">Remove and [reassign the Office license](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="cc28b-107">Öppna en Office-app och [Logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från alla befintliga användarkonton.</span><span class="sxs-lookup"><span data-stu-id="cc28b-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="cc28b-108">Gå till Windows-inställningar > **konton** > **e-& konton**och ta bort alla arbetskonton utom det berörda kontot.</span><span class="sxs-lookup"><span data-stu-id="cc28b-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="cc28b-109">Gå till Windows-inställningar > **konton** > **tillgång till arbete eller skola**och koppla från alla arbetskonton utom det berörda kontot.</span><span class="sxs-lookup"><span data-stu-id="cc28b-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="cc28b-110">Återställ aktiveringstillståndet för Office.</span><span class="sxs-lookup"><span data-stu-id="cc28b-110">Reset the Office activation state.</span></span> <span data-ttu-id="cc28b-111">[Läs mer](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="cc28b-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="cc28b-112">[Logga in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med det aktuella användarkontot.</span><span class="sxs-lookup"><span data-stu-id="cc28b-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="cc28b-113">Ytterligare felsökningslösningar finns [i olicensierade produkt-och aktiveringsfel i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="cc28b-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>