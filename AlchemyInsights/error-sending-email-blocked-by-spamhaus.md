---
title: Skicka e-postmeddelanden blockeras av SpamHaus fel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 52a5c20d59a2eac4c4bf465edaa888952d47f39f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387867"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fel vid överföring av e-post: Klientvärd blockeras med hjälp av Spamhaus

IP-adressen som meddelandet är på en Blockeringslista som ägs av [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Skälen för att blockeras av Spamhaus inkludera avslöjade konton äventyras av datorer som delar en gemensam IP-adress och principer för Internet-leverantör (ISP). Det är möjligt korrigeringar:
  
- För blockerade inkommande meddelanden till Office 365 där du kan bestämma källservern för e-post, måste du ta reda på orsaken och ta bort spärren från webbplatsen Spamhaus.

- Blockerade inkommande meddelanden till Office 365 där källans IP-adress hör till någon annan måste adress ägare ta bort spärren från webbplatsen Spamhaus. Om IP-adressen är i princip Block lista (PBL), ägaren tilldela en annan statisk IP-adress eller ta bort adressen från PBL.

- Du kan få felet om meddelanden dirigeras via en 3: e part tjänst för blockerade utgående meddelanden från din domän i Office 365. Du kan använda verktyget en WHOIS-sökning för att hitta den blockerade IP-adress ägaren.
