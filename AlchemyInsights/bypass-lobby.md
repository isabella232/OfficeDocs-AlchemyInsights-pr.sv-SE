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
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889100"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kontrollera Lobbyinställningar och deltagarnivå i Teams

Om du vill tillåta alla, inklusive fjärråtkomst, externa och anonyma användare, att **kringgå lobbyn**, kan du använda PowerShell för att utföra den här uppgiften. Här är ett exempel på hur du ändrar den globala Mötes policyn för din organisation.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Denna cmdlet kräver för närvarande användning av Skype för Business PowerShell-modulen. För att få ställa in att använda denna cmdlet, checka ut [Hantera principer via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

När du har konfigurerat en princip måste du använda den för användare. eller, om du har ändrat den globala principen, kommer den automatiskt att gälla för användare. För alla principändringar måste du vänta minst **4 timmar upp till 24 timmar** för att policyerna ska börja gälla. 

Se till att granska dokumentationen nedan innan du gör dessa ändringar för att förstå exakt vad detta tillåter.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Förstå team som uppfyller lobby policykontroller

Dessa inställningar styr vilka mötesdeltagare som väntar i lobbyn innan de är antagna till mötet och vilken deltagarnivå de är tillåtna i ett möte. Du kan använda PowerShell för att uppdatera Mötes principinställningar som ännu inte har implementerats (märkt "kommer snart") i Teams administratörscenter. Se nedan för ett exempel PowerShell-cmdlet som tillåter alla användare att kringgå lobbyn.

- Ta [automatiskt emot personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) är en per organisatör-princip som styr om personer ansluter till ett möte direkt eller väntar i lobbyn tills de är antagna av en autentiserad användare.

- [Tillåt anonyma personer att starta ett möte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) är en per-organisatörsprincip som styr om anonyma personer, inklusive B2B och federerade användare, kan ansluta sig till användarens möte utan en autentiserad användare från organisationen i närvaro.

- [Tillåt uppringda användare att kringgå lobbyn](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) är en per-organisatör politik som styr om personer som ringer in via telefon ansluta till mötet direkt eller vänta i lobbyn oavsett den **automatiskt erkänna folk** inställningen.

- [Tillåt organisatörer att åsidosätta Lobbyinställningar](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) är en per-Organizer-princip som styr om mötesorganisatören kan åsidosätta lobby inställningarna som en administratör ställer in **automatiskt medger personer** och **tillåter uppringda användare att kringgå lobbyn** när de schemalägger ett nytt möte.

**Anmärkning:** Läs [Hantera Mötes principer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) för en fullständig översikt över Mötes principer för Microsoft Teams.
