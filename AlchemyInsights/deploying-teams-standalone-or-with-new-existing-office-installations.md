---
title: Distribuera team som fristående eller med nya eller befintliga Office-installationer
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 4b843407f05db207f3b676c03c7088d3d0ba062e
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704651"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Distribuera team som fristående eller med nya eller befintliga Office-installationer

Microsoft Teams ingår nu som en del av ***nya installationer*** av Microsoft 365 Apps for Enterprise, Microsoft 365 Apps for business och Office för Mac. Mer information finns i [När kommer Microsoft Teams att börja inkluderas i nya installationer av Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Från och med version 1906 i månadskanal läggs Teams dessutom ***till i befintliga installationer*** av Microsoft 365 Apps for Enterprise (och Microsoft 365 Apps for business) på enheter som kör Windows när du uppdaterar den befintliga installationen till den senaste versionen. Mer information finns i [Hur är det med befintliga installationer av Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Om du inte vill vänta på det här distributionsschemat kan du distribuera Teams som fristående för användarna genom att [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)följa dessa [instruktioner](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) eller låta användarna installera Teams för sig själva från .

Om din organisation inte är redo att distribuera Teams har vi de åtgärder du kan vidta för att ***utesluta Teams*** från [nya](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) eller [befintliga](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installationer av Office. Om du vill att Teams ska installeras, men inte vill att Teams ska starta automatiskt för användaren när den har installerats, läser du Förhindra att [Microsoft Teams startar automatiskt efter installationen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Information om hur du ***avinstallerar Teams*** från en enhet som kör Windows finns i [Avinstallera Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Om du vill rensa Microsoft Teams från flera måldatorer eller användare läser du [rensning av Microsoft Teams-distribution.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Om du använder delade datorer, Fjärrskrivbordstjänster (RDS) eller VIRTUELL SKRIVBORDsinfrastruktur (VDI) läser du [Delade dator- och VDI-miljöer med Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Om du använder Office för Mac läser du [Microsoft Teams-installationer på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> När Teams har installerats [uppdateras](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) det automatiskt ungefär varannan vecka med nya funktioner och kvalitetsuppdateringar. 