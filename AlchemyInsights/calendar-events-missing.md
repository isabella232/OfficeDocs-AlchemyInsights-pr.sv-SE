---
title: Kalenderhändelser saknas eller uppdateras inte
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837589"
---
# <a name="calendar-events-missing-or-not-updating"></a>Kalenderhändelser saknas eller uppdateras inte

Om kalenderobjekt saknas eller inte uppdateras börjar du med att titta på antalet objekt i kalendermappens egenskaper i Outlook: 

1. Högerklicka på den aktuella **användarens kalendermapp** och välj sedan **Egenskaper**.

1. Välj **fliken Synkronisering.**

Om objektantalet inte är samma mellan servermappen och offlinemappen:

1.  Markera **mappen** Kalender.

1.  Gå till fliken / **Skicka/ta** emot och välj sedan **Uppdatera mapp**.

Om kalendern fortfarande inte uppdateras eller om händelser saknas hämtar du verktyget Calendar Checking Tool för Outlook från [Microsoft Download Center.](https://www.microsoft.com/download/details.aspx?id=28786) Avgör om det finns fler än 5 000 objekt i kalendermappen eftersom det kan orsaka symptom som kalendermöten som inte har uppdaterats eller mötesfel. 

Mer information finns i Prestandaproblem i Outlook när det finns för många objekt eller mappar i [en cachelagrad .ost- eller .pst-fil.](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders)