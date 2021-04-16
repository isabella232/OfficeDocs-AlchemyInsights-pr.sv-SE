---
title: Behöver du markera en domän eller e-postavsändare som betrodd?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792150"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Behöver du markera en domän eller e-postavsändare som betrodd?

- Du bör **inte använda listor över betrodda** avsändare eftersom det öppnar organisationen för attacker av skräppost, phish och förfalskning.
- Om det finns affärskrav rekommenderar vi emellertid att du **använder** **[e-postflödesregler för](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** detta. Våra riktlinjer säkerställer att avsändarautentisering (verifierar att avsändarens domän inte kapas). **Obs!** Vi rekommenderar inte att du hanterar falska positiva meddelanden med hjälp av listor över betrodda avsändare, eftersom undantag för skräppostfiltrering kan öppna organisationen för säkerhetsattacker. Om användarna får meddelanden som felaktigt har markerats som skräppost ska du **[rapportera meddelanden och filer till Microsoft.](https://protection.office.com/reportsubmission)**
- Betrodda avsändare i Outlook, lista över tillåtna avsändare  eller lista över tillåtna domäner i skydd mot skräppost bör undvikas eftersom avsändare kringgår all skräppost, förfalskningsskydd och säkerhets- och avsändarautentisering (SPF, DKIM, DMARC). Den här metoden används endast för temporär testning.
