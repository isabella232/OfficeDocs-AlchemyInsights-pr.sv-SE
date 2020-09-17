---
title: Inställningar för Mötes princip
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794352"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="33bbe-102">Hantera Mötes principer i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="33bbe-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="33bbe-103">**Obs! det kan ta upp till 24 timmar innan princip ändringarna börjar gälla för användarna.**</span><span class="sxs-lookup"><span data-stu-id="33bbe-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="33bbe-104">Du kanske inte kan göra ändringar i nyskapade principer omedelbart; vänta 4 timmar och försök sedan att ändra en nyligen skapad princip igen.</span><span class="sxs-lookup"><span data-stu-id="33bbe-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="33bbe-105">Mötes principer används för att kontrol lera vilka funktioner som är tillgängliga för Mötes deltagare för möten som har schemalagts av användare i organisationen.</span><span class="sxs-lookup"><span data-stu-id="33bbe-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="33bbe-106">Vissa funktioner för Mötes principer kanske inte implementeras i team administrations centret ännu (de här är märkta "kommer snart" i dokumentationen).</span><span class="sxs-lookup"><span data-stu-id="33bbe-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="33bbe-107">I det här fallet, eller om du får ett fel meddelande som "vi kan inte uppdatera policyn just nu, men prova igen senare" i administrations centret för Microsoft Teams rekommenderar vi att du använder PowerShell för att skapa eller ändra principer för team möten.</span><span class="sxs-lookup"><span data-stu-id="33bbe-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="33bbe-108">Mer information om Mötes principer finns i följande resurser:</span><span class="sxs-lookup"><span data-stu-id="33bbe-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="33bbe-109">Information om hur du skapar principer, gör ändringar och tilldelar användare till principer finns i [Hantera Mötes principer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="33bbe-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="33bbe-110">Information om hur du ändrar princip ändringar med PowerShell-cmdletar finns i [Översikt över Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="33bbe-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="33bbe-111">Du måste använda PowerShell- [modulen i Skype för företag](https://www.microsoft.com/download/details.aspx?id=39366) för att få arbets grupper.</span><span class="sxs-lookup"><span data-stu-id="33bbe-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="33bbe-112">Läs [dokumentationen för \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) för mer information.</span><span class="sxs-lookup"><span data-stu-id="33bbe-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

