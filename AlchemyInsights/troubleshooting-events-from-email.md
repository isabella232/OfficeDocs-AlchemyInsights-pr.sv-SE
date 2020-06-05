---
title: Felsöka händelser från e-post
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569402"
---
# <a name="troubleshooting-events-from-email"></a>Felsöka händelser från e-post

1. Kontrollera att funktionen är aktiverad för postlådan: **Get-EventsFromEmailConfiguration -Identity <mailbox> **

2. Titta sedan på loggarna "Händelser från e-post" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Leta reda på det InternetMessageId som matchar objektet i postlådan i loggarna "Händelser från e-post".  

4. TrustScore avgör om objektet läggs till eller inte. Händelser läggs bara till om TrustScore = "Trusted".

TrustScore bestäms av SPF-, Dkim- eller Dmarc-egenskaper, som finns i meddelandehuvudet.

Så här visar du dessa egenskaper:

**Outlook på skrivbordet**

- Öppna objektet
- Fil -> egenskaper -> Internet-huvuden

eller

**MFCMapi (på andra sätt)**

- Navigera till objektet i inkorgen
- Leta efter PR_TRANSPORT_MESSAGE_HEADERS_W

Dessa egenskaper bestäms och registreras under transport och routning. För ytterligare felsökning kan du behöva följa upp med Transport Support om felen i SPF, DKIM and.or DMARC.