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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702108"
---
# <a name="11-call-recording"></a><span data-ttu-id="feefb-102">Inspelning av 1:1-samtal</span><span class="sxs-lookup"><span data-stu-id="feefb-102">1:1 call recording</span></span>

<span data-ttu-id="feefb-103">Om **knappen Starta** inspelning är nedtonad under ett nödsamtal måste du ändra principinställningarna för den påverkade användaren.</span><span class="sxs-lookup"><span data-stu-id="feefb-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="feefb-104">Kontrollera principinställningen genom att köra Diagnostik för den påverkade användaren genom att skriva **Diag: Teams 1:1-samtalsinspelning** ovan.</span><span class="sxs-lookup"><span data-stu-id="feefb-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="feefb-105">Med början den 31 maj 2021 börjar vi framtvinga en ny Teams *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="feefb-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="feefb-106">Innan den här ändringen kontrolleras inspelning av 1:1-samtal av *AllowCloudRecording* Teams mötespolicyn.</span><span class="sxs-lookup"><span data-stu-id="feefb-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="feefb-107">Den här ändringen har dokumenterats i inlägget i meddelandecentret: [(Uppdaterad) 1:1 Inledningen till inspelningspolicyn för samtal.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)</span><span class="sxs-lookup"><span data-stu-id="feefb-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="feefb-108">*AllowCloudRecordingForCalls*   alternativet för samtalsprincip är **$False** som standard.</span><span class="sxs-lookup"><span data-stu-id="feefb-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="feefb-109">Om du föredrar att blockera alla användare från att spela in 1:1-samtal behöver du inte vidta någon åtgärd.</span><span class="sxs-lookup"><span data-stu-id="feefb-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="feefb-110">Om du vill aktivera samtalsinspelning för alla användare i 1:1-samtal [använder Teams PowerShell](/microsoftteams/teams-powershell-install) för att köra följande cmdlet:</span><span class="sxs-lookup"><span data-stu-id="feefb-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="feefb-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="feefb-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="feefb-112">Du kan också skapa en ny princip och ange **-AllowCloudRecordingForCalls** **$true** tilldela den principen till användarna.</span><span class="sxs-lookup"><span data-stu-id="feefb-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="feefb-113">Mer information finns i [principkontroller för samtalsinspelning är (nästan!) Här](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="feefb-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
