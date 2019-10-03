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
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="b05db-102">Kontrollera Lobbyinställningar och deltagarnivå</span><span class="sxs-lookup"><span data-stu-id="b05db-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="b05db-103">Dessa inställningar styr vilka mötesdeltagare som väntar i lobbyn innan de är antagna till mötet och vilken deltagarnivå de är tillåtna i ett möte.</span><span class="sxs-lookup"><span data-stu-id="b05db-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="b05db-104">Du kan använda PowerShell för att uppdatera Mötes principinställningar som ännu inte har implementerats (märkt "kommer snart") i Teams administratörscenter.</span><span class="sxs-lookup"><span data-stu-id="b05db-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="b05db-105">Se nedan för ett exempel PowerShell-cmdlet som tillåter alla användare att kringgå lobbyn.</span><span class="sxs-lookup"><span data-stu-id="b05db-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="b05db-106">Ta [automatiskt emot personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) är en per organisatör-princip som styr om personer ansluter till ett möte direkt eller väntar i lobbyn tills de är antagna av en autentiserad användare.</span><span class="sxs-lookup"><span data-stu-id="b05db-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="b05db-107">[Tillåt anonyma personer att starta ett möte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) är en per-organisatörsprincip som styr om anonyma personer, inklusive B2B och federerade användare, kan ansluta sig till användarens möte utan en autentiserad användare från organisationen i närvaro.</span><span class="sxs-lookup"><span data-stu-id="b05db-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="b05db-108">[Tillåt uppringda användare att kringgå lobbyn](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) är en per-organisatör politik som styr om personer som ringer in via telefon ansluta till mötet direkt eller vänta i lobbyn oavsett den **automatiskt erkänna folk** inställningen.</span><span class="sxs-lookup"><span data-stu-id="b05db-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="b05db-109">[Tillåt organisatörer att åsidosätta Lobbyinställningar](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) är en per-Organizer-princip som styr om mötesorganisatören kan åsidosätta lobby inställningarna som en administratör har angett i **automatiskt medger att personer** och **tillåter fjärråtkomst användare att kringgå lobbyn** när de schemalägger ett nytt möte.</span><span class="sxs-lookup"><span data-stu-id="b05db-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="b05db-110">**Anmärkning:** Läs [Hantera Mötes principer i Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) för en fullständig översikt över Mötes principer för Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b05db-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="b05db-111">**PowerShell-exempel**</span><span class="sxs-lookup"><span data-stu-id="b05db-111">**PowerShell example**</span></span>

<span data-ttu-id="b05db-112">Om du vill tillåta alla, inklusive externa eller anonyma användare, att kringgå lobbyn, kan du också använda PowerShell för att utföra den här uppgiften.</span><span class="sxs-lookup"><span data-stu-id="b05db-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="b05db-113">Här är ett exempel på hur du ändrar den globala Mötes policyn för din organisation.</span><span class="sxs-lookup"><span data-stu-id="b05db-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="b05db-114">(Se till att granska dokumentationen ovan innan du gör dessa ändringar för att förstå exakt vad detta tillåter.)</span><span class="sxs-lookup"><span data-stu-id="b05db-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="b05db-115">Set-CsTeamsMeetingPolicy-identitet global-AutoAdmittedUsers "alla"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="b05db-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="b05db-116">Mer information finns [i set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="b05db-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
