---
title: S/MIME i Outlook på webben
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666858"
---
# <a name="encrypt-email-messages-in-outlook"></a>Kryptera e-postmeddelanden i Outlook

Office 365-meddelandekryptering är byggd på Microsoft Azure Rights Management (Azure RMS), som är en del av informationsskydd i Azure. Om prenumerationen innehåller Azure Rights Management eller Azure informationsskydd, **du behöver inte vidta några åtgärder för att manuellt aktivera eller aktivera** tjänsten Rights Management.

Baserat på kundernas feedback kommer vi inte längre att aktivera Exchange e-flöde regler att automatiskt kryptera utgående e-post som innehåller en viss typ av känslig information i din innehavare som standard. I stället vi tillhandahåller detaljerade instruktioner om hur du gör det yourselves. Mer information om hur du skapar en transportregel om du vill kryptera känslig information finns i [den här artikeln](https://aka.ms/OmeEtr).

- Om du använder Outlook på webben (tidigare **OWA**): när du skriver ett e-postmeddelande, bara klicka på **skydda** i OWA. ”Gör inte framåt” behörighet gäller. Klicka på **Ändra behörighet** och välj **kryptera** endast kryptera meddelandet.

- Om du använder **Outlook-klienten**: Välj **Alternativ**om du vill skicka ett krypterat meddelande från Outlook 2013 och 2016 eller Outlook 2016 för Mac, > **behörigheter**och sedan välja alternativet skydd du behöver.

- Att **automatiskt kryptera all e-post** skickas till vissa mottagare eller externa partnerorganisationer, måste du skapa en regel för e-post flöde transport i Exchange Admin Center. Detaljerade anvisningar finns i [denna artikel](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

