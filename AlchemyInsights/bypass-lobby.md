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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="c0ec1-102">Kontrollera Lobbyinställningar och deltagarnivå i Teams</span><span class="sxs-lookup"><span data-stu-id="c0ec1-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="c0ec1-103">Om du vill tillåta alla, inklusive fjärråtkomst, externa och anonyma användare, att **kringgå lobbyn**, kan du använda PowerShell för att utföra den här uppgiften.</span><span class="sxs-lookup"><span data-stu-id="c0ec1-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="c0ec1-104">Här är ett exempel på hur du ändrar den globala Mötes policyn för din organisation.</span><span class="sxs-lookup"><span data-stu-id="c0ec1-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="c0ec1-105">Denna cmdlet kräver för närvarande användning av Skype för Business PowerShell-modulen.</span><span class="sxs-lookup"><span data-stu-id="c0ec1-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="c0ec1-106">För att få ställa in att använda denna cmdlet, checka ut [Hantera principer via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="c0ec1-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="c0ec1-107">När du har konfigurerat en princip måste du använda den för användare. eller, om du har ändrat den globala principen, kommer den automatiskt att gälla för användare.</span><span class="sxs-lookup"><span data-stu-id="c0ec1-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="c0ec1-108">För alla principändringar måste du vänta minst **4 timmar upp till 24 timmar** för att policyerna ska börja gälla.</span><span class="sxs-lookup"><span data-stu-id="c0ec1-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="c0ec1-109">Se till att granska dokumentationen nedan innan du gör dessa ändringar för att förstå exakt vad detta tillåter.</span><span class="sxs-lookup"><span data-stu-id="c0ec1-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="c0ec1-110">Förstå team som uppfyller lobby policykontroller</span><span class="sxs-lookup"><span data-stu-id="c0ec1-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="c0ec1-111">Dessa inställningar styr vilka mötesdeltagare som väntar i lobbyn innan de är antagna till mötet och vilken deltagarnivå de är tillåtna i ett möte.</span><span class="sxs-lookup"><span data-stu-id="c0ec1-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="c0ec1-112">Du kan använda PowerShell för att uppdatera Mötes principinställningar som ännu inte har implementerats (märkt "kommer snart") i Teams administratörscenter.</span><span class="sxs-lookup"><span data-stu-id="c0ec1-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="c0ec1-113">Se nedan för ett exempel PowerShell-cmdlet som tillåter alla användare att kringgå lobbyn.</span><span class="sxs-lookup"><span data-stu-id="c0ec1-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="c0ec1-114">Ta [automatiskt emot personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) är en per organisatör-princip som styr om personer ansluter till ett möte direkt eller väntar i lobbyn tills de är antagna av en autentiserad användare.</span><span class="sxs-lookup"><span data-stu-id="c0ec1-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="c0ec1-115">[Tillåt anonyma personer att starta ett möte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) är en per-organisatörsprincip som styr om anonyma personer, inklusive B2B och federerade användare, kan ansluta sig till användarens möte utan en autentiserad användare från organisationen i närvaro.</span><span class="sxs-lookup"><span data-stu-id="c0ec1-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="c0ec1-116">[Tillåt uppringda användare att kringgå lobbyn](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) är en per-organisatör politik som styr om personer som ringer in via telefon ansluta till mötet direkt eller vänta i lobbyn oavsett den **automatiskt erkänna folk** inställningen.</span><span class="sxs-lookup"><span data-stu-id="c0ec1-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="c0ec1-117">[Tillåt organisatörer att åsidosätta Lobbyinställningar](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) är en per-Organizer-princip som styr om mötesorganisatören kan åsidosätta lobby inställningarna som en administratör ställer in **automatiskt medger personer** och **tillåter uppringda användare att kringgå lobbyn** när de schemalägger ett nytt möte.</span><span class="sxs-lookup"><span data-stu-id="c0ec1-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="c0ec1-118">**Anmärkning:** Läs [Hantera Mötes principer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) för en fullständig översikt över Mötes principer för Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c0ec1-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
