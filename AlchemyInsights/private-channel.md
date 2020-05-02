---
title: Privat kanal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005456"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="7e642-102">Privata kanaler i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7e642-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="7e642-103">Privata kanaler är en ny funktion i Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7e642-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="7e642-104">Observera att privata kanaler inte kan konverteras från standardkanaler eller vice versa.</span><span class="sxs-lookup"><span data-stu-id="7e642-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="7e642-105">Mer information om privata kanaler, till exempel information om [skapande och medlemskap](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) för privata kanaler och [sharepoint-webbplatser för privata kanaler,](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)finns [i Privata kanaler i Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="7e642-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="7e642-106">**Anm.:** Eftersom konfiguration för bevarande av privata kanalmeddelanden ännu inte stöds, har klienter med bevarandeprinciper aktiverade inte privata kanaler aktiverade som standard.</span><span class="sxs-lookup"><span data-stu-id="7e642-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="7e642-107">Privata kanaler kan aktiveras i administrationscentret för Teams.</span><span class="sxs-lookup"><span data-stu-id="7e642-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="7e642-108">Observera också att även om lagring av privata kanalmeddelanden inte stöds, stöds lagring av filer som delas i privata kanaler.</span><span class="sxs-lookup"><span data-stu-id="7e642-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="7e642-109">**Behöver du en ny teamägare?**</span><span class="sxs-lookup"><span data-stu-id="7e642-109">**Need a new team owner?**</span></span>

<span data-ttu-id="7e642-110">Om din privata kanalägare lämnar kan du lägga till en ny gruppägare via Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="7e642-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="7e642-111">Gå [hit](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) för att installera Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="7e642-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="7e642-112">Här är cmdlet du behöver:</span><span class="sxs-lookup"><span data-stu-id="7e642-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="7e642-113">Mer information om Teams Powershell finns i [Teams PowerShell Översikt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="7e642-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
