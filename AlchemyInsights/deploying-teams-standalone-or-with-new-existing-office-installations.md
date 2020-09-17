---
title: Distribuera team som fristående eller med nya eller befintliga Office-installationer
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
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806777"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Distribuera team som fristående eller med nya eller befintliga Office-installationer

Microsoft Teams är nu inkluderat som en del av ***nya installationer*** av Microsoft 365-appar för Enterprise, Microsoft 365-appar för företag och Office för Mac. För mer information, se [när kommer Microsoft Teams att börja ingå i nya installationer av Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Från och med version 1906 i aktuell kanal kommer team att ***läggas till i befintliga installationer*** av Microsoft 365-appar för Enterprise (och Microsoft 365-appar för företag) på enheter med Windows när du uppdaterar din befintliga installation till den senaste versionen. Mer information finns i [Vad händer med befintliga installationer av Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Om du inte vill vänta på detta installations schema kan du distribuera Teams som fristående för användarna genom att [följa de här anvisningarna](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   , eller så kan du låta användarna installera Teams från  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Om din organisation inte är redo att distribuera Teams har vi de steg du kan vidta för att ***exkludera team*** från [nya](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) eller [befintliga](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office-installationer. Om du vill att team ska installeras, men inte vill att teamen ska starta automatiskt för användaren när det är installerat, kan du läsa [förhindra att Microsoft Teams startas automatiskt efter installationen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Information om hur du ***avinstallerar Teams*** från en enhet med Windows finns i [Avinstallera Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Information om hur du rensar Microsoft Teams från flera mål datorer eller användare finns i [Microsoft Teams Deployment Cleanup](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Om du använder delade datorer, fjärr skrivbords tjänster eller virtuella Skriv bords infrastruktur (VDI) kan du läsa [dela dator och VDI-miljöer med Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Om du använder Office för Mac läser du [Microsoft Teams-installationer på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> När Teams har installerats uppdateras det [automatiskt](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) cirka två veckor med nya funktioner och kvalitets uppdateringar. 