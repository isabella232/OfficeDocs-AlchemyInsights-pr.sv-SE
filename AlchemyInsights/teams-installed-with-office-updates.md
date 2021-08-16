---
title: Teams installeras med Office uppdateringar
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
- "2599"
- "9000140"
- "9000660"
- "2509"
ms.openlocfilehash: c473a001d1441362baad9feb44323b46f1cef42d3c431ef87f0fb0172f10d152
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048750"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>Microsoft Teams installeras med Office uppdateringar

Microsoft Teams ingår som en del ***av nya installationer*** av Microsoft 365-appar för företag, Microsoft 365-applikationer för affärsverksamhet och Office för Mac. Mer information finns i [När börjar Microsoft Teams inkluderas i nya installationer av Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Från och med version 1906 i aktuell kanal kommer Teams  dessutom gradvis att läggas till i befintliga installationer av Microsoft 365-appar för företag (och Microsoft 365-applikationer för affärsverksamhet) på enheter som kör Windows när du uppdaterar din befintliga installation till den senaste versionen. Mer information finns i [Vad gäller för befintliga installationer Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Obs!** Om du inte vill vänta på det här distributionsschemat kan du distribuera Teams [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)som fristående för användarna genom att följa de här anvisningarna, eller så kan du be användarna installera Teams själva från https://teams.microsoft.com/downloads .

Om organisationen inte är redo att distribuera Teams kan du utesluta ***Teams*** från [nya](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) eller [befintliga](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installationer av Office. Om du Teams installeras men inte vill att Teams startas automatiskt för användaren när den har installerats går du till Förhindra [att Microsoft Teams startas](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)automatiskt efter installationen .

Om ***du vill Teams*** från en enhet som kör Windows, se Avinstallera [Microsoft Teams](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81). Information om hur Microsoft Teams från flera måldatorer eller -användare finns [Microsoft Teams i Rensning av distribution.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Om du använder delade datorer, Fjärrskrivbordstjänster (RDS) eller VDI (Virtual Desktop Infrastructure) kan du gå till Delade datorer och [VDI-miljöer med Microsoft Teams.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams) Om du använder en mac Office för Mac se [hur Microsoft Teams på en Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

**Obs!** När Teams installeras uppdateras den [automatiskt](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) ungefär varannan vecka med nya funktioner och kvalitetsuppdateringar. 