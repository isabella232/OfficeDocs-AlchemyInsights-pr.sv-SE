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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="81a17-102">Kontrol lera lobbyn och nivå för deltagande i Teams</span><span class="sxs-lookup"><span data-stu-id="81a17-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="81a17-103">Om du vill tillåta alla, inklusive uppringnings-och externa användare, **kan du använda**PowerShell för att utföra den här åtgärden.</span><span class="sxs-lookup"><span data-stu-id="81a17-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="81a17-104">Här är ett exempel på hur du ändrar den globala Mötes principen för organisationen.</span><span class="sxs-lookup"><span data-stu-id="81a17-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="81a17-105">Denna cmdlet kräver att PowerShell-modulen för Skype för företag används för närvarande.</span><span class="sxs-lookup"><span data-stu-id="81a17-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="81a17-106">Om du vill konfigurera för att använda denna cmdlet läser du [Hantera principer via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="81a17-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="81a17-107">När du har konfigurerat en princip måste du tillämpa den på användarna; Om du har ändrat den globala principen används den automatiskt för användarna.</span><span class="sxs-lookup"><span data-stu-id="81a17-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="81a17-108">För att principer ska ändras måste du vänta minst **4 timmar upp till 24 timmar** innan principerna börjar gälla.</span><span class="sxs-lookup"><span data-stu-id="81a17-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="81a17-109">Se till att läsa dokumentationen nedan innan du gör de här ändringarna för att förstå exakt vad det innebär.</span><span class="sxs-lookup"><span data-stu-id="81a17-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="81a17-110">Förstå Teams kontroller för arbets lag och lobbyn</span><span class="sxs-lookup"><span data-stu-id="81a17-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="81a17-111">Dessa inställningar styr vilka Mötes deltagare som väntar i lobbyn innan de tillåts delta i mötet och vilken nivå det deltar i mötet.</span><span class="sxs-lookup"><span data-stu-id="81a17-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="81a17-112">Du kan använda PowerShell för att uppdatera Mötes princip inställningar som ännu inte har implementerats (med etiketten "kommer snart") i administrations centret för Teams.</span><span class="sxs-lookup"><span data-stu-id="81a17-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="81a17-113">Se nedan för ett exempel på en PowerShell-cmdlet som tillåter alla användare att gå förbi lobbyn.</span><span class="sxs-lookup"><span data-stu-id="81a17-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="81a17-114">Att [automatiskt tillåta personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) är en princip för varje organisatör som styr om personer ansluter direkt till ett möte eller väntar i lobbyn tills de tillåts av en autentiserad användare.</span><span class="sxs-lookup"><span data-stu-id="81a17-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="81a17-115">[Tillåt anonyma användare att starta ett möte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) är en princip för varje organisatör som styr om anonyma personer, inklusive B2B och federerade användare, kan gå med i användarens möten utan en autentiserad användare från organisationen i närvaro.</span><span class="sxs-lookup"><span data-stu-id="81a17-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="81a17-116">[Tillåt att uppringda användare kringgår lobbyn](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) är en regel som styr om personer som ringer via telefon ansluter till mötet direkt eller väntar i lobbyn oavsett vilken inställning som ställs in **automatiskt** .</span><span class="sxs-lookup"><span data-stu-id="81a17-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="81a17-117">[Tillåt att organisatörer åsidosätter inställningarna för lobbyn](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) är en princip för en viss organisatör som styr om mötesorganisatören kan åsidosätta lobbyn-inställningarna som en administratör ställer in **automatiskt** **för att godkänna personer och tillåta att uppringda användare kringgår lobbyn** när de schemalägger ett nytt möte.</span><span class="sxs-lookup"><span data-stu-id="81a17-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="81a17-118">**Obs!** Läs [Hantera Mötes principer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) för en fullständig översikt över Microsoft Teams Mötes principer.</span><span class="sxs-lookup"><span data-stu-id="81a17-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
