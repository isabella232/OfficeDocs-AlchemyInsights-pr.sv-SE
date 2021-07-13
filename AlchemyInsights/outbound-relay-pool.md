---
title: Utgående reläpool
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381864"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="40888-102">Utgående reläpool</span><span class="sxs-lookup"><span data-stu-id="40888-102">Outbound relay pool</span></span>

<span data-ttu-id="40888-103">Microsoft gör några ändringar i konfigurationen för att vidarebefordra eller vidarebefordra e-post Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="40888-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="40888-104">Meddelanden i vissa fall vidarebefordras eller vidarebefordras via Microsoft 365 med en särskild reläpool.</span><span class="sxs-lookup"><span data-stu-id="40888-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="40888-105">Meddelanden som skickas med reläpoolen kan hamna i mottagarens skräppostmapp.</span><span class="sxs-lookup"><span data-stu-id="40888-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="40888-106">Mer information finns i [Pooler för utgående leverans](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="40888-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="40888-107">För att undvika ett scenario med hjälp av reläpoolen ska du kontrollera att vidarebefordrade/vidarebefordrade meddelanden uppfyller något av följande kriterier:</span><span class="sxs-lookup"><span data-stu-id="40888-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="40888-108">Den utgående avsändaren är en godkänd domän för klientorganisationen.</span><span class="sxs-lookup"><span data-stu-id="40888-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="40888-109">SPF (Sender Policy Framework) klarar sig när meddelandet kommer till Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="40888-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="40888-110">DKIM (DomainKeys Identified Mail) på P2-avsändardomänen passeras när meddelandet kommer till Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="40888-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="40888-111">Meddelanden som uppfyller ovanstående villkor vidarebefordras inte via reläpoolen.</span><span class="sxs-lookup"><span data-stu-id="40888-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="40888-112">Om MX-posten för din domän pekas till en tredje part eller en lokal server ska du använda förbättrad filtrering för att kontrollera att SPF-verifieringen är rätt för inkommande e-post och för att undvika att skicka e-post via reläpoolen.</span><span class="sxs-lookup"><span data-stu-id="40888-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="40888-113">**Hur vet vi om vi påverkas av reläpoolen?**</span><span class="sxs-lookup"><span data-stu-id="40888-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="40888-114">Om dina vidarebefordrade eller vidarebefordrade e-postmeddelanden använder något av villkoren ovan vidarebefordras inte meddelanden via reläpoolen.</span><span class="sxs-lookup"><span data-stu-id="40888-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="40888-115">Men om ett meddelande skickas via en reläpool finns den utgående server-IP i intervallet 40.95.0.0/16 och det utgående servernamnet innehåller **rly** i namnet.</span><span class="sxs-lookup"><span data-stu-id="40888-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

