---
title: Fel när e-post blockeras av SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783821"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Det gick inte att skicka e-post: klient värden blockerades med spamhaus

Den IP-adress som skickade meddelandet finns i en block lista som ägs av [spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Orsaker till att spamhaus är blockerade är inte säkert att konton, angripna datorer har en offentlig IP-adress och Internet leverantörens principer. Möjliga orsaker:
  
- För blockerade inkommande meddelanden där du styr käll-e-postservern måste du fastställa orsaken och ta bort det från spamhaus webbplats.

- För blockerade inkommande meddelanden där käll-IP-adressen tillhör någon annan måste adress ägaren ta bort blocket från spamhaus webbplats. Om IP-adressen finns i princip blockeringslistan (PBL) kan ägaren tilldela en annan statisk IP-adress eller ta bort adressen från PBL.

- Om du har blockerat utgående meddelanden från din domän som är ansluten till Microsoft kan du få det här felet om meddelandena cirkuleras via en tredjepartstjänst. Du kan använda ett WHOIS för att hitta den blockerade IP-adressen.
