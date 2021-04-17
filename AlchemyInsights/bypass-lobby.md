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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="1ade1-102">Kontrollera lobbyinställningar och nivå för deltagande i Teams</span><span class="sxs-lookup"><span data-stu-id="1ade1-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="1ade1-103">Om du vill tillåta att alla, inklusive uppringnings-, externa och anonyma användare, går förbi **lobbyn** kan du använda PowerShell för att utföra den här uppgiften.</span><span class="sxs-lookup"><span data-stu-id="1ade1-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="1ade1-104">Här är ett exempel på hur du ändrar den globala mötesprincipen för organisationen.</span><span class="sxs-lookup"><span data-stu-id="1ade1-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="1ade1-105">För den här cmdleten krävs för närvarande användningen av Skype för företag PowerShell-modulen.</span><span class="sxs-lookup"><span data-stu-id="1ade1-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="1ade1-106">Information om hur du kommer igång med att använda denna cmdlet finns i [Hantera principer via PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="1ade1-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="1ade1-107">När du har skapat en princip måste du tillämpa den på användarna. Eller, om du ändrade den globala principen, kommer den automatiskt att gälla för användare.</span><span class="sxs-lookup"><span data-stu-id="1ade1-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="1ade1-108">För alla principförändringar måste du vänta i minst 4 timmar upp till **24 timmar** för att principerna ska gälla.</span><span class="sxs-lookup"><span data-stu-id="1ade1-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="1ade1-109">Läs dokumentationen nedan innan du gör ändringarna så att du förstår exakt vad som tillåts.</span><span class="sxs-lookup"><span data-stu-id="1ade1-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="1ade1-110">Förstå principkontroller för Teams-möten</span><span class="sxs-lookup"><span data-stu-id="1ade1-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="1ade1-111">De här inställningarna styr vilka mötesdeltagare som väntar i lobbyn innan de tas emot i mötet och i vilken grad de kan delta i ett möte.</span><span class="sxs-lookup"><span data-stu-id="1ade1-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="1ade1-112">Du kan använda PowerShell för att uppdatera inställningar för mötesprinciper som ännu inte har implementerats (märkt "kommer snart") i administrationscentret för Teams.</span><span class="sxs-lookup"><span data-stu-id="1ade1-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="1ade1-113">Nedan finns en PowerShell-cmdlet som gör att alla användare kan kringgå lobbyn.</span><span class="sxs-lookup"><span data-stu-id="1ade1-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="1ade1-114">[Automatiskt släppa in personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) är en princip för varje organisatör som styr om personer ansluter till ett möte direkt eller vänta i lobbyn tills de tas emot av en autentiserad användare.</span><span class="sxs-lookup"><span data-stu-id="1ade1-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="1ade1-115">[Tillåt anonyma](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) personer att starta ett möte är en princip per organisatör som styr om anonyma personer, inklusive B2B och externa användare, kan ansluta till användarens möte utan en autentiserad användare från organisationen som är närvarande.</span><span class="sxs-lookup"><span data-stu-id="1ade1-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="1ade1-116">[Tillåt att uppringningsanvändare](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) kringgår lobbyn **(kommer** snart) är en princip per organisatör som styr om personer som  ringer in via telefon ansluts direkt eller väntar i lobbyn oavsett inställningen Tillåt automatiskt personer.</span><span class="sxs-lookup"><span data-stu-id="1ade1-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="1ade1-117">Tillåt att organisatörer åsidosätter lobbyinställningar (kommer snart) är en princip per organisatör som  styr huruvida mötesorganisatören kan åsidosätta [lobbyinställningarna](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) som en administratör anger i Tillåt automatiskt uppringning att användare kringgår lobbyn när de schemalägger ett nytt möte. </span><span class="sxs-lookup"><span data-stu-id="1ade1-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="1ade1-118">**Obs!** Läs [Hantera mötes principer i Teams för](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) en fullständig översikt över Mötesprinciper för Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1ade1-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
