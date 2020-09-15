---
title: Gå förbi lobbyn
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684968"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kontrol lera lobbyn och nivå för deltagande i Teams

Om du vill tillåta alla, inklusive uppringnings-och externa användare, **kan du använda**PowerShell för att utföra den här åtgärden. Här är ett exempel på hur du ändrar den globala Mötes principen för organisationen.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Denna cmdlet kräver att PowerShell-modulen för Skype för företag används för närvarande. Om du vill konfigurera för att använda denna cmdlet läser du [Hantera principer via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

När du har konfigurerat en princip måste du tillämpa den på användarna; Om du har ändrat den globala principen används den automatiskt för användarna. För att principer ska ändras måste du vänta minst **4 timmar upp till 24 timmar** innan principerna börjar gälla. 

Se till att läsa dokumentationen nedan innan du gör de här ändringarna för att förstå exakt vad det innebär.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Förstå Teams kontroller för arbets lag och lobbyn

Dessa inställningar styr vilka Mötes deltagare som väntar i lobbyn innan de tillåts delta i mötet och vilken nivå det deltar i mötet. Du kan använda PowerShell för att uppdatera Mötes princip inställningar som ännu inte har implementerats (med etiketten "kommer snart") i administrations centret för Teams. Se nedan för ett exempel på en PowerShell-cmdlet som tillåter alla användare att gå förbi lobbyn.

- Att [automatiskt tillåta personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) är en princip för varje organisatör som styr om personer ansluter direkt till ett möte eller väntar i lobbyn tills de tillåts av en autentiserad användare.

- [Tillåt anonyma användare att starta ett möte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) är en princip för varje organisatör som styr om anonyma personer, inklusive B2B och federerade användare, kan gå med i användarens möten utan en autentiserad användare från organisationen i närvaro.

- [Tillåt att uppringda användare kringgår lobbyn](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) är en regel som styr om personer som ringer via telefon ansluter till mötet direkt eller väntar i lobbyn oavsett vilken inställning som ställs in **automatiskt** .

- [Tillåt att organisatörer åsidosätter inställningarna för lobbyn](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) är en princip för en viss organisatör som styr om mötesorganisatören kan åsidosätta lobbyn-inställningarna som en administratör ställer in **automatiskt** **för att godkänna personer och tillåta att uppringda användare kringgår lobbyn** när de schemalägger ett nytt möte.

**Obs!** Läs [Hantera Mötes principer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) för en fullständig översikt över Microsoft Teams Mötes principer.
