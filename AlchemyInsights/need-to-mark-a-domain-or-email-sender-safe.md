---
title: Behöver du markera en domän eller e-post avsändare?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803263"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Behöver du markera en domän eller e-post avsändare?

- Användning av **listor för säkra avsändare rekommenderas inte** eftersom den öppnar din organisation för skräp post, Phish och förfalskningar.
- Om det finns ett företags behov **rekommenderar** vi att du använder **[regler för e-postflöde](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** för detta. Vår vägledning säkerställer att avsändaren (verifierar att sändande domän inte är falsk). **Obs!** vi rekommenderar inte att du hanterar falsk identifiering genom att använda listor med säkra avsändare, eftersom undantag för skräp post filtrering kan öppna din organisation för säkerhets attacker. Om dina användare (er) får meddelanden som är felaktigt markerade som skräp post, kan du **[rapportera meddelanden och filer till Microsoft](https://protection.office.com/reportsubmission)**.
- Betrodda avsändare i Outlook, listan med tillåtna avsändare eller tillåtna domäner i principer för skräp post skydd **bör undvikas** eftersom avsändare kringgår all skräp post, falsk identitet och phishskydd (SPF, DKIM, DMARC). Den här metoden är bäst för tillfälliga tester.
