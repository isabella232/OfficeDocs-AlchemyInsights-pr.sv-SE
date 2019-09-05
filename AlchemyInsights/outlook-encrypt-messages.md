---
title: S/MIME i Outlook på webben
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752878"
---
# <a name="encrypt-email-messages-in-outlook"></a>Kryptera e-postmeddelanden i Outlook

Office 365 meddelandekryptering bygger på Microsoft Azure Rights Management (Azure RMS), som är en del av Azure information Protection. Om din prenumeration innehåller Azure Rights Management eller Azure information Protection, **behöver du inte vidta några åtgärder för att manuellt aktivera eller aktivera** Rights Management-tjänsten.

Baserat på kundfeedback kommer vi inte längre att aktivera Exchange mail Flow-regler för att automatiskt kryptera utgående e-post som innehåller viss typ av känslig information i din klient som standard. I stället ger vi detaljerade instruktioner om hur ni kan göra det själva. Mer information om hur du skapar en transportregel för att kryptera känslig information finns i [den här artikeln](https://aka.ms/OmeEtr).

- Om du använder Outlook på webben (tidigare **OWA**): när du skriver ett e-postmeddelande klickar du bara på **skydda** i OWA. Detta kommer att gälla "vidarebefordra inte"-behörighet. Klicka på **Ändra behörighet** och välj **kryptera** för att bara kryptera meddelandet.

- Om du använder **Outlook-klienten**: om du vill skicka ett krypterat meddelande från Outlook 2013 eller 2016, eller Outlook 2016 för Mac, Välj **alternativ** > **behörigheter**, välj sedan det skyddsalternativ du behöver.

- Om du vill **kryptera alla e-postmeddelanden** som skickas till vissa mottagare eller externa partnerorganisationer automatiskt måste du skapa en transportregel för e-flöde i Exchange administratörs Center. Detaljerade instruktioner finns i [den här supportartikeln](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

