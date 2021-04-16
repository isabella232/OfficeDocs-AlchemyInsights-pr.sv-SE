---
title: Börja använda livehändelser i Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811978"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="9cd5e-102">Börja använda livehändelser i Teams</span><span class="sxs-lookup"><span data-stu-id="9cd5e-102">Getting started with Teams live events</span></span>

<span data-ttu-id="9cd5e-103">Microsoft Teams livehändelser är ett tillägg till Teams-möten som gör att du kan schemalägga och skapa händelser som strömmas till stora åhörargrupper online.</span><span class="sxs-lookup"><span data-stu-id="9cd5e-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="9cd5e-104">Om du vill skapa en livehändelse behöver du följande:</span><span class="sxs-lookup"><span data-stu-id="9cd5e-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="9cd5e-105">Bekräfta först att Teams Livehändelser är [tillgängliga i ditt land och din region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Livehändelser stöds ännu inte i vissa länder.</span><span class="sxs-lookup"><span data-stu-id="9cd5e-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="9cd5e-106">Om du har tilldelat licenser och angett principer, men fortfarande inte kan skapa en Teams livehändelse, är det troligt att du befinner dig i ett land eller en region där livehändelser inte är tillgängliga ännu.</span><span class="sxs-lookup"><span data-stu-id="9cd5e-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="9cd5e-107">En licens för [Office 365 Enterprise, E1, E3 eller E5 eller en licens för Office 365 A3 eller A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="9cd5e-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="9cd5e-108">**Obs!** På grund av den nyliga ökningen av Teams-användningen kan det ta cirka 24 timmar innan en användare är helt aktiverad efter det att du tilldelat en Teams-licens.</span><span class="sxs-lookup"><span data-stu-id="9cd5e-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="9cd5e-109">Du kan inte tilldela Teams-principer till dem och de kanske inte har tillgång till vissa Teams-funktioner som samtal och ljudkonferenser förrän de aktiverats helt.</span><span class="sxs-lookup"><span data-stu-id="9cd5e-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="9cd5e-110">Behörighet att [skapa livehändelser i administrationscentret för Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="9cd5e-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="9cd5e-111">Behörighet att [skapa livehändelser i Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (för händelser som skapas med en extern sändningsapp eller enhet).</span><span class="sxs-lookup"><span data-stu-id="9cd5e-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="9cd5e-112">Fullständigt gruppmedlemskap i organisationen (får inte vara gäst eller från en annan organisation).</span><span class="sxs-lookup"><span data-stu-id="9cd5e-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="9cd5e-113">Schemaläggning av privata möten, skärmdelning och IP-videodelning är aktiverat i principen för Teams-möten.</span><span class="sxs-lookup"><span data-stu-id="9cd5e-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="9cd5e-114">[Metodtips](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) för livehändelser i Teams.</span><span class="sxs-lookup"><span data-stu-id="9cd5e-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="9cd5e-115">Om du vill ha mer information kan du läsa [Komma igång med livehändelser i Microsoft Teams](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="9cd5e-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>