---
title: Fel när e-post skulle skickas blockerad av SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813742"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fel när e-post skickas: Klientvärden blockeras med Spamhaus

IP-adressen som har skickat meddelandet finns på en blockeringslista som ägs av [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245) Orsaker till att blockeras av Spamhaus är till exempel komprometterade konton, komprometterade datorer som delar en offentlig IP-adress och Internetleverantörens principer. Möjliga korrigeringar är:
  
- För blockerade inkommande meddelanden där du styr käll-e-postservern måste du fastställa orsaken och ta bort blockeringen på Spamhaus-webbplatsen.

- För blockerade inkommande meddelanden där käll-IP-adressen tillhör någon annan måste adressägaren ta bort blockeringen på Spamhaus-webbplatsen. Om IP-adressen finns med på principlistan över blockerade kan ägaren tilldela en annan statisk IP-adress eller ta bort adressen från principlistan över blockerade.

- För blockerade utgående meddelanden från din domän som är ansluten till Microsoft kan du få det här felet om meddelandena dirigeras via en tredjepartstjänst. Du kan använda WHOIS-sökverktyget för att hitta den blockerade IP-adressägaren.
