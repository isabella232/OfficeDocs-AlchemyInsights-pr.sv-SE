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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376861"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Kontrollera Lobbyinställningar och deltagarnivå

Dessa inställningar styr vilka mötesdeltagare som väntar i lobbyn innan de är antagna till mötet och vilken deltagarnivå de är tillåtna i ett möte. Du kan använda PowerShell för att uppdatera Mötes principinställningar som ännu inte har implementerats (märkt "kommer snart") i Teams administratörscenter.  Se nedan för ett exempel PowerShell-cmdlet som tillåter alla användare att kringgå lobbyn.  

- Ta [automatiskt emot personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) är en per organisatör-princip som styr om personer ansluter till ett möte direkt eller väntar i lobbyn tills de är antagna av en autentiserad användare.

- [Tillåt anonyma personer att starta ett möte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) är en per-organisatörsprincip som styr om anonyma personer, inklusive B2B och federerade användare, kan ansluta sig till användarens möte utan en autentiserad användare från organisationen i närvaro.

- [Tillåt uppringda användare att kringgå lobbyn](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) är en per-organisatör politik som styr om personer som ringer in via telefon ansluta till mötet direkt eller vänta i lobbyn oavsett den **automatiskt erkänna folk** inställningen.

- [Tillåt organisatörer att åsidosätta Lobbyinställningar](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) är en per-Organizer-princip som styr om mötesorganisatören kan åsidosätta lobby inställningarna som en administratör har angett i **automatiskt medger att personer** och **tillåter fjärråtkomst användare att kringgå lobbyn** när de schemalägger ett nytt möte.

**Anmärkning:** Läs [Hantera Mötes principer i Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) för en fullständig översikt över Mötes principer för Microsoft Teams. 


**PowerShell-exempel**

Om du vill tillåta alla, inklusive externa eller anonyma användare, att kringgå lobbyn, kan du också använda PowerShell för att utföra den här uppgiften.  Här är ett exempel på hur du ändrar den globala Mötes policyn för din organisation.   

(Se till att granska dokumentationen ovan innan du gör dessa ändringar för att förstå exakt vad detta tillåter.)

Set-CsTeamsMeetingPolicy-identitet global-AutoAdmittedUsers "alla"-AllowPSTNUsersToBypassLobby $True

Mer information finns [i set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
