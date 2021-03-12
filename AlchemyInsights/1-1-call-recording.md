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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733867"
---
# <a name="11-call-recording"></a><span data-ttu-id="292db-102">Inspelning av 1:1-samtal</span><span class="sxs-lookup"><span data-stu-id="292db-102">1:1 call recording</span></span>

<span data-ttu-id="292db-103">Administratörer måste vidta åtgärder nu för att fortsätta tillåta användare att spela in 1:1-samtal.</span><span class="sxs-lookup"><span data-stu-id="292db-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="292db-104">Från och med den 12 april 2021 börjar vi framtvinga ett nytt samtalsprincipalternativ för Teams *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="292db-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="292db-105">Funktionerna för inspelning av 1:1-samtal kontrolleras av *alternativet AllowCloudRecording* i Teams mötespolicy.</span><span class="sxs-lookup"><span data-stu-id="292db-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="292db-106">Om användarna tillåts spela in Teams-möten kan de även spela in 1:1-samtal.</span><span class="sxs-lookup"><span data-stu-id="292db-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="292db-107">Om du föredrar att blockera alla användare från att spela in 1:1-samtal behöver du inte vidta någon åtgärd.</span><span class="sxs-lookup"><span data-stu-id="292db-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="292db-108">*Policyalternativet AllowCloudRecordingForCalls* är $False alternativ som standard.</span><span class="sxs-lookup"><span data-stu-id="292db-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="292db-109">Den här ändringen beskrivs i följande meddelandecenterinlägg: [(Uppdaterad) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) introduktion till policyn för samtalsinspelning Om du vill ställa in policyalternativet för Teams måste du använda [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="292db-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="292db-110">**Så här aktiverar du samtalsinspelning i 1:1-samtal:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="292db-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="292db-111">**Så här inaktiverar du samtalsinspelning i 1:1-samtal:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="292db-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

