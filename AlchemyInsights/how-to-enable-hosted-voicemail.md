---
title: Så här aktiverar du röst brev låda
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679164"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="beeb6-102">Så här aktiverar du röst brev låda</span><span class="sxs-lookup"><span data-stu-id="beeb6-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="beeb6-103">För att aktivera röst brev låda måste **HostedVoicemail** vara inställt på $True.</span><span class="sxs-lookup"><span data-stu-id="beeb6-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="beeb6-104">Egenskapen **HostedVoicemail** för användaren med Remote POWERSHELL (RPS).</span><span class="sxs-lookup"><span data-stu-id="beeb6-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="beeb6-105">Mer information om hur du ansluter till RPS finns i [Microsoft Teams PowerShell-översikten](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) för att få mer information om hur du ansluter till RPS.</span><span class="sxs-lookup"><span data-stu-id="beeb6-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="beeb6-106">Teams-administratören bör vara inloggad i fjärr-PowerShell för Teams.</span><span class="sxs-lookup"><span data-stu-id="beeb6-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="beeb6-107">Från PowerShell uppmana team administratören att köra **set-csuser user@contoso.com-HostedVoiceMail $True** där SIP URI är av en användare.</span><span class="sxs-lookup"><span data-stu-id="beeb6-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="beeb6-108">Ändringar i policyn kan ta upp till 24 timmar att replikera.</span><span class="sxs-lookup"><span data-stu-id="beeb6-108">Changes to policies can take up to 24 hours to replicate.</span></span>