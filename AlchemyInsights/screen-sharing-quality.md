---
title: Skärmdelningskvalitet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11061"
- "11062"
- "9002254"
- "9002536"
ms.openlocfilehash: 0832f886d3f5c0bfbfe138647403e4e215deaacb
ms.sourcegitcommit: d822377ec76adf9ef6d13bc761a16c9900a3e7cb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/26/2021
ms.locfileid: "52125447"
---
# <a name="screen-sharing-quality"></a><span data-ttu-id="18f46-102">Skärmdelningskvalitet</span><span class="sxs-lookup"><span data-stu-id="18f46-102">Screen sharing quality</span></span>

<span data-ttu-id="18f46-103">I de flesta fall kommer kvalitetsproblem med skärmdelning till begränsad bandbredd från klientsidan.</span><span class="sxs-lookup"><span data-stu-id="18f46-103">In most cases quality issues with Screen Sharing comes down to limited bandwidth from the client side.</span></span>  <span data-ttu-id="18f46-104">I de fall där bandbredden inte är begränsad optimerar Teams mediakvalitet, inklusive upp till 1080p-videoupplösning, upp till 30fps för video och 15fps för innehåll samt ljud med hög återgivning.</span><span class="sxs-lookup"><span data-stu-id="18f46-104">Where bandwidth isn't limited, Teams optimizes media quality, including up to 1080p video resolution, up to 30fps for video and 15fps for content, and high-fidelity audio.</span></span>

<span data-ttu-id="18f46-105">Teams alltid på bandbreddsanvändning och kan ge HD-videokvalitet på under 1,2 Mbit/s.</span><span class="sxs-lookup"><span data-stu-id="18f46-105">Teams is always conservative on bandwidth utilization and can deliver HD video quality in under 1.2Mbps.</span></span> <span data-ttu-id="18f46-106">Den faktiska bandbreddsförbrukningen i varje ljud-/videosamtal eller möte varierar beroende på faktorer som videolayout, videoupplösning och videorutor per sekund.</span><span class="sxs-lookup"><span data-stu-id="18f46-106">The actual bandwidth consumption in each audio/video call or meeting vary based on factors such as video layout, video resolution, and video frames per second.</span></span> <span data-ttu-id="18f46-107">När det finns mer bandbredd ökar kvaliteten och användningen för att ge den bästa upplevelsen.</span><span class="sxs-lookup"><span data-stu-id="18f46-107">When more bandwidth is available, quality and usage increase to deliver the best experience.</span></span> <span data-ttu-id="18f46-108">I den här tabellen beskrivs hur Teams använder bandbredd:</span><span class="sxs-lookup"><span data-stu-id="18f46-108">This table describes how Teams uses bandwidth:</span></span>

<span data-ttu-id="18f46-109">**Scenarier med bandbredd(upp/ned)**</span><span class="sxs-lookup"><span data-stu-id="18f46-109">**Bandwidth(up/down) Scenarios**</span></span>

- <span data-ttu-id="18f46-110">30 kbit/s Peer-to-peer-ljudsamtal</span><span class="sxs-lookup"><span data-stu-id="18f46-110">30 kbps Peer-to-peer audio calling</span></span>

- <span data-ttu-id="18f46-111">130 kbit/s Peer-to-peer-ljudsamtal och skärmdelning</span><span class="sxs-lookup"><span data-stu-id="18f46-111">130 kbps Peer-to-peer audio calling and screen sharing</span></span>

- <span data-ttu-id="18f46-112">500 kbit/s Videosamtal med peer-to-peer-kvalitet 360p på 30fps</span><span class="sxs-lookup"><span data-stu-id="18f46-112">500 kbps Peer-to-peer quality video calling 360p at 30fps</span></span>

- <span data-ttu-id="18f46-113">Videosamtal i HD-kvalitet med 1,2 Mbit/s i peer-to-peer-kvalitet med HD 720p vid 30fps</span><span class="sxs-lookup"><span data-stu-id="18f46-113">1.2 Mbps Peer-to-peer HD quality video calling with resolution of HD 720p at 30fps</span></span>

- <span data-ttu-id="18f46-114">Videosamtal i HD-kvalitet med 1,5 Mbit/s i peer-to-peer-kvalitet med HD 1080p vid 30fps</span><span class="sxs-lookup"><span data-stu-id="18f46-114">1.5 Mbps Peer-to-peer HD quality video calling with resolution of HD 1080p at 30fps</span></span>

- <span data-ttu-id="18f46-115">500 kbit/s/1 Mbit/s Gruppvideosamtal</span><span class="sxs-lookup"><span data-stu-id="18f46-115">500kbps/1Mbps Group Video calling</span></span>

- <span data-ttu-id="18f46-116">1 Mbit/s/ 2 Mbit/s HD Grupp-videosamtal (540p-videor på 1080p-skärm)</span><span class="sxs-lookup"><span data-stu-id="18f46-116">1Mbps/2Mbps HD Group video calling (540p videos on 1080p screen)</span></span>

<span data-ttu-id="18f46-117">Mer information finns i [Förbereda organisationens nätverk för Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span><span class="sxs-lookup"><span data-stu-id="18f46-117">For more information, see [Prepare your organization's network for Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span></span>