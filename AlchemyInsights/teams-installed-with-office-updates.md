---
title: Team installerade med Office-uppdateringar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2599"
- "9000140"
- "9000660"
- "2509"
ms.openlocfilehash: 6f45dbdbfa89711fa2472a1f0b9f8e630faeb91e
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2020
ms.locfileid: "42599502"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>Microsoft Teams installeras med Office-uppdateringar

Microsoft Teams ingår som en del av ***nya installationer*** av Office 365 ProPlus, Office 365 Business och Office för Mac. Mer information finns i [När kommer Microsoft Teams att börja inkluderas i nya installationer av Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Dessutom, från och med version 1906 i Månadskanal, kommer teams gradvis att läggas till ***befintliga installationer*** av Office 365 ProPlus (och Office 365 Business) på enheter som kör Windows när du uppdaterar din befintliga installation till den senaste versionen. Mer information finns i [Hur är det med befintliga installationer av Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

**Obs:** Om du inte vill vänta på det här utrullningsschemat kan du distribuera Teams som fristående för användarna genom att https://teams.microsoft.com/downloadsfölja dessa [instruktioner](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)eller så kan användarna installera Teams själva från .

Om din organisation inte är redo att distribuera team kan du ***utesluta team*** från [nya](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) eller [befintliga](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installationer av Office. Om du vill att Teams ska installeras, men inte vill att Teams ska starta automatiskt för användaren när de har installerats, läser du Förhindra att [Microsoft Teams startar automatiskt efter installationen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Information om hur du ***avinstallerar Team*** från en enhet som kör Windows finns i [Avinstallera Microsoft Teams](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81). Information om hur du rensar Microsoft Teams från flera måldatorer eller användare finns i [Microsoft Teams-distributionsrensning](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Om du använder delade datorer, fjärrskrivbordstjänster (RDS) eller Virtual Desktop Infrastructure (VDI) läser du [miljöer med delad dator och VDI med Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams). Om du använder Office för Mac läser du [Microsoft Teams-installationer på en Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**Obs:** När Teams har installerats [uppdateras](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) den automatiskt ungefär varannan vecka med nya funktioner och kvalitetsuppdateringar. 