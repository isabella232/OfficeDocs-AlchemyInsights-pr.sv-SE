---
title: Distribuera Teams som fristående eller med nya eller befintliga Office installationer
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320140"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Distribuera Teams som fristående eller med nya eller befintliga Office installationer

Microsoft Teams ingår nu i nya ***installationer av*** Microsoft 365-appar för företag, Microsoft 365-applikationer för affärsverksamhet och Office för Mac. Mer information finns i [När Microsoft Teams inkluderas i nya installationer av Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Från och med version 1906 i aktuell kanal  kommer Teams dessutom att läggas till i befintliga installationer av Microsoft 365-appar för företag (och Microsoft 365-applikationer för affärsverksamhet) på enheter med Windows när du uppdaterar din befintliga installation till den senaste versionen. Mer information finns i [Vad gäller för befintliga installationer av Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Obs!** Om du inte vill vänta på det här distributionsschemat kan du distribuera Teams [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) som fristående för användarna genom att följa de här anvisningarna eller så kan du be användarna installera Teams själva från [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Om din organisation inte är redo att distribuera Teams har vi de steg du [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) kan [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) vidta för att utesluta ***Teams*** från nya eller befintliga installationer av Office. Om du Teams installeras men inte vill att Teams startas automatiskt för användaren när den har installerats går du till Förhindra [att Microsoft Teams startas](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)automatiskt efter installationen .

Information ***om Teams*** från en enhet med Windows finns i Avinstallera [Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Information om hur Microsoft Teams bort från flera måldatorer eller -användare finns [Microsoft Teams i Rensa vid distribution.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Om du använder delade datorer, Fjärrskrivbordstjänster (RDS) eller VDI (Virtual Desktop Infrastructure) kan du gå till Delade datorer och [VDI-miljöer med Microsoft Teams.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

Om du använder en mac Office för Mac se [hur Microsoft Teams på en Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

**Obs!** Teams installeras uppdateras den automatiskt [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) ungefär varannan vecka med nya funktioner och kvalitetsuppdateringar. 