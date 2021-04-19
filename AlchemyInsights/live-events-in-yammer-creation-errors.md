---
title: Fel när livehändelser ska skapas i Yammer
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
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825533"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="669fb-102">Fel när livehändelser ska skapas i Yammer</span><span class="sxs-lookup"><span data-stu-id="669fb-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="669fb-103">**Skapa en livehändelse i Yammer**</span><span class="sxs-lookup"><span data-stu-id="669fb-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="669fb-104">Alternativet för att skapa en livehändelse visas alltid i Yammer.</span><span class="sxs-lookup"><span data-stu-id="669fb-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="669fb-105">I vissa fall kanske inte användare uppfyller kraven för att skapa en livehändelse och de får då ett felmeddelande när de försöker skapa den.</span><span class="sxs-lookup"><span data-stu-id="669fb-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="669fb-106">Nedan hittar du vanliga orsaker för det här problemet och olika sätt att lösa det för slutanvändarna.</span><span class="sxs-lookup"><span data-stu-id="669fb-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="669fb-107">**Vem kan skapa livehändelser**</span><span class="sxs-lookup"><span data-stu-id="669fb-107">**Who can create live events**</span></span>
- <span data-ttu-id="669fb-108">En licens för Office 365 Enterprise E1, E3 eller E5 eller en licens för Office 365 A3 eller A5.</span><span class="sxs-lookup"><span data-stu-id="669fb-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="669fb-109">Behörighet att skapa livehändelser i administrationscentret för Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="669fb-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="669fb-110">Behörighet att skapa livehändelser i Microsoft Stream (för händelser som produceras med en extern sändningsapp eller enhet).</span><span class="sxs-lookup"><span data-stu-id="669fb-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="669fb-111">Fullständigt gruppmedlemskap i organisationen (får inte vara gäst eller från en annan organisation).</span><span class="sxs-lookup"><span data-stu-id="669fb-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="669fb-112">Schemaläggning av privata möten, skärmdelning och IP-videodelning är aktiverat i principen för Teams-möten.</span><span class="sxs-lookup"><span data-stu-id="669fb-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="669fb-113">**Principer för att skapa livehändelser**</span><span class="sxs-lookup"><span data-stu-id="669fb-113">**Live event creation policies**</span></span>

<span data-ttu-id="669fb-114">Yammer följer de principer för livehändelser som anges i Office 365-klientorganisationen för Stream.</span><span class="sxs-lookup"><span data-stu-id="669fb-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="669fb-115">Som standard kan alla i din organisation skapa en livehändelse.</span><span class="sxs-lookup"><span data-stu-id="669fb-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="669fb-116">Administratörer kan [ändra den här inställningen vilket kan hindra användarna från att skapa en livehändelse](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="669fb-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="669fb-117">Det är viktigt att kontrollera att användarna har behörighet att skapa livehändelser om de får ett principfel.</span><span class="sxs-lookup"><span data-stu-id="669fb-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
