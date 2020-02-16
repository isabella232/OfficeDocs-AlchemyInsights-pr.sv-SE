---
title: Inställningar för mötesprincip
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042862"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="ac774-102">Hantera mötesprinciper i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ac774-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="ac774-103">**Det kan ta upp till 24 timmar innan principändringar träder i kraft för användarna.**</span><span class="sxs-lookup"><span data-stu-id="ac774-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="ac774-104">Du kanske inte kan göra ändringar i nyskapade principer omedelbart. vänta 4 timmar och försöka ändra en nyskapad princip igen.</span><span class="sxs-lookup"><span data-stu-id="ac774-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="ac774-105">Mötesprinciper används för att styra de funktioner som är tillgängliga för mötesdeltagare för möten som schemaläggs av användare i organisationen.</span><span class="sxs-lookup"><span data-stu-id="ac774-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="ac774-106">Vissa funktioner i mötesprinciper kanske inte implementeras i administrationscentret teams ännu (dessa är märkta "kommer snart" i dokumentationen).</span><span class="sxs-lookup"><span data-stu-id="ac774-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="ac774-107">I det här fallet, eller om du får ett felmeddelande som "Vi kan inte uppdatera principen just nu men prova den igen senare" i administrationscentret för Microsoft Teams rekommenderar vi att du använder PowerShell för att skapa eller ändra teams mötesprinciper.</span><span class="sxs-lookup"><span data-stu-id="ac774-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="ac774-108">Mer information om mötesprinciper finns i följande resurser:</span><span class="sxs-lookup"><span data-stu-id="ac774-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="ac774-109">Mer information om hur du skapar principer, gör ändringar och tilldela användare till principen finns i [Hantera mötesprinciper i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="ac774-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="ac774-110">Mer göra principändringar med PowerShell-cmdlets finns i [Team PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="ac774-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="ac774-111">Du måste använda [Skype för företag PowerShell-modulen](https://www.microsoft.com/download/details.aspx?id=39366) för teams mötesprinciper.</span><span class="sxs-lookup"><span data-stu-id="ac774-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="ac774-112">Läs [dokumentationen \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) för mer information.</span><span class="sxs-lookup"><span data-stu-id="ac774-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

