---
title: Felsökning av händelser från e-post
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834857"
---
# <a name="troubleshooting-events-from-email"></a>Felsökning av händelser från e-post

1. Kontrollera att funktionen är aktiverad för postlådan: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Titta sedan i loggarna "Händelser från **e-post" Exportera-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. I loggarna för händelser från e-post hittar du InternetMessageId som matchar objektet i postlådan.  

4. TrustScore avgör om objektet läggs till eller inte. Händelser läggs bara till om TrustScore = "Trusted".

TrustScore bestäms av egenskaperna SPF, Dkim eller Dmarc, som finns i meddelandehuvudet.

Så här visar du de här egenskaperna:

**Skrivbordsversionen av Outlook**

- Öppna objektet
- Arkiv -> Egenskaper -> internethuvuden

eller

**MFCMapi**

- Navigera till objektet i Inkorgen
- Leta efter PR_TRANSPORT_MESSAGE_HEADERS_W

Dessa egenskaper bestäms och registreras under transport och routning. För ytterligare felsökning kan du behöva följa upp med TransportSupport om felen i SPF, DKIM och.or DMARC.