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
ms.openlocfilehash: 8750c9036f258d9c5edc94bb027d564140bbd9914712cc1f25ff3abc3f4b9468
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54041604"
---
# <a name="outbound-relay-pool"></a>Utgående reläpool

Microsoft gör några ändringar i konfigurationen för att vidarebefordra eller vidarebefordra e-post Microsoft 365. Meddelanden i vissa fall vidarebefordras eller vidarebefordras via Microsoft 365 med en särskild reläpool. Meddelanden som skickas med reläpoolen kan hamna i mottagarens skräppostmapp. Mer information finns i [Pooler för utgående leverans](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

För att undvika ett scenario med hjälp av reläpoolen ska du kontrollera att vidarebefordrade/vidarebefordrade meddelanden uppfyller något av följande kriterier:

- Den utgående avsändaren är en godkänd domän för klientorganisationen.
- SPF (Sender Policy Framework) klarar sig när meddelandet kommer till Microsoft 365.
- DKIM (DomainKeys Identified Mail) på P2-avsändardomänen passeras när meddelandet kommer till Microsoft 365.
 
Meddelanden som uppfyller ovanstående villkor vidarebefordras inte via reläpoolen.

Om MX-posten för din domän pekas till en tredje part eller en lokal server ska du använda förbättrad filtrering för att kontrollera att SPF-verifieringen är rätt för inkommande e-post och för att undvika att skicka e-post via reläpoolen.

**Hur vet vi om vi påverkas av reläpoolen?**

Om dina vidarebefordrade eller vidarebefordrade e-postmeddelanden använder något av villkoren ovan vidarebefordras inte meddelanden via reläpoolen. Men om ett meddelande skickas via en reläpool finns den utgående server-IP i intervallet 40.95.0.0/16 och det utgående servernamnet innehåller **rly** i namnet.

