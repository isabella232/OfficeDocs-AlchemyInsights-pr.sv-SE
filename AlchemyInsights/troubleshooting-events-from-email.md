---
title: Felsöka händelser från e-post
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
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658752"
---
# <a name="troubleshooting-events-from-email"></a>Felsöka händelser från e-post

1. Kontrol lera att funktionen är aktive rad för post lådan: **get- <mailbox> EventsFromEmailConfiguration-Identity**

2. Titta sedan på "händelserna from E-mail"-loggarna **export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Leta reda på InternetMessageId som matchar objektet i post lådan i loggarna händelser från e-post.  

4. TrustScore bestämmer om objektet läggs till eller inte. Händelser läggs endast till om TrustScore = "betrodd".

TrustScore bestäms av SPF-, DKIM-eller DMARC-egenskaper, som finns i meddelande huvudet.

Så här visar du dessa egenskaper:

**Outlook på Skriv bordet**

- Öppna objektet
- Egenskaper för fil >-> Internet rubriker

eller

**MFCMapi**

- Navigera till objektet i Inkorgen
- Leta efter PR_TRANSPORT_MESSAGE_HEADERS_W

Dessa egenskaper bestäms och spelas in under transport och routning. För ytterligare fel sökning kan du behöva följa upp transport stöd om felet i SPF-, DKIM-och. DMARC.