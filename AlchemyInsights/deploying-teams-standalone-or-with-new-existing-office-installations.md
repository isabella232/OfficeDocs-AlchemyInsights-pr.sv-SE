---
title: Distribuera team som fristående eller med nya eller befintliga Office-installationer
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054248"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Distribuera team som fristående eller med nya eller befintliga Office-installationer

Microsoft Teams är nu ingår i ***nya installationer*** av Office 365 ProPlus, Office 365 Business och Office för Mac. Mer information finns i [när Microsoft-Teams börjar tas med i nya installationer av Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Dessutom kommer börjar med Version 1906 i månatliga kanal, team att ***läggas till i befintliga installationer*** av Office 365 ProPlus (och Office 365 Business) på enheter som kör Windows när du uppdaterar den befintliga installationen till den senaste versionen. Mer information finns i [hur befintliga installationer av Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Om du inte vill vänta på att installationen schemat du kan distribuera team som fristående för dina användare genom att [följa dessa instruktioner](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) eller du kan låta användarna installera team för sig själva från [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Om din organisation inte är redo att distribuera team har vi steg du kan vidta för att ***utesluta team*** från [nya](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) eller [befintliga](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installationer av Office. Om du vill att grupper kan installeras, men inte vill team ska starta automatiskt för användaren när det är installerat, se [Microsoft förhindra team från att starta automatiskt efter installationen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

***Avinstallera team*** från en enhet som kör Windows i avsnittet [Avinstallera Microsoft team](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). För rensning av Microsoft Teams från flera måldatorer eller användare, se [Microsoft team distribution Rensa](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Om du använder delade datorer, Remote Desktop Services (RDS) eller virtuella skrivbordet infrastruktur (VDI) finns i [delad dator och VDI-miljöer med Microsoft team](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Om du använder Office för Mac finns i [Microsoft-team installationer på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> När du har installerat team är det [uppdateras automatiskt](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) ungefär varannan vecka med nya funktioner och uppdateringar för kvalitet. 