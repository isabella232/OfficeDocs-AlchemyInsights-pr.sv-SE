---
title: Inspelning av 1:1-samtal
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696976"
---
# <a name="11-call-recording"></a><span data-ttu-id="d8730-102">Inspelning av 1:1-samtal</span><span class="sxs-lookup"><span data-stu-id="d8730-102">1:1 call recording</span></span>

<span data-ttu-id="d8730-103">Om **knappen Starta** inspelning är nedtonad under ett nödsamtal måste du ändra principinställningarna för den påverkade användaren.</span><span class="sxs-lookup"><span data-stu-id="d8730-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="d8730-104">Med början den 31 maj 2021 börjar vi framtvinga en ny Teams *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="d8730-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="d8730-105">Innan den här ändringen kontrolleras inspelning av 1:1-samtal av *AllowCloudRecording* Teams mötespolicyn.</span><span class="sxs-lookup"><span data-stu-id="d8730-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="d8730-106">Den här ändringen har dokumenterats i inlägget i meddelandecentret: [(Uppdaterad) 1:1 Inledningen till inspelningspolicyn för samtal.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)</span><span class="sxs-lookup"><span data-stu-id="d8730-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="d8730-107">*AllowCloudRecordingForCalls*   alternativet för samtalsprincip är **$False** som standard.</span><span class="sxs-lookup"><span data-stu-id="d8730-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="d8730-108">Om du föredrar att blockera alla användare från att spela in 1:1-samtal behöver du inte vidta någon åtgärd.</span><span class="sxs-lookup"><span data-stu-id="d8730-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="d8730-109">Om du vill aktivera samtalsinspelning för alla användare i 1:1-samtal använder Teams PowerShell för att köra följande cmdlet:</span><span class="sxs-lookup"><span data-stu-id="d8730-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="d8730-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="d8730-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="d8730-111">Du kan också skapa en ny princip och ange **-AllowCloudRecordingForCalls** **$true** tilldela den principen till användarna.</span><span class="sxs-lookup"><span data-stu-id="d8730-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="d8730-112">Mer information finns i [principkontroller för samtalsinspelning är (nästan!) Här](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="d8730-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
