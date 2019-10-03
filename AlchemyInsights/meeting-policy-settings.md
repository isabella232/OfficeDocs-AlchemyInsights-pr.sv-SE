---
title: Principinställningar för möten
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376856"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="9367d-102">Hantera Mötes principer i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9367d-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="9367d-103">Mötes principer används för att styra de funktioner som är tillgängliga för mötesdeltagare för möten som schemaläggs av användare i din organisation.</span><span class="sxs-lookup"><span data-stu-id="9367d-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="9367d-104">Vissa funktioner i Mötes principer kanske inte implementeras i Teams administratörscenter ännu (dessa är märkta "kommer snart" i dokumentationen).</span><span class="sxs-lookup"><span data-stu-id="9367d-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="9367d-105">I det här fallet, eller om du får ett felmeddelande som "vi kan inte uppdatera principen just nu men försök igen senare" i Microsoft Teams administratörscenter, rekommenderar vi att du använder PowerShell för att skapa eller ändra Teams Mötes principer.</span><span class="sxs-lookup"><span data-stu-id="9367d-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="9367d-106">Mer information om Mötes principer finns i följande resurser:</span><span class="sxs-lookup"><span data-stu-id="9367d-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="9367d-107">Mer information om hur du skapar principer, gör ändringar och tilldelar användare till principen finns [i hantera Mötes principer i Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="9367d-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="9367d-108">Om du vill göra principändringar med hjälp av PowerShell-cmdlets, se [Teams PowerShell-översikt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="9367d-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="9367d-109">Du måste använda [Skype för Business PowerShell-modulen](https://www.microsoft.com/download/details.aspx?id=39366) för team Mötes principer.</span><span class="sxs-lookup"><span data-stu-id="9367d-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="9367d-110">Granska [dokumentationen för \*-csteamsmeetingpolicy cmdlets](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) för mer information.</span><span class="sxs-lookup"><span data-stu-id="9367d-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="9367d-111">**Anmärkning:** Det kan ta upp till 24 timmar innan principändringarna träder i kraft för användarna.</span><span class="sxs-lookup"><span data-stu-id="9367d-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="9367d-112">Du kanske inte kan göra ändringar i nyligen skapade principer omedelbart. vänta 4 timmar och försök att ändra en nyskapad princip igen.</span><span class="sxs-lookup"><span data-stu-id="9367d-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="9367d-113">Om du fortfarande har problem kan du prova PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9367d-113">If you're still having problems, try PowerShell.</span></span>  