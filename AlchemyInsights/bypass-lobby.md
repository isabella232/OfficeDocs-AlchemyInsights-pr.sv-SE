---
title: Förbikopplingslobbyn
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820052"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kontrollera lobbyinställningar och nivå för deltagande i Teams

Om du vill tillåta att alla, inklusive uppringnings-, externa och anonyma användare, går förbi **lobbyn** kan du använda PowerShell för att utföra den här uppgiften. Här är ett exempel på hur du ändrar den globala mötesprincipen för organisationen.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

För den här cmdleten krävs för närvarande användningen av Skype för företag PowerShell-modulen. Information om hur du kommer igång med att använda denna cmdlet finns i [Hantera principer via PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

När du har skapat en princip måste du tillämpa den på användarna. Eller, om du ändrade den globala principen, kommer den automatiskt att gälla för användare. För alla principförändringar måste du vänta i minst 4 timmar upp till **24 timmar** för att principerna ska gälla. 

Läs dokumentationen nedan innan du gör ändringarna så att du förstår exakt vad som tillåts.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Förstå principkontroller för Teams-möten

De här inställningarna styr vilka mötesdeltagare som väntar i lobbyn innan de tas emot i mötet och i vilken grad de kan delta i ett möte. Du kan använda PowerShell för att uppdatera inställningar för mötesprinciper som ännu inte har implementerats (märkt "kommer snart") i administrationscentret för Teams. Nedan finns en PowerShell-cmdlet som gör att alla användare kan kringgå lobbyn.

- [Automatiskt släppa in personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) är en princip för varje organisatör som styr om personer ansluter till ett möte direkt eller vänta i lobbyn tills de tas emot av en autentiserad användare.

- [Tillåt anonyma](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) personer att starta ett möte är en princip per organisatör som styr om anonyma personer, inklusive B2B och externa användare, kan ansluta till användarens möte utan en autentiserad användare från organisationen som är närvarande.

- [Tillåt att uppringningsanvändare](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) kringgår lobbyn **(kommer** snart) är en princip per organisatör som styr om personer som  ringer in via telefon ansluts direkt eller väntar i lobbyn oavsett inställningen Tillåt automatiskt personer.

- Tillåt att organisatörer åsidosätter lobbyinställningar (kommer snart) är en princip per organisatör som  styr huruvida mötesorganisatören kan åsidosätta [lobbyinställningarna](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) som en administratör anger i Tillåt automatiskt uppringning att användare kringgår lobbyn när de schemalägger ett nytt möte. 

**Obs!** Läs [Hantera mötes principer i Teams för](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) en fullständig översikt över Mötesprinciper för Microsoft Teams.
