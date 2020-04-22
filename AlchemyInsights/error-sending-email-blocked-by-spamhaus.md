---
title: Fel att skicka e-post blockeras av SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714276"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fel att skicka e-post: Klientvärden blockerad med Spamhaus

IP-adressen som skickade meddelandet finns på en blockeringslista som ägs av [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Orsaker till att blockeras av Spamhaus är komprometterade konton, komprometterade datorer som delar en offentlig IP-adress och Internet Service Provider-principer (ISP). Möjliga korrigeringar är:
  
- För blockerade inkommande meddelanden där du styr källmeddelandeservern måste du fastställa orsaken och ta bort blocket från Spamhaus webbplats.

- För blockerade inkommande meddelanden där källans IP-adress tillhör någon annan måste adressägaren ta bort blocket från Spamhaus-webbplatsen. Om IP-adressen finns i PBL (Policy Block List) kan ägaren tilldela en annan statisk IP-adress eller ta bort adressen från PBL.

- För blockerade utgående meddelanden från din domän som är ansluten till Microsoft kan du få det här felet om meddelandena dirigeras via en tjänst från tredje part. Du kan använda ett WHOIS-uppslagsverktyg för att hitta ägaren till den blockerade IP-adressen.
