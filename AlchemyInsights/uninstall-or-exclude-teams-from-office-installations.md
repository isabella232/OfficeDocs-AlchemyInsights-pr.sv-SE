---
title: Avinstallera eller utesluta Teams från Office-installationer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: b6613733e743e08a9b18b1ada70fde164b0d5dc3
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010334"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="cd3c8-102">Avinstallera eller utesluta Teams från nya eller befintliga Office-installationer</span><span class="sxs-lookup"><span data-stu-id="cd3c8-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="cd3c8-103">Microsoft Teams ingår som en del av Microsoft 365 Apps for Enterprise, Microsoft 365 Apps for business och Office för Mac.</span><span class="sxs-lookup"><span data-stu-id="cd3c8-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="cd3c8-104">Använd [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) för att utesluta team från nya installationer av Office.</span><span class="sxs-lookup"><span data-stu-id="cd3c8-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="cd3c8-105">Information om hur du *avinstallerar* Teams från en enhet som kör Windows finns i [Avinstallera Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="cd3c8-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="cd3c8-106">Om du vill rensa Microsoft Teams från flera måldatorer eller användare läser du [rensning av Microsoft Teams-distribution.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)</span><span class="sxs-lookup"><span data-stu-id="cd3c8-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="cd3c8-107">Använd alternativet [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) för att förhindra att Microsoft Teams installeras automatiskt med Office.</span><span class="sxs-lookup"><span data-stu-id="cd3c8-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="cd3c8-108">Använd alternativet [PreventFirstLaunchAfterInstallera](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *innan Teams installeras*för att förhindra att Microsoft Teams startar automatiskt efter installationen.</span><span class="sxs-lookup"><span data-stu-id="cd3c8-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="cd3c8-109">Om du använder Office för Mac läser du [Microsoft Teams-installationer på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="cd3c8-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>