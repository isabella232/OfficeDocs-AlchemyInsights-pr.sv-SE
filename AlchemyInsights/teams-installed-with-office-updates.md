---
title: Teams installerade med Office-uppdateringar
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
ms.openlocfilehash: 36b0b1a7bf37c27304b4124157dba9aba337678c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832400"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>Microsoft Teams installerade med Office-uppdateringar

Microsoft Teams ingår som en del av ***nya installationer*** av Microsoft 365-appar för företag, Microsoft 365-appar för företag och Office för Mac. Mer information finns i [När börjar Microsoft Teams inkluderas i nya installationer av Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Från och med version 1906 i aktuell kanal kommer  Teams gradvis att läggas till i befintliga installationer av Microsoft 365-appar för företag (och Microsoft 365-appar för företag) på enheter som kör Windows när du uppdaterar din befintliga installation till den senaste versionen. Mer information finns i [Vad är befintliga installationer av Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Obs!** Om du inte vill vänta på det här distributionsschemat kan du distribuera [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)Teams som fristående för användarna genom att följa de här anvisningarna, eller så kan användarna installera Teams själva från https://teams.microsoft.com/downloads .

Om din organisation inte är redo att distribuera Teams kan du utesluta ***Teams*** från [nya eller](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) [befintliga](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installationer av Office. Om du vill att Teams ska installeras, men inte vill att Teams ska starta automatiskt för användaren när det har installerats, se Förhindra att Microsoft Teams startar automatiskt [efter installationen.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Om ***du vill avinstallera Teams*** från en enhet med Windows, se Avinstallera Microsoft [Teams](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81). Information om hur du rensar upp Microsoft Teams från flera måldatorer eller -användare finns i [Rensning av Microsoft Teams-distribution.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Om du använder delade datorer, Fjärrskrivbordstjänster (RDS) eller VDI (Virtual Desktop Infrastructure) kan du gå till Delade datorer och [VDI-miljöer med Microsoft Teams.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams) Om du använder Office för Mac kan du gå till [Microsoft Teams-installationer på en Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

**Obs!** När Teams har installerats uppdateras det [automatiskt ungefär](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) varannan vecka med nya funktioner och kvalitetsuppdateringar. 