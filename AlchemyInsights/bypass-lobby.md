---
title: Bypass lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768458"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Kontrollera Lobbyinställningar och deltagarnivå

Om du vill tillåta alla, inklusive fjärråtkomst, externa och anonyma användare att kringgå lobbyn i Microsoft Teams, kan du använda PowerShell för att göra det. Här är ett exempel på hur du ändrar den globala Mötes policyn för din organisation:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Denna cmdlet kräver för närvarande användning av Skype för Business PowerShell-modulen. Om du vill få installationsprogrammet att använda denna cmdlet, checka ut [Hantera principer via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Du kan ställa in en ny princip, som du sedan måste använda den för användare. Om du ändrar den globala policyn tillämpas den automatiskt på användare. För alla principändringar måste du vänta minst 4 timmar och upp till 24 timmar för att policyerna ska börja gälla.

Se till att granska dokumentationen nedan innan du gör dessa ändringar för att förstå exakt vad detta tillåter.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Förstå team som uppfyller lobby policykontroller

- Ta [automatiskt emot personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) är en per organisatör-princip som styr om personer ansluter till ett möte direkt eller väntar i lobbyn tills de är antagna av en autentiserad användare.

- [Tillåt anonyma personer att starta ett möte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) är en per-organisatörsprincip som styr om anonyma personer, inklusive B2B och federerade användare, kan ansluta sig till användarens möte utan en autentiserad användare från organisationen i närvaro.

- [Tillåt uppringda användare att kringgå lobbyn](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) är en per-organisatör politik som styr om personer som ringer in via telefon ansluta till mötet direkt eller vänta i lobbyn oavsett den **automatiskt erkänna folk** inställningen.

- [Tillåt organisatörer att åsidosätta Lobbyinställningar](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) är en per-Organizer-princip som styr om mötesorganisatören kan åsidosätta lobby inställningarna som en administratör ställer in **automatiskt medger personer** och **tillåter uppringda användare att kringgå lobbyn** när de schemalägger ett nytt möte.

**Anmärkning:** Läs [Hantera Mötes principer i Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) för en fullständig översikt över Mötes principer för Microsoft Teams.
