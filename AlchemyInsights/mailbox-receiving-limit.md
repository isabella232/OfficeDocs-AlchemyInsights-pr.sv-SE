---
title: Postlåda som tar emot begränsning vid tillämpning av begränsningar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/31/2021
ms.locfileid: "59316033"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Postlåda som tar emot begränsning vid tillämpning av begränsningar

Microsoft började nyligen tillämpa tröskelvärdet per postlåda på 3 600 meddelanden per timme. Mer information finns i [Exchange Online begränsningar](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits). Microsoft 365 postlådor som tar emot över 3 600 meddelanden inom en timme begränsas under de kommande 60 minuterna. 

Begränsningen för avsändarmottagare som blockerar meddelanden som tas emot av en Microsoft 365 från en viss avsändare tillämpas. Om en enskild avsändare skickar över 33 % av tröskelvärdet eller 1 200 meddelanden per rullande timme till en viss mottagare, startar SRP-gränsen och postlådan tar inte längre emot meddelanden från den avsändaren. Observera att:

- Den här gränsen gäller för e-postmeddelanden som tas emot från andra klientorganisationar, lokala avsändare eller Internetavsändare.
- E-postleveransen till postlådan har blockerats under de kommande 60 minuterna. 
- Avsändarna på de här postlådorna får en rapport om utebliven leverans (5.2.121 eller 5.2.122) som anger att postlådan har överskridit det maximala leveranströskelvärdet. Årsklientorganisationen (e-post inom samma klientorganisation) fortsätter att levereras.
- När SRP-gränsen tillämpas fortsätter den mottagande postlådan att ta emot meddelanden från andra avsändare.

Administratörer kan övervaka den aktuella postlådeaktiviteten genom att få åtkomst till en ny rapport och insikter i Exchange-administrationscentret som heter "Postlådor som överskrider mottagande gränser". Insikten visas bara om en klientorganisation har stötande postlådor, medan rapporten alltid visas på instrumentpanelen men är tom om inte en klientorganisation har stötande postlådor.

Mer information om hur du tar emot begränsningar finns i Postlådor som överskrider [den mottagande insikten om begränsningar i den nya EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Mer information om rapporten om att överskrida mottagargränser finns i Rapporten om postlådor som överskrider [mottagargränser i den nya EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)