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
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319966"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Behöver du markera en domän eller e-postavsändare som betrodd?

- Du bör **inte använda listor över betrodda** avsändare eftersom det öppnar din organisation för attacker av skräppost, phish och förfalskning.
- Om det finns affärskrav rekommenderar vi emellertid att du **använder** **[e-Flow för](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** detta. Våra riktlinjer säkerställer att avsändarautentisering (verifierar att avsändarens domän inte kapas). 
    **Obs!** Vi rekommenderar inte att du hanterar falska positiva meddelanden med hjälp av listor över betrodda avsändare, eftersom undantag för skräppostfiltrering kan öppna organisationen för säkerhetsattacker. Om användarna får meddelanden som felaktigt har markerats som skräppost ska du **[rapportera meddelanden och filer till Microsoft.](https://protection.office.com/reportsubmission)**
- Valv Avsändare i Outlook, lista över tillåtna avsändare eller lista över  tillåtna domäner i skydd mot skräppost bör undvikas eftersom avsändare kringgår all skräppost, förfalskning, spoishskydd och avsändarautentisering (SPF, DKIM, DMARC). Den här metoden används endast för temporär testning.
- Validering av att ett visst **[e-postmeddelande](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)** kringgår utvärdering av skräppostskydd kan göras genom att markera meddelanderubriken "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN), se Rubriker för skräppostmeddelanden .
- Eftersom Microsoft vill att våra kunder ska vara [säkra som standard](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)tillämpas inte vissa åsidosättningar i klientorganisationen för skadlig programvara och nätfiske med hög säkerhet. Dessa åsidosättningar omfattar: o Listor över tillåtna avsändare eller tillåtna domäner (principer mot skräppost) o Outlook Valv Senders o IP Allow List (anslutningsfiltrering) 
- Den enda åsidosättningen som tillåter nätfiskemeddelande med hög säkerhet att kringgå filtrering är Exchange-postflödesregler (kallas även transportregler). Information om hur du använder e-postflödesregler för att kringgå filtrering finns i Använda e-postflödesregler för att ange **[SCL (Spam Confidence Level) i meddelanden.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**