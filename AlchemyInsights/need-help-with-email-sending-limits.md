---
title: Behöver du hjälp med begränsningarna för att skicka e-post?
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
- "9002938"
- "5630"
ms.openlocfilehash: a13eec5d0d1abccd748653e7d7d9bb999b2e3b7a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58328844"
---
# <a name="need-help-with-email-sending-limits"></a>Behöver du hjälp med begränsningarna för att skicka e-post?

Nedan visas de **avsiktliga sändningsbegränsningarna** som tillämpas i tjänsten. Mer information om de här begränsningarna finns [här](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).

- För att hindra att oönskade massmeddelanden levereras tillämpar vi **begränsningar för alla utgående och interna meddelanden** per användare. Den här gränsen ligger på **10 000 mottagare per dag** för alla SKU:er.  Kunder som behöver skicka legitima, kommersiella massutskick (till exempel kundbrev) bör använda tredjepartsleverantörer som specialiserar sig i dessa tjänster.
    **Obs**: När gränsen har nåtts går det inte att skicka meddelanden från postlådan förrän antalet mottagare som under det senaste dygnet har mottagit meddelanden blir färre än gränsvärdet. Användaren kan inte skicka meddelanden förrän det har skett.
- Gränsen för meddelandehastigheten på **30 meddelanden per minut** gäller för alla SKU:er. Det här anger hur många meddelanden en användare kan skicka från sitt Exchange Online-konto inom en viss tidsperiod.
- Det **högsta antalet mottagare som tillåts i fälten Till, Kopia och Hemlig kopia** för ett enskilt e-postmeddelande är **1 000** för alla SKU:er. Om du vill anpassa den här gränsen kan du göra det [här](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).
