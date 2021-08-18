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
ms.openlocfilehash: 7e5bb1fda1dec0c0f72d1944d54b6f2747a6e909
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326095"
---
# <a name="outbound-relay-pool"></a>Utgående reläpool

Microsoft gör några ändringar i konfigurationen för att vidarebefordra eller vidarebefordra e-post Microsoft 365. Meddelanden i vissa fall vidarebefordras eller vidarebefordras via e Microsoft 365 med en särskild reläpool. Meddelanden som skickas med reläpoolen kan hamna i mottagarens skräppostmapp. Mer information finns i [Pooler för utgående leverans](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

För att undvika ett scenario med hjälp av reläpoolen ska du kontrollera att vidarebefordrade/vidarebefordrade meddelanden uppfyller något av följande kriterier:

- Den utgående avsändaren är en godkänd domän för klientorganisationen.
- SPF (Sender Policy Framework) passeras när meddelandet kommer till Microsoft 365.
- DKIM (DomainKeys Identified Mail) på P2-avsändardomänen passeras när meddelandet kommer Microsoft 365.
 
Meddelanden som uppfyller ovanstående villkor vidarebefordras inte via reläpoolen.

Om MX-posten för din domän pekade på en tredje part eller en lokal server använder du förbättrad filtrering för att kontrollera att SPF-verifieringen är rätt för inkommande e-post och för att undvika att skicka e-post via reläpoolen.

**Hur vet vi om vi påverkas av reläpoolen?**

Om dina vidarebefordrade eller vidarebefordrade e-postmeddelanden använder något av villkoren ovan vidarebefordras inte meddelanden via reläpoolen. Men om ett meddelande skickas via en reläpool finns den utgående server-IP i intervallet 40.95.0.0/16 och det utgående servernamnet innehåller **rly** i namnet.

