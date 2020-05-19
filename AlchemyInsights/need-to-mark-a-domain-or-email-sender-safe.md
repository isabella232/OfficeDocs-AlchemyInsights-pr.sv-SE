---
title: Behöver du markera en domän eller e-postavsändare säker?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281189"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Behöver du markera en domän eller e-postavsändare säker?

- Användning av **listor över betrodda avsändare rekommenderas inte** eftersom det öppnar organisationen för skräppost-, phish- och förfalskningsattacker.
- Men om det finns ett affärskrav rekommenderar vi **att** du använder **[Mail Flow-regler](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** för detta. Vår vägledning säkerställer att avsändarautentisering (verifierar att skicka domän inte förfalskas). **Vi**rekommenderar inte att du hanterar falska positiva identifieringar med hjälp av säkra avsänningslistor, eftersom undantag från skräppostfiltrering kan öppna din organisation för säkerhetsattacker. Om dina användare får meddelanden som felaktigt markerats som skräppost eller skräppost ska du **[rapportera meddelanden och filer till Microsoft](https://protection.office.com/reportsubmission)**.
- Betrodda avsändare i Outlook, listan Överordnare eller tillåten domänlista i anti-spam-principer **bör undvikas** eftersom avsändare kringgår all skräppost, förfalskning och phish-skydd och avsändandeautentisering (SPF, DKIM, DMARC). Den här metoden används endast bäst för tillfälliga tester.
