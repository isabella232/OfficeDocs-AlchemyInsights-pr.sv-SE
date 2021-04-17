---
title: Inställningar för mötesprincip
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825461"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="4ae16-102">Hantera mötesprinciper i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="4ae16-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="4ae16-103">**Obs! Det kan ta upp till 24 timmar innan principändringarna verkställs för användarna.**</span><span class="sxs-lookup"><span data-stu-id="4ae16-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="4ae16-104">Du kanske inte kan ändra nyligen skapade principer direkt. vänta 4 timmar och försök sedan ändra en princip som nyligen skapats igen.</span><span class="sxs-lookup"><span data-stu-id="4ae16-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="4ae16-105">Mötesprinciper används för att styra vilka funktioner som är tillgängliga för mötesdeltagare för möten som schemaläggs av användare i organisationen.</span><span class="sxs-lookup"><span data-stu-id="4ae16-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="4ae16-106">Vissa funktioner i mötes principer kanske inte implementeras i administrationscentret för Teams ännu (dessa heter "kommer snart" i dokumentationen).</span><span class="sxs-lookup"><span data-stu-id="4ae16-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="4ae16-107">I det här fallet, eller om du får ett felmeddelande som "Vi kan inte uppdatera policyn just nu men försök igen senare" i administrationscentret för Microsoft Teams, rekommenderar vi att du använder PowerShell för att skapa eller ändra mötesprinciper för Teams.</span><span class="sxs-lookup"><span data-stu-id="4ae16-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="4ae16-108">Mer information om mötesprinciper finns i följande resurser:</span><span class="sxs-lookup"><span data-stu-id="4ae16-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="4ae16-109">Mer information om hur du skapar principer, ändrar och tilldelar användare till principen finns i [Hantera mötesprinciper i Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="4ae16-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="4ae16-110">Information om hur du gör principändringar med PowerShell-cmdlets finns [i Översikt över Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="4ae16-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="4ae16-111">Du måste använda Skype för [företag PowerShell-modulen för](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) Teams-mötesprinciper.</span><span class="sxs-lookup"><span data-stu-id="4ae16-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="4ae16-112">Mer information [finns i dokumentationen för \*-CsTeamsMeetingPolicy-cmdlets.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="4ae16-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

