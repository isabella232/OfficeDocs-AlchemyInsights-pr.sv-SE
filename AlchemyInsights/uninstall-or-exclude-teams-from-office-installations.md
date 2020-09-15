---
title: Avinstallera eller exkludera team från Office-installationer
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
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658239"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Avinstallera eller exkludera team från nya eller befintliga Office-installationer

Microsoft Teams är en del av Microsoft 365-appar för Enterprise, Microsoft 365-appar för företag och Office för Mac.

- Använd [distributions verktyget för Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) för att utesluta Teams från nya installationer av Office.
- Information om hur du *avinstallerar* Teams från en enhet med Windows finns i [Avinstallera Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Information om hur du rensar Microsoft Teams från flera mål datorer eller användare finns i [Microsoft Teams Deployment Cleanup](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Använd alternativet [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) för att förhindra att Microsoft Teams installeras automatiskt med Office.
- Använd alternativet [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *innan Teams installeras*för att förhindra att Microsoft Teams startar automatiskt efter installationen.

Om du använder Office för Mac läser du [Microsoft Teams-installationer på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).