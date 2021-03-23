---
title: Blockera användare från att spela in möten
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037067"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="f71b6-102">Blockera användare från att spela in möten</span><span class="sxs-lookup"><span data-stu-id="f71b6-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="f71b6-103">Om du behöver förhindra **eller blockera specifika användare** från att spela in Teams-möten kan du göra det via inställningar för Teams mötespolicy.</span><span class="sxs-lookup"><span data-stu-id="f71b6-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="f71b6-104">I administrationscentret för Microsoft Teams inaktiverar du inställningen **Tillåt molninspelning** i den mötesprincip som tilldelats den användaren.</span><span class="sxs-lookup"><span data-stu-id="f71b6-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="f71b6-105">Mer information finns i [Hantera mötesprinciper i Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="f71b6-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="f71b6-106">Använd supportdiagnostik för att verifiera om en viss användare tillåts eller inte kan spela in Teams-möten.</span><span class="sxs-lookup"><span data-stu-id="f71b6-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="f71b6-107">Kör en ny supportfråga och skriv i **Diag: Mötesinspelning** – diagnostiken kontrollerar principinställningarna för den angivna användaren och bestämmer principinställningarna.</span><span class="sxs-lookup"><span data-stu-id="f71b6-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="f71b6-108">Tänk på att det kan ta några timmar innan de nya principinställningarna börjar gälla, så om du precis har gjort en ändring bör du vänta några timmar innan du kör diagnostiken igen.</span><span class="sxs-lookup"><span data-stu-id="f71b6-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="f71b6-109">Mer information finns i [Aktivera eller inaktivera molninspelning.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="f71b6-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
