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
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768458"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="c55fd-102">Kontrollera Lobbyinställningar och deltagarnivå</span><span class="sxs-lookup"><span data-stu-id="c55fd-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="c55fd-103">Om du vill tillåta alla, inklusive fjärråtkomst, externa och anonyma användare att kringgå lobbyn i Microsoft Teams, kan du använda PowerShell för att göra det.</span><span class="sxs-lookup"><span data-stu-id="c55fd-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="c55fd-104">Här är ett exempel på hur du ändrar den globala Mötes policyn för din organisation:</span><span class="sxs-lookup"><span data-stu-id="c55fd-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="c55fd-105">Denna cmdlet kräver för närvarande användning av Skype för Business PowerShell-modulen.</span><span class="sxs-lookup"><span data-stu-id="c55fd-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="c55fd-106">Om du vill få installationsprogrammet att använda denna cmdlet, checka ut [Hantera principer via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="c55fd-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="c55fd-107">Du kan ställa in en ny princip, som du sedan måste använda den för användare.</span><span class="sxs-lookup"><span data-stu-id="c55fd-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="c55fd-108">Om du ändrar den globala policyn tillämpas den automatiskt på användare.</span><span class="sxs-lookup"><span data-stu-id="c55fd-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="c55fd-109">För alla principändringar måste du vänta minst 4 timmar och upp till 24 timmar för att policyerna ska börja gälla.</span><span class="sxs-lookup"><span data-stu-id="c55fd-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="c55fd-110">Se till att granska dokumentationen nedan innan du gör dessa ändringar för att förstå exakt vad detta tillåter.</span><span class="sxs-lookup"><span data-stu-id="c55fd-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="c55fd-111">Förstå team som uppfyller lobby policykontroller</span><span class="sxs-lookup"><span data-stu-id="c55fd-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="c55fd-112">Ta [automatiskt emot personer](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) är en per organisatör-princip som styr om personer ansluter till ett möte direkt eller väntar i lobbyn tills de är antagna av en autentiserad användare.</span><span class="sxs-lookup"><span data-stu-id="c55fd-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="c55fd-113">[Tillåt anonyma personer att starta ett möte](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) är en per-organisatörsprincip som styr om anonyma personer, inklusive B2B och federerade användare, kan ansluta sig till användarens möte utan en autentiserad användare från organisationen i närvaro.</span><span class="sxs-lookup"><span data-stu-id="c55fd-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="c55fd-114">[Tillåt uppringda användare att kringgå lobbyn](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kommer snart**) är en per-organisatör politik som styr om personer som ringer in via telefon ansluta till mötet direkt eller vänta i lobbyn oavsett den **automatiskt erkänna folk** inställningen.</span><span class="sxs-lookup"><span data-stu-id="c55fd-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="c55fd-115">[Tillåt organisatörer att åsidosätta Lobbyinställningar](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kommer snart**) är en per-Organizer-princip som styr om mötesorganisatören kan åsidosätta lobby inställningarna som en administratör har angett i **automatiskt medger att personer** och **tillåter fjärråtkomst användare att kringgå lobbyn** när de schemalägger ett nytt möte.</span><span class="sxs-lookup"><span data-stu-id="c55fd-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="c55fd-116">**Anmärkning:** Läs [Hantera Mötes principer i Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) för en fullständig översikt över Mötes principer för Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c55fd-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
